# 2주차 내용 퀴즈

## 3장 : HTTP 메시지

### 3.2 메시지의 각 부분

#### 1. HTTP 메세지의 본문과 헤더는 둘 다 비워둘 수 있다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

X
본문은 비어있을 수 있지만 헤더의 집합은 반드시 빈 줄(CRLF)로 끝나야한다.

</div>
</details>

<br>

### 3.3 메서드

#### 2. 안전한 메서드(Safe Method)가 무엇인지 설명하고 그 종류를 두가지 나열하세요.

<details>
<summary>답안</summary>
<div markdown="1">

안전한 메서드란 서버측의 상태 정보를 변경하지 않는 메소드를 말하며 GET, HEAD가 있다.

</div>
</details>

 <br>

#### 3. 다음 중 멱등한 메서드를 모두 고르시오.

`GET` `POST` `DELETE`

<details>
<summary>답안</summary>
<div markdown="1">

GET, DELETE
POST는 여러번 호출시 각기 다른 결과가 리턴될 수 있으므로 멱등하지 않다.

</div>
</details>
