# JIRA Service Management 개발팀 업무 메뉴얼

## 1. 이슈 유형별 티켓 처리 가이드

### 1.1 이슈유형: Accu Common Issue

<kbd>
    <img src = ./images/dev_001.png width=1024>
</kbd><p><br></p>

#### 1.1.1. 추가정보 탭

<kbd>
    <img src = ./images/dev_002.png width=600>
</kbd><p><br></p>

#### 1.1.2. 현장지원 탭
```
현장지원일자: 사이트에 다녀온 날짜를 입력. (여러번 다녀온 경우에는 최종일자로 수정)
현장지원결과: 원인 확인 및 조치가 완료된 경우에는 완료. 별도 소스 변경이 필요한 경우에는 "소스변경필요" 선택
          (단순 서버 재기동에 의한 해결의 경우에는 root cause가 해결된 상황은 아니므로 "미해결종료"로 등록)
현장지원 Comment: 현장에서 확인한 내용 및 특이사항 기재 (가급적 상세하게...)
```
<kbd>
    <img src = ./images/dev_003.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/dev_004.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/dev_005.png width=600>
</kbd><p><br></p>

#### 1.1.3. 개발 탭
```
개발 내용: 개발 내용에 대해서 간략히 기재 또는 mytask 상의 고유번호
단위 테스트 체크리스트: 추후 상세화 예정
개발 Comment: 테스트 시 유의 사항 및 영향도에 대해선 언급 필요.
             테스트 환경 (Local에서 수행 or 테스트서버가 있는 경우 해당 서버 정보)

* 개발 완료 이후 해당 티켓의 상태를 "개발" -> "테스트 요청" 으로 변경 (AM에서 적용이 가능한 상태인지 확인하기 위함.)
```
<kbd>
    <img src = ./images/dev_006.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/dev_007.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/dev_008.png width=600>
</kbd><p><br></p>

#### 1.1.4. 테스트 탭
```
테스트 Comment: 테스트 중에 발생한 특이사항 기재
```
<kbd>
    <img src = ./images/dev_009.png width=600>
</kbd><p><br></p>

#### 1.1.45. 배포
```
배포담당자: 직접방문하는 경우에는 개발팀 방문자를 기입
실제 배포일자: 사이트 적용일자 (반영 이후 변경하고, 여러차례 발생할 경우 최종일자로 update)
배포 Comment: 배포간에 발생힌 특이 사항
```
<kbd>
    <img src = ./images/dev_010.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/dev_011.png width=600>
</kbd><p><br></p>

## 2. Notification 을 위한 메일 설정

### 2.1 설정 순서

Step 1. VDI내부의 제어판을 열고 "Mail (Mircosoft Outlook XXXX)" 항목을 클릭 (Outlook 종료 상태에서 해야 함.)
<kbd>
    <img src = ./images/outlook_00.png width=600>
</kbd><p><br></p>

Step 2.프로필에 위치한 "프로필 보기" (하단의 붉은색 영역)을 클릭
<kbd>
    <img src = ./images/outlook_05.png width=600>
</kbd><p><br></p>

Step 3.아래 화면에서 추가 버튼을 클릭(아래의 옵션은 "사용할 프로필 선택"을 선택한다.)
<kbd>
    <img src = ./images/outlook_04.png width=600>
</kbd><p><br></p>

Step 5.팝업된 "새프로필" 창에서 프로필 이름을 입력한다.(개인별로 관리하기 쉽도록 임의로 입력)

Step 6.전환된 "계정추가" 창에서 부여받은 전자메일 주소는 "~~~~@skcc.com" (별도로 공유)를 입력, 입력 후 "다음" 클릭
    (개인 메일 및 본인 사내 메일 입력 금지!)

Step 7. 이후 outlook 실행


만약 아래와 같은 프로필 설정화면이 나올 경우 Outlook을 선택하시고, "확인"을 누르시고    
<kbd>
    <img src = ./images/outlook_02.png width=600>
</kbd><p><br></p>

아래처럼 자격증명 화면이 나올 경우에는 하단의 "다른 계정 사용"을 누르고, 부여받은 ID/PW를 입력한다.
<kbd>
    <img src = ./images/outlook_03.png width=600>
</kbd><p><br></p>

최종 설정 완료되면 아래와 같이 Outlook 좌측에 아래와 같이 개인 계장(윗쪽 녹색영역)과 시스템 계정(붉은색 박스)이 모두 보이면 설정 완료.
<kbd>
    <img src = ./images/outlook_06.png width=600>
</kbd><p><br></p>
