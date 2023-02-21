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


### Q) 전송 인코딩을 제어하고 서술하기 위해 정의되는 헤더 필드는 Transfer-Encoding, TE이다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">
A) O

Transfer-Encoding: 어떤 인코딩이 메시지에 적용되었는지 수신자에게 알려준다.

TE: 어떤 전송 인코딩을 사용할 수 있는지 서버에게 알려주기 위해 요청 헤더에 사용한다.

</div>
</details>
<br>

