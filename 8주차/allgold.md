# 8주차 내용 퀴즈

## 15장 : 엔터티와 인코딩

### 1. 지속 커넥션에서 `Content-Length` 헤더가 필수인 이유는

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

`Content-Length` 헤더는 클라이언트에게 메시지 하나가 어디서 끝나고 다음 시작은 어디인지 알려준다.

</div>
</details>

---

### 2. HTTP 에서 여러 다른 종류와 길이와 값으로 채워진 폼을 허용하기 위해 사용하는 MIME 타입은?

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

`Content-Type: multipart/form-data` 나 `Content-Type: multipart/mixed` 헤더에 멀티파트 본문을 함께 보낸다.

</div>
</details>

---

### 3. 조건부 요청의 강한 검사기와 약한 검사기 의 예시는?

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

강한 검사기 : ETag
약한 검사기 : 최종 변경 시각

- 보너스 문제 : 강한 검사기를 약한 검사기로 사용하려면?

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

> 클라이언트와 서버는 때때로 엔터티 태그 검사를 통과하지 못한 버전을 채택하는 경우가 있다. 예를 들어 서버는 크고 자주 찾는 캐시된 문서에 대해, 캐시의 재검사로 인한 대량 전송을 유발하지 않으면서 겉모양새만 약간 고치고 싶을 수도 있다. 이 경우, 서버는 태그 앞에 'W/' 를 붙이면서 ‘약한’ 엔터티 태그임을 알린다. (419p)

</div>
</details>

</div>
</details>

---

### 4. 범위 요청을 하기 위하여 서버는 1) `_________` 헤더를 사용하고 클라이언트는 2) `_________` 헤더를 사용한다.

### 클라이언트의 2) `_________`헤더는 3) `_________` 서비스에서 멀티미디어 파일의 다른 부분을 여러 다른 피어로부터 동시에 다운로드 받을 때도 널리 사용한다.

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

1. `Accept-Range`
2. `Range`
3. `P2P`

</div>
</details>

---

### 5. ETag를 사용하는 조건부 헤더 2가지와, 해당 조건부 헤더에 대해서 설명해주세요

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

1. `If-Match` : 지난번 ETag 응답 헤더에 들어있던 것과 엔터티 태그가 같다면 그 리소스의 사본을 보내라.
2. `If-None-Match` : 지난번 ETag 응답 헤더에 들어있던 것과 엔터티 태그가 다르다면 그 리소스의 사본을 보내라.
</div>
</details>
