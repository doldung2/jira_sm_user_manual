# JIRA Service Management 사용자 메뉴얼

## 1. 티켓 접수

### 1.1 포탈을 통한 티켓 접수(고객이 접수하는 채널)
#### 요약, 설명필드에 문의 제목 및 내용을 상세히 기재하고, 필요 시 캡쳐파일등을 첨부파일로 첨부한다.<br> (화면에 보이는 "대신 이 요청을 제기합니다" 관리자가 포탈을 통해서 접수하는 경우만 보인다)

<kbd>
    <img src = ./images/user_001.png width=500>
</kbd><p><br></p>


### 1.2 관리화면을 통한 티켓 접수(내부직원이 접수하는 채널)

#### 화면 상단의 "만들기" 버튼을 누르면 나오는 팝업 창에서 생성

<kbd>
    <img src = ./images/user_002.png>
</kbd><p><br></p>

> 화면은 아래처럼 2가지 용도로 구분된다. 소스 변경이 필요한 오류 및 현장지원 건의 경우 8개의 탭으로 구성되어있고, 각 프로세스 단계별로 입력하도록 되어있는 반면 "프로젝트 기술지원 및 자료요청"의 경우에는 별도 탭없이 필드(요약, 지원요청부서, 지원내역, 첨부파일)로만 구성되어있다.

#### 1.2.1 오류 및 기술지원인 경우

<kbd>
    <img src = ./images/user_003.png width=500><br>
</kbd>
<!--<p align="center">"오류 및 기술지원 화면"의 화면 구성</p>-->

#### 1.2.2 프로젝트 기술 지원 및 자료 요청의 경우

##### 내부 사용자들만 접근가능하며, 사내 외부팀을 지원할 때 생성하는 요청입니다.(트라이얼 이용신청의 경우도 해당 요청 티켓을 이용)

> 요약: 지원 내용 또는 프로젝트 명을 입력합니다.<br>
> 지원요청부서: 지원을 요청한 팀 또는 그룹을 입력합니다.<br>
> 지원요청자: 지원요청부서의 담당자 또는 PM을 입력합니다.<br> 
> 지원시작일: 실제 지원이 시작된 일자를 선택합니다.(트라이얼의 경우 MCM 제공 시작일자 - 협의된 시작일이 아닌 실제 시작일)<br> 
> 지원종료일: 실제 지원이 종료된 일자를 선택합니다.(트라이얼의 경우 MCM 제공 종료일자 - 협의된 종료일이 아닌 실제 종료일)<br> 
> 지원내역: 지원내역을 기재합니다.<br> 

<kbd>
    <img src = ./images/user_004.png width=500><br>
</kbd>
<!--<p align="center">"프로젝트 기술 지원 및 자료 요청"의 화면 구성</p>-->

## 2. 티켓 작성 가이드(Tab별 안내)

### 2.1 내용
#### 포털/내부사용자 발급 티켓에서 공통적으로 사용되는 필드입니다.
> 요약: 제목을 의미합니다.<br>
> 설명: 오류 및 요청사항을 수신자가 이해하기 용이하도록 정리해서 기재합니다.<br>
> 첨부파일: 오류 현상에 대한 화면 캡쳐 또는 사진 촬영이 가능한 경우 첨부합니다.(optional)<br>

<kbd>
    <img src = ./images/user_005.png width=500>
</kbd>

### 2.2 추가정보
#### 내부 사용자들만 접근가능하며, 고객은 입력할 수 없는 필드로 구성되어있습니다.

> 우선순위: Task의 우선순위이며, 우선순위에 대한 정의는 아래 별도 기재<br>
> 연결된 이슈/이슈: 특정 이슈와 중복 건인지, 아니면 이슈의 원인이되는 또 다른 이슈인지를 정의<br>
> 서비스: 이슈가 발생한 product를 의미함.(ex> pipeline, rpm1.0 등. 중복선택 가능.)<br>
> 고객사: 제품 구매 고객사를 선택합니다.(고객이 조회되지 않는 경우 채널파트에 등록 요청)<br>
> AM담당자/채널담당자/개발담당자/테스트담당자: 각 단계별 담당자. 최초에는 AM/채널 담당자만 기재 필수<br>
> 완료희망일자: 고객이 완료를 희망하는 날짜이며, 최종 반영일자와는 상이할 수 있음.(최종 반영일자는 배포탭에서 관리함)<br>

*우선순위 정의
우선순위 | 설명 | 예시
----- | ----- | -----
Highest|우회 또는 대체할 수 있는 방법이 없는 오류|장애 (서비스 진행 불가 또는 당월 정기작업 오류)
High|오류가 발생하였지만 우회방안이 있는 경우|관리자 권한 부여(DB insert 작업으로 우회) 또는 당월은 처리되었응나 익월 정기작업에 영향이 있는 경우
Medium|완료 일자가 존재하는 요구사항 또는 서비스 확인|일반적인 개발 요구 사항 및 자료 요청
Low|고객과 합의된 완료 일정이 없는 요구사항|요구 사항에 없는 신규 기능 개발
Lowest|미사용 서비스의 오류, 보류된 요구 사항|랜처 환경의 개선 or RPM 2.0 이후 개발 가능 건

<kbd>
    <img src = ./images/user_006.png width=500>
</kbd>

### 2.3 원격지원
#### 오류에 대한 원격지원 시 기재합니다. 원격지원은 접수전화 및 전화/이메일 문의등이 있으며, 터미널을 통한 리모트 대응도 포함됩니다.

> 원격지원 결과: 원격지원 결과를 선택합니다. 해결/현장지원필요/없음 중 택1.<br>
> 원격지원 Comment: 원격지원 중에 있었던 특이사항을 기재합니다.<br>

<kbd>
    <img src = ./images/user_007.png width=500>
</kbd>

### 2.4 현장지원
#### 현장지원이 발생한 경우 기재하는 탭입니다.

> 현장지원 일자: 현장 방문한 일자를 등록합니다.(여러번 방문한 경우에는 최종 방문일자를 update하고, 과거 방문일자를 comment란에 기입합니다.)<br>
> 현장지원 결과: 현장지원 결과를 선택합니다. 해결/소스변경필요/없음 중 택1.<br>
> 현장지원 Comment: 현장지원 중에 있었던 특이사항을 기재합니다.<br>

<kbd>
    <img src = ./images/user_008.png width=500>
</kbd>

### 2.5 요건협의
#### 요구사항협의중에 나온 내용을 기재하는 탭입니다.

> 배포예정일자: 요구사항협의 중 고객과 합의된 반영일자를 등록합니다. (고객사 사정에 의해 최종 반영일자와 상이할 수 있음.)<br>
> 요건협의내용: 요구사항에 대해서 정리하여 입력합니다.<br>

<kbd>
    <img src = ./images/user_009.png width=500>
</kbd>

### 2.6 개발
#### 개발된 내용에 대해서 기재하는 탭입니다.

> 개발내용: 개발된 내용을 기술 또는 변경된 소스를 복사/붙여넣기 합니다.<br>
> 단위테스트 체크리스트: 단위 및 기능테스트에 대한 점검 체크리스트입니다.<br>
> 개발 Comment: 개발 중 발생한 특이사항에 대해서 입력합니다.<br>

<kbd>
    <img src = ./images/user_010.png width=500>
</kbd>

### 2.7 테스트
#### 사용자테스트 내용에 대해서 기재하는 탭입니다.

> 사용자 테스트 체크리스트: 사용자 테스트에 대한 점검 체크리스트입니다.<br>
> 테스트 Comment: 테스트 중 특이사항 및 테스트 결과에 대해서 등록합니다.<br>

<kbd>
    <img src = ./images/user_011.png width=500>
</kbd>

### 2.8 배포
#### 배포 내용에 대해서 기재하는 탭입니다. 

> 배포 담당자: 배포를 담당한 담당자를 등록합니다.<br>
> 실제 배포일자: 고객사에 실제 반영된 일자를 등록합니다.<br>
> 배포 Comment: 배포 진행 중 특이사항 및 leassoned learn 내용을 기재합니다.<br>

<kbd>
    <img src = ./images/user_012.png width=500>
</kbd>

## 3. 티켓 처리 가이드

### 3.1 전체 워크플로우
#### 요청 유형별로 "운영지원", "1차요청" 으로 분기처리된다.

<kbd>
    <img src = ./images/user_013.png>
</kbd>

#### 3.1.1 운영 지원
##### 이슈 만들기에서 요청 유형을 "프로젝트 기술 지원 및 자료요청"으로 선택하거나, 이슈 유형을 "Accu Support Issue"으로 할 경우 해당 워크플로우로 티켓이 수행된다.(Accu Support Issue로 요청은 요청 유형이 자동으로 mapping되지 않으므로 사용을 자제하시기 바랍니다.)

> 주로 내부 프로젝트를 지원하거나, Trial 사용 요청에 대한 티켓을 관리할 때 해당 워크플로우로 수행된다.<br>
> 화면 및 필드 내용은 앞에서 소개한 <a href=https://github.com/doldung2/jira_sm_user_manual/blob/main/jira_user_manual.md#122-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EA%B8%B0%EC%88%A0-%EC%A7%80%EC%9B%90-%EB%B0%8F-%EC%9E%90%EB%A3%8C-%EC%9A%94%EC%B2%AD%EC%9D%98-%EA%B2%BD%EC%9A%B0>1.2.2 프로젝트 기술 지원 및 자료 요청의 경우</a>를 참고하시면 됩니다.
<kbd>
    <img src = ./images/user_014.png>
</kbd>


#### 3.1.2 1차 요청
##### 이슈 만들기에서 요청 유형을 "단순문의", "기술지원", "오류접수"로 선택하거나, 이슈 유형을 "Accu Common Issue"로 할 경우 해당 워크플로우로 티켓이 처리된다. 1차대응은 AM담당자에 의해서 자체 해결될 경우 해당 단계에서 마무리되며, 2차지원부터는 프로그램 변경이 검토된다.(Accu Common Issue로 요청은 요청 유형이 자동으로 mapping되지 않으므로 사용을 자제하시기 바랍니다.)

> 주로 고객사에서 오류 및 문의 접수가 되는 경우에 해당 워크플로우가 수행된다.<br>
> 만약 원격지원 또는 현장지원으로 문의/오류가 해결될 경우 해당 탭만 내용이 기재되면 완료 가능하다. <br>
> 만약 소스 변경이 필요한 경우에는 뒷쪽에 위치한 탭에 모든 필드가 기재되어야만 완료가 가능하다 <br>
> 화면 및 필드 내용은 앞에서 소개한 <a href=https://github.com/doldung2/jira_sm_user_manual/blob/main/jira_user_manual.md#2-%ED%8B%B0%EC%BC%93-%EC%9E%91%EC%84%B1-%EA%B0%80%EC%9D%B4%EB%93%9Ctab%EB%B3%84-%EC%95%88%EB%82%B4>티켓 작성 가이드(Tab별 안내)</a>를 참고하시면됩니다.
<kbd>
    <img src = ./images/user_015.png>
</kbd>