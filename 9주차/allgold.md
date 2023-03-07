# 9주차 내용 퀴즈 

## 16장 : 국제화 

### 1. `ISO-8859`, `UTF-8`, `ISO 2022-JP`의 인코딩 방식의 차이점

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

- ISO-8859 : 고정폭 인코딩 사용

- UTF-8 : 가변폭 인코딩 사용 (비모달)

- ISO 2022-JP : 가변폭 인코딩 사용 (모달)

</div>
</details>

---

### 2. 서버에서 클라이언트로 엔터티 본문의 문자를 설명하기 위하여 HTTP 헤더에 `_______(1)________`  과 `_______(2)________` 를 사용하고, 클라이언트는 서버에게 자신이 사용할 수 있는 차셋 알고리즘과 언어를 설명하기 위하여 `_______(3)_____`과 `_____(4)____`를 사용한다.

부연 설명
3. 클라이언트가 받아들일 수 있는 문자집합을 표현함
4. 클라이언트가 선호하는 언어를 표현함
<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

1. Content-Type charset 매개 변수
2. Content-Language
3. Accept-Charset
4. Accept Language 

</div>
</details>

---

### 3. HTTP의 메타 태그중 `_______________`을 사용하여 클라이언트가 서버에서 수신한 HTML의 문자집합을 추측할 수 있다.

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

`<META HTTP-EQUIV="Content-Type">`

</div>
</details>


---

### 4. OX 퀴즈

1. 글리프 하나를 다른 것으로 바꾸었을 때 텍스트의 의미가 바뀐다면, 두 글리프들은 서로 다른 글자다. `(O / X)`
2. 현재 표준으로 사용되는 문자 인코딩 방식의 인코딩 구조는 가변폭 비모달 방식이다. `( O / X )`

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

1. `O`,  글리프 : 하나의 글자를 표현하기 위한, 획의 패턴이나 다른 것과 구분되는 유일한 시각적 형태. 하나의 글자를 여러 방식으로 쓰는 것이 가능하다면 글리프를 여러 개 가질 수 있다.
2. `O` , 현재 표준으로 사용되는 문자 인코딩 구조는 `UTF-8` 방식이며, 이는 가변폭 비모달 방식의 인코딩 구조를 사용한다.

</div>
</details>

---

### 5. JavaScript에서 URI 의 특정 문자를 이스케이프 문자로 변환하는 함수는?

<details>
<summary>퀴즈 답안</summary>
<div markdown="1">

- `encodeURI()` : URI에서 특별한 뜻을 가진 문자(예약 문자)는 인코딩 하지 않습니다. (encodeURI() 혼자서는 XMLHttpRequest 등이 사용할, 적합한 HTTP GET과 POST 요청을 구성할 수 없습니다)
- `encodeURIComponent()` : encodeURIComponent()를 사용해, 서버에 POST로 요청할 양식 필드를 인코딩 하세요. 입력 중 의도치 않게 생성될 수 있는 HTML 특수 개체 등의 "&" 문자를 처리할 수 있습니다.


> encodeURI() 혼자서는 XMLHttpRequest 등이 사용할, 적합한 HTTP GET과 POST 요청을 구성할 수 없습니다. GET과 POST에서 특별한 문자로 취급하는 "&", "+", "="를 인코딩 하지 않기 때문입니다. 그러나 encodeURIComponent()는 저 세 문자도 인코딩 대상에 포함합니다.

참고 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/encodeURI


</div>
</details>