# 9주차 내용 퀴즈

## 16장 : 국제화

### Q) Content-Language 헤더는 어떤 언어의 사용자를 대상으로 하는지 나타낸다. (O/X)

```
Content-Language: fr
```

<details>
<summary>답안</summary>
<div markdown="1">
A) O

- 프랑스어 사용자를 대상으로 하는 문서(콘텐츠)

</div>
</details>

<br>


### Q) 다음 Content-Language 헤더 필드를 가진 문서(Document)는 영어로 작성되었다. (O/X)
```
Content-Language: en-US
```

<details>
<summary>답안</summary>
<div markdown="1">
A) X

Content-Language 필드는 `어떤 언어의 사용자`를 대상으로 하는지 나타낸다. 문서가 작성된 언어와는 상관이 없다.
- 초급자를 위한 영어 문법 페이지는 한국어를 사용하는 사용자를 위한것이기 때문에 `Content-Language: ko`를 가져야한다.


</div>
</details>

<br>



### Q) 데이터 비트는 디코딩되어 문자코드가 된다. 코딩된 문자집합에서 문자코드에 대응하는 문자를 찾아서 문자를 만들어낸다. (O/X)

<details>
<summary>답안</summary>
<div markdown="1">

- 표준화된 MIME charset 태그를 Content-Type, Accept-Charset 헤더에 사용한다.
- MIME charset 태그를 통해 인코딩 구조를 파악하고, 이를 통해 데이터 비트를 디코딩하여 문자코드를 만든다.
- 코딩된 문자집합에서 문자코드에 대응하는 문자를 찾아서 문자를 만들어낸다.
- 코딩된 문자집합의 예로는 US-ASCII가 있다.
  - 코드값으로 0~127을 사용한다.(7비트로 표현가능)


</div>
</details>

<br>
