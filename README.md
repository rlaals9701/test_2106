# HTML CSS JS 기초

## HTML

> HTML:Hyper Text Markup Language
> 
> 웹 페이지의 구조를 표시
> 
> 웹페이지의 콘텐츠를 표시
> 
### hHTML Elements

> Element : 요소 - 의미적
>
> Teg : 태그 - 기술적

> 문법(Syntax)
> 
> <>로 감싸줌
> 
> 소문자 사용
>
> 시작태그<>와 종료태그</>set 구성
```
<tegname>contents</tagname>
```
>
> 예외) 시작태그만 존재하는 경우 : 빈 요소(empty element)

> 포함관계(nested)
```
<body>
  <div>
    text
  </div>
</body>
```

### HTML Attribute

> HTML 속성
> HTML 요소의 부가 정보
> 속성name(이름) = "속성value(값)"

```
<a href="http://www.naver.com">naver</a>
```

### 제목태그

> heading -> h
>
> h1~h6
>
>h1이 가장 큰 제목

### HTML 기본구조

```
<!DOCTYPE html> -1
<html> -2
  <head> -3
    <meta charset="utf-8"> -4
    <title>My test page</title> - 5
  </head>
  <body> -6
    <p>This is my page</p>
  </body>
</html>
```

1. 웹 문서의 버전 : HTML5
2. HTML 문서의 가장 바깥쪽 요소
3. 웹 문서를 설명하는 정보가 담기는 영역 요소
4. 웹 문서의 정보 표시 요소
5. 웸 문서의 제목을 표시 요소(타이틀 태그영역)
6. 웹 문서의 콘텐츠 요소들이 담기는 영역 요소

### 단락 태그

> p(paragraph) : 단락을 표시
> 단락과 단락사이를 구분하는 수평선
```
<hr> - horizontal rule
```
> 단락을 구분하지 않고 줄 바꿈
```
<br> - break(뜻)
```
### 목록 태그

> 순서없는 목록 ul(unordered list) >>숫자 생기는거 싫으면 css에서 수정가능
> 순서있는 목록 ol(Ordered List)
> 목록 항목 li (List Item)

```
<ul>
  <li>html</li>
  <li>html</li>
</ul>
  
 <ol>
  <li>html</li>
  <li>html</li>
</ol> 
```
> 포함관계(nested)로 구성된 목록 - 코딩할때 밖에서 안쪽으로방향 순서로
-HTML
  -HTML4
  -HTML5
-css
  -css2
  -css3
  ```
  <ul>
    <li>
      html
      <ul>
        <li>html4</li>
        <li>html5</li>
      </ul>
    </li>
    <li>
      css
      <ul>
        <li>css2</li>
        <li>css3</li>
      </ul>
    </li>
  </ul>
  ```

> 설명목록(descriptin List) - dl

```
<dl>
  <dt>html</dt> (dt: description title)
  <dd>표준 마크업 언어</dd> (dd: description data)
</dl>
```

> 하이퍼링크 a(anchor)
> 
> attribute(속성) : href(hypertext reference)>> 어디로 이동할지 : 연결되는 웹 문서의 url
```
<a href="http://www.naver.com">네이버로 이동</a>
```
> 북마크 기능
> 외부페이지 연결이 아닌 같은 페이지에서 특정위치로 이동하는 기능
> 
> 도착지점에 id attribute 를 사용하여 이름 지정
```
<a href="#t1"></a>
...
<h2 id="t1">넣고싶은 위치</h2>
```

### table element
>기본 사용 태그 : table, thead, tbody , tr, td, th
>
>열제목 : therd(table head) th(table heading)
>
>표 내용 :tbody,td(table data)
>
>행 : tr (table row) 아랫줄 
>
https://www.tablesgenerator.com/html_tables





