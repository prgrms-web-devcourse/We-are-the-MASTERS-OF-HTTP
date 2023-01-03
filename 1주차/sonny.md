# 1주차 내용 퀴즈

## 2장 : URL과 리소스

#### 1. https://www.naver.com 의 스킴은 http, 호스트는 www.naver.com, 포트는 80이다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

X

HTTPS의 기본 포트값은 433이다.
</div>
</details>

<br>


#### 2. 서로 다른 URL은 같은 리소스를 가리킬 수 없다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

X. 같은 리소스를 가리킬 수 있다. hostname이 동일한 ip주소를 가리키는 경우 (dns)

ex)
http://text.com:80/index.html
http://152.12.123.43:80/index.html

</div>
</details>

 <br>



#### 3. 안전하지 않은 문자를 안전한 문자로 인코딩하는 것을 "이스케이프"라고 한다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

O

</div>
</details>


#### 4. 몇몇 문자는 URL에서 특수한 문자로 예약되어 있다. 이러한 이스케이프되야하는 문자 예시 2가지를 얘기해주세요.

<details>
<summary>답안</summary>
<div markdown="1">

`/` : 경로를 나눌때
`#` : 프래그먼트를 지정할 때
`?` : 쿼리를 지정할 때
등등

</div>



#### 5. 다음 URL과 동일한 Origin을 찾아주세요.
http://www.text.com/other.html

  1. https://www.text.com/other.html
  2. http://www.text.com:81/other.html
  3. http://www.something.com:80/other.html
  4. http://www.text.com/another.html


<details>
<summary>답안</summary>
<div markdown="1">

4번

1번은 스킴(프로토콜)이 다르다.
2번은 포트번호가 다르다
3번은 호스트가 다르다.
4번은 스킴, 호스트, 포트번호가 같다.

</div>
