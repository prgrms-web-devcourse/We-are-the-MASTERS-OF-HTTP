# 10주차 내용 퀴즈

## 17장 내용협상과 트랜스코딩

### 1. O/X퀴즈

- 서버 주도 내용 협상에서 적절한 리소스를 제공할 수 없는 경우, `300(Multiple Choices)`, `406(Not Acceptable)` 이나 `415(Unsupported Media Type)` 로 응답할 수 있다.
- 브라우저에서 특정 사이트를 접속할 때, 브라우저 언어 설정을 통하여 요청의 `Accept-Language` 값을 자동으로 설정할 수 있다.

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

1. O (참고자료 : [MDN - Content negotiation](https://developer.mozilla.org/en-US/docs/Web/HTTP/Content_negotiation))

> The 300 (Multiple Choices) or 406 (Not Acceptable), 415 (Unsupported Media Type) HTTP response codes by the server (agent-driven negotiation or reactive negotiation), that are used as fallback mechanisms.

2. O (참고자료 : [MDN - Accept Language](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language))

> Browsers set required values for this header according to their active user interface language.

</div>
</details>

<br>

### 2. Content Negotiation 에서 `Vary` 헤더는 어떻게 사용되는가?

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

해당 헤더를 통하여, 콘텐츠 협상에 실제로 사용한 헤더(관련 요청 헤더)를 표시하여 캐시가 최적으로 작동할 수 있게함.
프록시를 낀 투명 협상을 이용하려면 이 헤더를 사용함

</div>
</details>

---
