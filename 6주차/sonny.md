# 6주차 내용 퀴즈

## 11장 : 클라이언트 식별과 쿠키

###
- 브라우저는 브라우저에 저장된 모든 쿠키를 모든 사이트에 전송한다 (O/X)
- Set-Cookie 응답 헤더의 Domain 속성은 어떤 사이트가 그 쿠키를 읽을 수 있는지 브라우저에게 알려준다
<details>
<summary>답안</summary>
<div markdown="1">

전부 O

</div>
</details>

<br>



### 서버가 사용자을 식별할 수 있는 방법은 어떤것들이 있을까요?

<details>
<summary>답안</summary>
<div markdown="1">

1. 사용자 정보를 전달하는 HTTP 요청헤더
    - From
    - User-Agent
    - Referer
    - Authorization
    - Client-ip
    - X-Forwarded-For
    - Cookie
2. 클라이언트의 IP 추적 후 IP 주소로 식별

3. 사용자 로그인 (사용자의 토큰을 Authorization 헤더에 담아 전송)
4. URL에 식별자를 포함하는 기술 Fat URL
5. 쿠키

</div>
</details>

<br>



### 다음 Set-Cookie 헤더는 무슨 의미일까요?

```
Set-Cookie: domain: "abcdefg.com"; path="/test/"
```

<details>
<summary>답안</summary>
<div markdown="1">

### 쿠키 Path 속성, Domain 속성

특정 Path, Domain에 접근해야 쿠키를 받는다

http://abcdefg.com/test/에 접근하면 쿠키를 받게 된다.

</div>
</details>

<br>

