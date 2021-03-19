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
          (단순 서버 재기동에 의한 해결의 경우에는 root cause가 해결된 상황은 아니므로 "문제등록필요"로 등록)
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
테스트 Comment
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

<kbd>
    <img src = ./images/outlook_00.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/outlook_02.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/outlook_03.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/outlook_04.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/outlook_05.png width=600>
</kbd><p><br></p>

<kbd>
    <img src = ./images/outlook_06.png width=600>
</kbd><p><br></p>
