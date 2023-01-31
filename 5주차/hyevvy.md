# 내용 공유

# 관련 자료

# 5주차 내용 퀴즈

## 9장 : 웹 로봇

#### 1.

<details>
<summary>답안</summary>
<div markdown="1">

(p.164)

</div>
</details>

####

<details>
<summary>답안</summary>
<div markdown="1">

</div>
</details>

## 10장 : HTTP/2.0

#### 1. HTTP/1.1의 메시지 포맷은 구현의 단순성과 접근성에 주안점을 두고 최적화되었다. 그러다보니 성능이 어느정도 희생되었고, 응답을 받아야만 그 다음 요청을 보낼 수 있기 때문에 심각한 회전지연을 피할 수 없었다. 이 문제를 회피하기 위해 도입한 두 가지는?

<details>
<summary>답안</summary>
<div markdown="1">

(p.287) 병렬 커넥션 , 파이프라인
그러나 이는 근본적인 해결책은 되지 못 했다.

</div>
</details>

<br>

#### 2. HTTP/2.0 은 서버와 클라이언트 사이의 `____` 위에서 동작한다. 이 때 이를 초기화하는 것은 `(서버 / 클라이언트)` 다

<details>
<summary>답안</summary>
<div markdown="1">

(p.288)

TCP 커넥션, 클라이언트

</div>
</details>

#### 3. 한 개의 스트림은 하나 이상의 요청과 응답을 처리할 수 있다.

<details>
<summary>답안</summary>
<div markdown="1">

(p.288)
X, 오로지 한 쌍의 요청과 응답만을 처리할 수 있다.
단, 하나의 커넥션 위에서 여러 개의 스트림이 동시에 만들어질 수 있으므로, 여러 개의 요청과 응답을 동시에 처리하는 것 역시 가능하다.

</div>
</details>

#### 4. HTTP/2.0은 무조건 HTTP 메시지의 헤더를 압축하여 전송한다. 이 때, 헤더를 받은 수신 측은 헤더를 쓰지 않고 버리는 경우라면 성능 개선을 위해 압축해제를 수행할 필요가 없다. ( O / X )

<details>
<summary>답안</summary>
<div markdown="1">

(p.292)
X, 헤더를 받은 수신측은 반드시 압축 해제를 수행해야한다. 만약 그럴 수 없다면 반드시 COMPRESSION_ERROR 와 함께 커넥션을 끊어야한다.

</div>
</details>
