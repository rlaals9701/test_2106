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




