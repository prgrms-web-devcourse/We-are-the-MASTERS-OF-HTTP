# 5주차 내용 퀴즈

## 9장 : 웹 로봇

### 9.2 로봇의 HTTP

#### 1. 로봇 구현자들은 잘못된 크롤러의 소유자를 찾아내거나 서버에게 로봇이 어떤 종류의 컨텐츠를 다룰 수 있는지에 대한 정보를 주기위해 사이트에 신원 식별 헤더를 전송하는 것이 좋다. 다음 보기에서 골라 빈칸을 채우세요.

> **보기**
>
> `User-Agent` `From` `Accept` `Referer`

a. `_________` 로봇의 사용자/관리자의 이메일 주소를 제공한다.

b. `_________` 현재의 요청 URL을 포함한 문서의 URL을 제공한다.

c. `_________` 서버에게 어떤 미디어 타입을 보내도 되는지 말해준다.

d. `_________` 서버에게 요청을 만든 로봇의 이름을 말해준다.

<details>
<summary>답안</summary>
<div markdown="1">

(a): From

(b): Referer

(c): Accept

(d): User-Agent

</div>
</details>

<br>

#### 2. 하나의 호스트와 포트에는 여러개의 robot.txt가 있을 수 있다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

X
한 호스트의 포트당 한개의 robot.txt가 있다.

</div>
</details>

 <br>

## 10장 : HTTP/2.0

### 10.2 개요

#### 3. HTTP/2.0에서 모든 메시지는 `_______`에 담겨 전송된다.

<details>
<summary>답안</summary>
<div markdown="1">

프레임

</div>
</details>

 <br>

#### 4. HTTP/2에서는 `_______` 압축 형식을 사용하여 요청 및 응답 헤더 메타 데이터를 압축합니다.

 <details>
<summary>답안</summary>
<div markdown="1">

HPACK

</div>
</details>

 <br>
