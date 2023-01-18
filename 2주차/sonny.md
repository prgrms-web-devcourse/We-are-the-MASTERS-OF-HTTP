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

멱등성 여부

- GET 메서드는 멱등성을 가진다. 
  - 1번 요청하나 2번 요청하나 결과가 변하지 않는다.
  - 서버 리소스에 변화를 일으키지 않기 때문에 안전한 메서드이다.
  - 멱등성을 가지는 메서드는 GET, HEAD, PUT, DELETE, OPTIONS가 있다

- POST 메서드는 멱등성을 가지지 않는다
  - 서버 리소스에 변화를 일으킨다.

- PUT, DELETE 메서드는 안전하지 않은 메서드이지만, 멱등성을 가진다.

</div>
</details>

<br>



URL의 포트는 어떤 역할을 하는가? 포트번호가 다르다는 것은 어떤 의미일까? CORS 정책에서 왜 포트번호가 다르면 다른 Origin(출처)로 인식할까?

- 포트번호: 하나의 호스트(서버)내에서 실행되고 있는 프로세스를 구분짓기 위해 사용하는 16비트 번호
- 포트번호가 다르다는 것은 다른 서비스(프로세스)라는 의미이다. CORS에서는 다른 Origin으로 인식한다.