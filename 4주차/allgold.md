# 4주차 내용 퀴즈

## 6장 : 프락시

### 1. 프락시를 넘나드는 메시지의 흐름을 추적하는 방법 2가지

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

1. Via 헤더 필드 사용하기
2. TRACE 메서드 사용하기

</div>
</details>

---

### 2. 프락시의 사용 예제

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

**프락시 서버는 실용적이고 유용한 것이라면 무슨 일이든 한다.**

- 필터
- 보안 방화벽
- 웹 캐시
- 대리 프락시
- 콘텐츠 라우터
- 트랜스코더
- 익명화 프락시

</div>
</details>

---

## 7장 : 캐시

### 3. `If-Modified-Since` 조건을 통하여 GET 요청을 하였을 떄, 재검사가 적중하였다면 메시지 본문에 서버 객체의 내용을 첨부하여 응답한다. (O / X)

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

X
(책 205)
재검사가 적중하였다 = 캐시의 해당 데이터가 신선한 상태이다.
서버는 작은 `304 Not Modified` 응답을 클라이언트에게 돌려주며, 효율을 위하여 본문은 보내지 않는다.

</div>
</details>

---

### 4. 응답헤더 Expires와 max-age의 차이점과 이 중에서 Expires를 사용하지 않도록 권고하는 이유는?

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

Expires : 절대 유효기간 명시
max-age : 문서의 최대 나이 정의

절대 시계의 경우 컴퓨터의 시계가 올바르게 맞추어져 있을 것을 요구하지만, 그러지 않을 가능성이 높음.

### **보너스 문제 : `max-age` 를 사용하는 경우, 캐시가 매 접근마다 문서를 캐시하지 않거나 혹은 매 접근마다 리프레시 하도록 요청하는 방법은?**

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

해당 값을 0으로 설정한다.
`Cache-Control: max-age=0`

</div>
</details>

</div>
</details>

---

### 5. 캐시의 효과를 어떻게 측정할 수 있나요? 또한 이러한 측정 방법이 시사하는 바는?(2가지)

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

cache-hit-rate 사용.
이는 문서 적중률과 바이트 적중률로 나뉨

- 문서 적중률 : 캐시가 요청을 처리하는 비율 ⇒ 문서 적중률이 높다는 것은 캐시에서 요청을 대부분 처리했다는 의미이므로 원 서버까지의 지연이 줄어들었다는 의미이다.
- 바이트 적중률: 캐시를 통해 제공된 모든 바이트의 비율 ⇒ 바이트 적중률이 높다는 것은 캐시를 통해 많은 용량이 제공되었다는 의미이므로 네트워크 대역폭에서 이득을 보았다는 의미이다.

</div>
</details>
