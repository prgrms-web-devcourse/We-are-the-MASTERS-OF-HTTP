# 2주차 내용 퀴즈

## 3장 : HTTP 메시지

### 1. HTTP 1.1 GET 메서드에는 메시지 본문을 사용할 수 없다(O/X)

<details>
<summary>답안</summary>
<div markdown="1">

X, 사용할 수도 있다.

- 2014년에 이후에 나온 RFC 7230-7237에서 개정되었다.(GET 메시지는 메시지 본문이 없다라는 문구가 삭제되었다.)
- elastic search는 GET 메서드에 메시지 본문을 함께 사용하고 있다.
```
GET /_search
{
  "query": {
    "query_string": {
      "query" : "foo"
    }
  }
}
```
- 그러나 프레임워크, 서버등에서 GET 메서드의 메시지 본문사용을 지원 하지 않는 경우가 많다.
- 정리하면 스펙 상으로는 사용할 수도 있다. 그러나 왠만하면 사용하지 말자. 사용하려면 잘 확인하고 사용하자

</div>
</details>

<br>


### 2. CORS(Cross Origin Resource Policy)를 해결하기 위해 설정되는 응답 헤더에는 어떤 것이 있나요?

<details>
<summary>답안</summary>
<div markdown="1">


응답 헤더 - `Access-Control-Allow-Origin`
- 브라우저에게 리소스에 접근할 수 있는 출처를 알려줌
  
Access-Control-Allow-Origin : *
- 모든 출처의 요청을 허용하도록 브라우저에게 지시함

Access-Control-Allow-Origin : www.test.com
- www.test.com의 요청만 허용하도록 브라우저에게 지시함 ()
- 만약 www.test2.com에서 요청을 한다면 브라우저는 요청을 막고 에러를 발생함
- CORS는 브라우저에서 구현, 사용하는 브라우저 보안


</div>
</details>

<br>


### 3. GET 메서드와 POST 메서드의 차이는 무엇인가요?
<details>
<summary>답안</summary>
<div markdown="1">

서버에 Side Effect 여부. 어려운 말로 멱등성을 가지는지

- GET 메서드는 멱등성을 가진다 (안전한 메서드)
  - 몇번의 요청을 보내도 서버의 상태는 항상 동일하다
  - 멱등성을 가지는 메서드 GET, HEAD, PUT, DELETE, OPTIONS가 있다
  - 결국은 메서드가 자동으로 멱등성을 가지는 것이 아니라, 개발자가 메서드들이 멱등성을 지키게 구현하도록 노력해야한다.
  
- POST 메서드는 멱등성을 가지지 않는다

</div>
</details>

<br>
