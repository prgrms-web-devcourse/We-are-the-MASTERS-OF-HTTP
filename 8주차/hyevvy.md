# 내용 공유

# 관련 자료

# 8주차 내용 퀴즈

## 15장 : 엔터티와 인코딩

#### 1. 엔터티 본문은 헤더 필드의 끝을 의미하는 빈 `_____` 줄 바로 다음부터 시작하며, 콘텐츠가 텍스트든 바이너리든 항상 `_____` 바로 다음에 위치한다. (O / X)

<details>
<summary>답안</summary>
<div markdown="1">
(p.396) CRLF , O

</div>
</details>

#### 2. 다음은 엔터티 헤더 필드 중 하나인 **Content-Length**에 대한 설명이다.

1. Content-Length 가 잘못된 값을 담더라도 아예 빠진 경우보다 피해를 덜 유발하므로, 무조건 적어야하는 필드이다. (O / X)

2. Content-Length는 지속 커넥션을 위해 필수인데, 청크 인코딩을 사용할 때는 Content-Length 헤더 없이 사용할 수 있다. (O / X)

3. 본문의 콘텐츠가 인코딩되어 있다면, Content-Length헤더는 인코딩되지 않은 원본의 길이가 아닌 인코딩된 본문의 길이를 바이트 단위로 정의한다. (O / X)
4. <details>
   <summary>답안</summary>
   <div markdown="1">
   (p.398)
5. X
6. O
7. O

</div>
</details>

#### 3. HTTP와 HTTPS의 계층적인 측면에 대해 가장 큰 차이점을 설명해주세요.

<details>
<summary>답안</summary>
<div markdown="1">
- (p.357) HTTPS는 HTTP 하부에 전송 레벨 암호 보안 계층을 제공한다.
이 보안 계층은 안전 소켓 계층 혹은 그를 계승한 전송 계층 보안을 이용하며 구현되는데, 이 둘을 표현하는 용어로 SSL을 사용한다.

</div>
</details>
