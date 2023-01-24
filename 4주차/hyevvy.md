# 내용 공유

# 관련 자료

# 4주차 내용 퀴즈

## 6장 : 프락시

#### 1. 웹 서버는 특정 웹사이트에 방문한 사용자들이 언제, 어디서, 어떤 페이지를 방문하였는지에 대한 정보를 기록한 파일이다. 로그를 실시간 모니터링할 때 쓰는 명령어는 무엇인가?

<details>
<summary>답안</summary>
<div markdown="1">

tail

</div>
</details>

<br>

#### 2. 웹 서버는 경로가 파일이 아닌 디렉터리를 가리키는 디렉터리 URL에 대한 요청을 받으면 무조건 에러를 반환한다

<details>
<summary>답안</summary>
<div markdown="1">

(p.140) X

- 에러를 반환하거나
- 디렉터리 대신 특별한 '색인 파일'을 반환하거나
- 디렉터리를 탐색해 그 내용을 담은 HTML 페이지를 반환한다

</div>
</details>

#### 3. 프락시 URI와 서버 URI는 어떻게 다른가?

<details>
<summary>답안</summary>
<div markdown="1">

(p.164) 웹 서버와 웹 프락시 메시지의 문법은 서로 같지만, 클라이언트가 프락시 대신 서버로 요청을 보내면 요청의 URI가 달라진다.
클라이언트가 웹 서버로 요청을 보낼 때, 요청줄은 스킴, 호스트, 포트번호가 없는 부분 URI를 가진다.
그러나 클라이언트가 프락시로 요청을 보낼 때, 요청줄은 완전한 URI를 가진다.

</div>
</details>

#### 4. 모든 프락시와 게이트웨이는 \***\*\_\_\_\_\*\***을 지원해야한다.

<details>
<summary>답안</summary>
<div markdown="1">

(p.178) Max-Forwards

</div>
</details>

## 7장 : 캐시

#### 1. 메모리 계층 구조란?

<details>
<summary>답안</summary>
<div markdown="1">

메모리 계층 구조(Memory hierarchy)란 메모리를 필요에 따라 여러 가지 종류로 나누어 둠을 의미한다[1]. 이때 필요한 대부분의 경우 CPU가 메모리에 더 빨리 접근하기 위함이다.
데이터 저장 공간을 속도-용량 순서대로 쌓으면 마치 아래와 같은 피라미드와 같은 형상이 나타난다.

<img width="222" alt="메모리 계층 구조" src="https://user-images.githubusercontent.com/72402747/214280127-46bdeb13-9cd0-4b2a-b25f-49535e0ee73e.png">

출처) [위키백과 - 메모리 계층 구조](https://ko.wikipedia.org/wiki/%EB%A9%94%EB%AA%A8%EB%A6%AC_%EA%B3%84%EC%B8%B5_%EA%B5%AC%EC%A1%B0)

</div>
</details>

<br>

#### 2. 클라이언트 입장에서 응답이 캐시에서 왔는지 원 서버에서 왔는지 어떻게 구별할 수 있는가?

<details>
<summary>답안</summary>
<div markdown="1">

(p.193)

1. 응답의 Date 헤더 값과 현재 시각을 비교하여 응답의 생성일이 더 오래되었다면 응답이 캐시된 것이다
2. 응답이 얼마나 오래되었는지 확인하는 Age 헤더를 이용하는 것이다.

</div>
</details>

#### 3. 캐시 처리 단계는?

<details>
<summary>답안</summary>
<div markdown="1">

(p.198)

1. 요청받기
2. 파싱
3. 검색
4. 신선도 검사
5. 응답 생성
6. 발송
7. 로깅

</div>
</details>
