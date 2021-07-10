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
### HTML 페이지에서 표시하는 콘텐츠

- 텍스트 콘텐츠

- 멀티미디어 콘텐츠 (임베디드embedded 콘텐츠)
  - 이미지
  - 비디오
  - 오디오

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

### image element
> tag : img
> 
> attribute : src(image 위치, 파일명), alt(대체 텍스트)


` : backtick
```
<img src="imge.jpg" alt="대체 텍스트"> 
```

### video element
> 비디오 및 오디오 콘텐츠는 용량이 크기 때문에 서버에 저장해 콘텐츠를 제공하면 많은 트래픽이 발생할 수 있음
>
> 트래픽 과부하를 해결하기 위해 유튜브 서비스를 사용하기도 함
>
>attribute
>
>controls : 컨트롤 버튼 표시
>
>autoplay : wkehdwotod(* muted와 같이 사용해야 함)
>
>muted : 음소거
>
>loop : 반복재생
```
<video width="900" height="400" controls autoplay muted loop>
  <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
</video>
```

### youtube

>비디오 콘텐츠 제공시 서버의 트래픽과부하를 해결할 수 있는 방법중 하나
>
>매개변수
>
>comtrols=1(켬),0(끔)
>
>autoplay=1,0 (뮤트와 함께 사용)
>
>mute=1,0
>
>loop=1,0 (플레이리스트와 같이 사용)

> 텍스트는 html문서에 직접 입력되는 콘텐츠
> 
> 이미지와 동영상, 오디오 콘텐츠는 외부에서 만들어지는 콘텐츠
> 
> 이미지, 동영상, 오디오는 직접 입력하는 것이 아니고 외부파일을 삽입=>임베드(embed) 콘텐츠

### 웹사이트 템플릿 디자인 사이트
https://freebiesbug.com/psd-freebies/website-template/

### container element (단순 영역 구분 요소)

>div(division)
>
>span

### Block, Inline

> 모든 element는 각각의 고유영역을 가지고있음
> 
> block element, Inline Element구분은 이들 영역 화면 표시 박식에 따른 구분
>
> block element는 줄바꿈 되어 표시 - block element영역의 가로 너비가 부모요소에 100%채우짐
> (** 포함하는 요소 : 부모요소, 포함되는 요소 : 자식요소)
> 
> inline element는 같은 줄에 나란히 표시 - inline element영역의 가로 너비가 콘텐츠 크기만큼만 정해짐
>
> inline element는 위,아래 여백을 적용할 수 없음
>

###parent element(부모요소), child element(자식요소)

>포함관계에서 포함하는 요소가 부모요소, 포함되는 요소는 자식요소
>
>직계 포함관계에서만 부모요소, 자식요소
>
>직계가 아닌 포함관계에서는 조상요소(ancestor),자손요소(decendant)

## CSS

### CSS 기본 개념

>선택자는 스타일을 지정할 HTML 요소를 가리 킵니다.
>
>선언 블록에는 세미콜론으로 구분 된 하나 이상의 선언이 포함됩니다.
>
>각 선언에는 콜론으로 구분 된 CSS 속성(PROPERTY) 이름과 값(VALUE)이 포함됩니다.
>
>여러 CSS 선언은 세미콜론으로 구분하고 선언 블록은 중괄호로 묶습니다.

### id,class

>html element에 특정 이름을 사용할 때 id, class attribute를 사용해서 이름을 붙여줄수 ㅇ
>
>id는 동일한 이름이 사용된 html element가 여러개이면 논리적 오류가 발생
>
>id는 html 문서 내에서 고유해야함
>
>class는 동일한 이름이 여러개의 element에 사용되어서 공통 디자인 요소나 공통 기능을 적용ㅇ
>
>id는 주로 서버에서 불러오는 데이터를 표시하는 위치에 고유하게 사용>백엔드 개발시 사용
>
>class는 주로css스타일 적용, javascript 인터렉션 적용시 사용>프론트엔드개발시 주로 사용
>
>id는 하나의 html element에 대해서 하나의 이름만 존재, html 문서내에서 고유해야함.
>
>class는 하나의 html element에 대해서 여러개의 이름을 지정할 수 있고, html 문서내에서 여러곳에서 공통 사용 가능

### css작성방법

>external css : 파일분리
>
>internal css : 같은 html 문서내에 <head> 태그 영역에 <style>태그를 사용하여 입력
>
>inline css : 시작태그에 style attribute를 사용해서 입력> javascript에서 css제어시 사용

###naming할 때 표기방식

>id, class naming, 변수/ 함수 / 클래스 namine, 파일/폴더 naming의 경우 가독성을 높이기 위해 사용
>표기방식을 사용하는 이유
> -naming할때 두단어 이상으로 구성되는 경우 단어와 단어 사이를 구분하기 위해 사용
> -단어의 시작부분에 첫글자를 대문자로 변경, 특수기호를 사용
>표기방식 종류  
>snake case : gnb_depth1  뱀방식> 파일/폴더
>kebab case : gnb-depth1  하이픈으로 연속연결> ID/CLASS
>camel case : gnbDepth1  낙타>JAVASCRIPT의 변수/함수
>pascal case : GnbDepth1 >javascript의 클래스
>

### oocss(object oriented css)

> html element를 대상화시키는 과정에서 element하나하나를 모두 객체화 시키는 이론
>
> html element 모두 각각 id,class attibute를 사용해서 이름을 지정해줌
>
  
  
