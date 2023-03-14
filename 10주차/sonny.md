# 10주차 내용 퀴즈

## 17장 : 내용 협상과 트랜스코딩

### Q) 트랜스코딩은 무엇인가요? 종류에는 어떤것들이 있나요?

<details>
<summary>답안</summary>
<div markdown="1">
트랜스코딩은 클라이언트의 요구에 맞는 리소스가 없을 때 비슷한 리소스를 변환한뒤 클라이언트에게 응답하는 방법입니다.
세 가지 종류가 있습니다.
- 포맷 변환
- 정보 합성
- 콘텐츠 주입

</div>
</details>

<br>


### Q) 클라이언트 주도 협상의 과정을 얘기해주시고 단점을 알려주세요.

<details>
<summary>답안</summary>
<div markdown="1">

1. 클라이언트는 응답 가능한 리소스의 목록을 서버에 요청한다.
2. 클라이언트는 리소스의 목록을 응답받고 그 중 가장 알맞는 리소스를 선택한 뒤 서버에 요청한다.

두 번의 요청을 해야하며 이로 인해 네트워크 비용이 증가한다. 그리고 여러 URL을 요구한다는 점이 단점이다.

</div>
</details>

<br>



### Q) 클라이언트는 자신의 원하는 리소스에 대한 정보를 자세히 담은 후 서버에게 요청합니다. 서버 주도 요청에 필요한 내용 협상 헤더 필드들은 무엇이 있을까요?
<details>
<summary>답안</summary>
<div markdown="1">
Accept
Accept-Language
Accept-Charset
Accept-Encoding

그 외 내용 협상 헤더가 아닌 필드
User-Agent

</div>
</details>

<br>

