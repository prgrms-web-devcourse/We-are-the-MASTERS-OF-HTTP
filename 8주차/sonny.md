# 8주차 내용 퀴즈

## 15장 : 클라이언트 식별과 쿠키

### Q) 엔터티 본문은 가공된 데이터로 엔터티 헤더가 그 데이터의 의미를 설명한다.

<details>
<summary>답안</summary>
<div markdown="1">
A) X

엔터티 본문은 가공되지 않는 Raw한 데이터이다. 엔터티 헤더가 그 데이터의 의미에 대해서 설명한다.
</div>
</details>

<br>



### Q) Content-Type 헤더 필드는 엔터티 본문의 MIME 타입을 기술한다 (O/X)
Q-1) MIME 타입이란 무엇인가요?

<details>
<summary>답안</summary>
<div markdown="1">
A) O

A-1) MIME 타입은 데이터 형식을 기술한다.
- text/html : 엔터티 본문은 HTML 문서
- text/plain : 엔터티 본문은 일반 텍스트 문서
- 등등


</div>
</details>

<br>



### Q) 콘텐츠를 서버에서 동적으로 생성하는 경우, 콘텐츠의 본문 길이를 알 수 없기 때문에 Content-Length 길이를 알 수 없다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

### 쿠키 Path 속성, Domain 속성
A) O
</div>
</details>

<br>


### Q) 청크 인코딩을 사용하면 본문을 여러 청크로 쪼개 보낼 수 있기때문에 동적으로 본문을 생성할 수 있다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">
A) O

</div>
</details>
<br>


### Q) 메시지 잘림은 캐싱 프록시 서버에 특히 취약하다. 이를 방지하기 위해 캐싱 프록시 서버는 Content-Length 헤더를 지니지 않은 HTTP 본문은 보통 캐싱하지 않는다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">
A) O


</div>
</details>
<br>


