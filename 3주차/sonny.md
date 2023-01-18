# 3주차 내용 퀴즈

## 5장 : 웹 서버

### 1. 웹 서버가 하는 일을 7가지를 순서대로 알려주세요.

<details>
<summary>답안</summary>
<div markdown="1">

1. 클라이언트와 커넥션을 맺는다.
2. HTTP 요청을 받아들이고 요청 메시지를 읽는다.
3. 요청 메시지를 해석하고 처리한다.
4. 요청 메시지에서 지정한 리소스에 접근한다.
5. HTTP 응답 메시지를 생성한다.
6. 응답을 클라이언트에게 보낸다.
7. 트랜잭션을 로그에 남긴다.


</div>
</details>

<br>


### 2. 웹 서버는 경로가 디렉터리를 가리키는 URL에 대한 요청이 왔을 때 index.html으로 이름 붙은 파일을 찾아 응답한다.

<details>
<summary>답안</summary>
<div markdown="1">

O

</div>
</details>

<br>


### 3. MIME 타입은 파일,데이터 타입을 식별하기 위해 사용한다. HTTP 응답 헤더 Content-Type 헤더에 명시된다.
<details>
<summary>답안</summary>
<div markdown="1">

O

</div>
</details>

<br>


### 4. 프락시를 사용하는 이유는 무엇일까요?(프락시의 기능)
<details>
<summary>답안</summary>
<div markdown="1">

- 필터링
- 접근 제어
- 보안 방화벽
- 웹 캐시
- 대리 프록시(웹 서버처럼 동작)
- 콘텐츠 라우터(인터넷 트래픽 조건과 콘텐츠 종류, 필터링에 따라 특정 웹 서버로 라우팅)
- 트랜스코더 (데이터 포맷을 변환)
- 익명화 (신원을 식별할 수 있는 특성들을 제거)
- 
</div>
</details>

<br>


### 5. 리버스 프락시(대리 프락시)는 네트워크 끝 단의 웹 서버 가장 앞에 위치하여 웹 서버로 향하는 모든 요청을 처리할 수 있다.
<details>
<summary>답안</summary>
<div markdown="1">

리버스 프록시
- 네트워크 끝 단의 웹 서버 바로 앞에 위치
- 웹 서버에 보안 기능을 추가
- 웹 서버 캐시로 성능 개선
</div>
</details>

<br>


### 6. 클라이언트 트래픽이 프락시로 가도록 하는 네 가지 방법은 무엇인가요?
<details>
<summary>답안</summary>
<div markdown="1">

1. 클라이언트를 수정
    - 브라우저의 프락시 설정을 사용하여 HTTP 요청을 바로 프락시로 보낸다.
2. 네트워크를 수정
    - 네트워크 인프라를 가로채어 웹 트래픽을 프락시로 가도록 조정(인터셉터 프락시)
3. DNS 이름 테이블을 수정
    - 리버스 프락시는 웹 서버의 이름과 IP주소를 자신이 직접 갖는다. 그래서 모든 요청이 웹 서버가 아닌 리버스 프락시로 간다.
    - DNS 이름 테이블을 직접 수동편집하거나 동적 DNS 서버를 사용하여 조정한다.
4. 웹 서버를 수정
    - HTTP 리다이렉션 명령을 클라이언트에게 응답함으로서 클라이언트의 요청을 프락시로 리다이렉트하게 한다.
</div>
</details>

<br>


### 7. 리액트 CRA를 개발환경(dev)에서 실행하면 CORS가 허용되는 이유는 무엇인가?
<details>
<summary>답안</summary>
<div markdown="1">

webpack이 프록시 서버를 만들고, 브라우저 설정으로 프록시에 요청을 보내도록 한다.

```js
module.exports = {
  devServer: {
    proxy: {

    }
  }
};
```

<img src="https://joshua1988.github.io/webpack-guide/assets/img/proxy.dce9d87c.png"  width="500"/>

</div>
</details>

<br>