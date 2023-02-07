# 6주차 내용 퀴즈

## 11장: 클라이언트 식별과 쿠키

### 1. HTTP 프로토콜의 `stateless` 에 대해서 설명하시오.

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

연결 자체에 대한 정보를 가지지 않으며, 각 요청 및 응답이 독립적으로 일어난다.

</div>
</details>

---

### 2. 쿠키의 타입은 `_______________` 애 따라 `__` 쿠키와 `__` 쿠키로 나눌 수 있다.

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

- 보너스 문제 : 쿠키를 세션 쿠키로 설정하는 방법은?

<details>
<summary>답안</summary>
<div markdown="1">

Discard 파라미터가 설정되어 있거나, Expires, Max-Age 파라미터가 없으면 세션 쿠키가 된다

</div>
</details>

</div>
</details>

---

### 3. 쿠키의 속성 중 domain 속성과 path 속성에 대한 설명

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

- `Domain` : 서버는 쿠키를 생성할 때 Set-Cookie 응답 헤더에 Domain 속성을 기술해서 **어떤 사이트가 그 쿠키를 읽을 수 있는지** 제어할 수 있다.
- `Path` : 웹 사이트 일부에만 쿠키를 적용할 수 있다. URL 경로의 앞부분을 가리키는 Path 속성을 기술해서 **해당 경로에 속하는 페이지에만 쿠키를 전달**한다.

</div>
</details>

---
