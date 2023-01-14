# 내용 공유

# 관련 자료

# 2주차 내용 퀴즈

## 3장 : HTTP 메소드

#### 1. 'HTTP/1.0 200 NOT OK'와 'HTTP/1.0 200 OK'는 사유 구절이 다르므로 다르게 처리된다

<details>
<summary>답안</summary>
<div markdown="1">

X

`사유구절` 은 오로지 사람에게 읽히기 위한 목적으로만 존재한다. 그러므로 사유구절이 달라도 상태코드가 같아면 동등하게 처리되어야한다.

</div>
</details>

<br>


#### 2. 안전한 메서드란 HTTP 요청의 결과로 서버에 어떤 작용도 없음을 의미하며, 이에 해당하는 메서드는 GET, POST 이다.

<details>
<summary>답안</summary>
<div markdown="1">

X

(p.61) GET, HEAD 메서드는 HTTP 요청의 결과로 서버에 어떠한 작용도 없으므로 안전한 메서드이다.

</div>
</details>


#### 3. DELETE 는 서버에세 요청 URL 로 지정한 리소스를 삭제할 것을 요청하며, 삭제가 수행되는 것을 보장한다.

<details>
<summary>답안</summary>
<div markdown="1">

X

(p.66) 클라이언트는 삭제가 수행되는 것을 보장받지 못한다. 왜냐하면 HTTP 명세는 서버가 클라이언트에게 알리지않고 요청을 무시하는 것을 허용하기 때문이다.

</div>
</details>


## 4장 : 커넥션 관리

#### 4. TCP 커넥션은 네가지 값으로 식별하는데, 이에는 <발신지 IP주소, 발신지 포트, 수신지 IP주소, 수신지 포트> 이며, 이 네가지 주소 구성 요소의 값이 모두 같을 수는 없다.

<details>
<summary>답안</summary>
<div markdown="1">

O

(p.89)

</div>
</details>


#### 

<details>
<summary>답안</summary>
<div markdown="1">

</div>
</details>