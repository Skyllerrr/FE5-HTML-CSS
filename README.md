# HTML/CSS

## HTML
## 태그 (Tag)
---
<br>
기본적으로 <> 시작 태그(여는 태그) </> 종료 태그(닫는 태그)의 쌍으로 구성되어있다.

<br></br>
## 요소의 포함
---
<br>

```html
<p>
	HTML은 요소 안에 
	<strong>다른 요소</strong>가 들어갈 수 있습니다
</p>

<!-- 잘못 사용된 예 -->
<p>
	HTML은 요소 안에 
	<strong>다른 요소 가 들어갈 수 있습니다
</p>
	</strong>
```
"주석"은 프로그램 동작에 영향을 미치지 않으며, 최소한으로 남기는 것이 좋다!

<br></br>
## !DOCTYPE html
---
<br>
"이 문서는 html Living Standard 문서!"라는 의미이다.
해당 코드를 통해 어떤 모드로 페이지를 랜더링할지 결정하며, 작성 시 완전 표준 모드로 랜더링을 한다.

<br></br>
## html
---
<br>
HTML 문서의 루트, 최상단 요소이다. <br>
lang 속성을 통해 해당 페이지의 주 언어가 무엇인지 설멍할 수 있으며, 한국은 ko로 설정한다.

<br></br>
## head
---
<br>
검색엔진을 위한 다양한 정보들이 담기는 곳이다. <br> 사용자에게는 title과 파비콘, viewport 정보등이 보이게 된다.

<br></br>
## meta
---
<br>
메타 데이터 : "어떤 목적을 위해 만들어진 데이터"

<br></br>
## charset
---
<br>

```html
<meta charset="utf-8">
```
문자 깨짐 오류가 발생할 수 있으므로 문자 코드의 종류를 설정해 준다. <br>
"utf-8"은 전 세계적인 언어들을 지원하도록 한다. 그래서 어떤 언어로 작성하더라도 웹페이지를 읽을 수 있다. (국제적인 코드 규약)

<br></br>
## viewport
---
<br>

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
width : 뷰포트의 너비를 제어한다. width=600과 같이 픽셀값으로 지정할 수도 있다.

height : 뷰포트의 높이를 제어한다.

initial-scale : 페이지가 처음 로드 될 때 확대 및 축소 수준을 제어한다. 최소 0.1, 기본 1, 최대 10

minimum-scale : 축소 정도를 제어한다.

maximum-scale : 페이지에 허용되는 확대 정도를 제어한다. 3보다 작은 값은 접근성에 맞지 않다.

<br></br>
## title
---
<br>
브라우저의 제목 표시줄이나 페이지 탭에 보이는 문서 제목을 정의한다. 텍스트만 가능 (특수 문자 X)
<br>
<br>

**<u>약 60자를 넘지 않아야 한다.</u>**

<br></br>
## link
---
<br>

```html
<html>
<head>
  <!-- 스타일 시트 링크 -->
  <link rel="stylesheet" href="style.css">
  
	<!-- 폰트 링크 -->
  <link rel="stylesheet" href="font.ttf">
  
	<!-- 파비콘 링크 -->
  <link rel="shortcut icon" href="favicon.ico"> 
</head>
<body>
</body>
</html>
```
현재 문서와 외부 리소스의 관계를 명시한다. <br>
외부 스타일 시트, 폰트, 파비콘을 연결할 때 사용한다.
빈 태그, 속성만을 포함한다.

<br>
head : 요소 내부에만 위치할 수 있다.
<br>
rel : relations 관계. 대상 파일의 속성을 나타낸다.
<br>
href : hyper-references 경로, 연결 시 참조할 파일의 위치를 나타낸다.

<br></br>
## body
---
<br>
body 태그는 사용자에게 보이는 영역이다.
<br>
본격적으로 우리가 작성할 영역!

<br></br>
## h1, h2, h3, h4, h5, h6
---
<br>
Heading : 제목
<br>
웹 페이지가 하나의 책이라고 생각한다면, 제목 태그는 목차와 같다.
<br>
<br>

***주의! h1 태그는 한 페이지에 한 번만 사용을 권장한다!***
<br>
<br>
h1, h2, h3를 크기 순서로 즉, 스타일의 목적으로 사용하지 말고 h1을 먼저쓰면 다음은 h2와 같이 형식 순서대로 써야한다.

<br></br>
## a
---
<br>
href : hypertext reference
<br>
<br>
target 속성값
<br>
_self : 현재 페이지(기본값)
<br>
_blank : 새 탭
<br>
_parent : 부모 페이지, 부모가 존재하지 않으면 _self와 동일
<br>
_top : 최상위 페이지

<br></br>
## p
---
<br>
paragraph의 약어로 하나의 문단을 나타낸다.
<br>
블록 요소이다.

<br></br>
## br
---
<br>
break(line break)의 약어로 줄을 나눈다는 뜻이다.
<br>
<br>

**여백을 위해 <p></p> 내용이 없는 p태그를 사용하거나, <br> 태그를 여러 번 사용하지 마라! 여백은 CSS를 사용하여 적용하자!**

<br></br>
## strong
---
<br>
중대하거나 긴급한 콘텐츠를 나타낸다.
<br>
기본적으로 굵은 글꼴이 적용되며 웬만하면 자주 쓰지말자 [최후의 수단...]

<br></br>
## em
---
<br>
Emphasis : 강조
<br>

**텍스트의 강세**를 나타낸다. 콘텐츠를 강조해서 읽었으면 하는 부분에서 적용된다.

<br></br>
## i
---
<br>
기본적으로 기울임 꼴이 적용된다.

<br></br>
## q
---
<br>
줄바꿈이 없는 짧은 인용문을 나타낼 때 사용한다.

<br></br>
## blockquote
---
<br>
긴 인용문을 나타낸다.

<br></br>
## address
---
<br>
물리적 주소, URL, 이메일 주소, 전화번호 등 해당 콘텐츠에 대한 연락처 정보를 나타낸다.

<br></br>
## mark
---
<br>
하이라이트 텍스트를 정의할 때 사용하며, 형광펜으로 칠한 것처럼 표시된다.

<br>
<br>
<br>
<br>
<br>

## CSS
## CSS란?
---
<br>
CSS는 Cascading Style Sheets의 약자로 스타일을 적용할 때 사용한다.

<br></br>
## 인라인 방식
---
<br>
태그 자체에 style 속성으로 스타일을 주는 방식이다.
<br>
하지만, 가상 요소 (:hover, ::before, ::after)등에 스타일을 줄 수 없어 사용에 제한이 있다.

<br>

```html
<p style="color:yellow; background-color:black;">Hello wold</p>
```

<br></br>
## 내부 스타일
---
<br>
head 태그 안 style 태그를 사용하여 스타일을 주는 방식이다.

<br>

```html
<!DOCTYPE html>
<html lang="ko-KR">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	<title>내부 스타일</title>
	<style>
		p {
				color:yellow; 
				background-color:black;
		}
	</style>
</head>
<body>
	<p>Hello world</p>
</body>
</html>
```
하지만, 코드가 길어질수록 HTML 파일 길이가 길어지기 때문에 효율적이지 않다.

<br></br>
## 외부 스타일
---
<br>
link를 사용하여 현재 문서와 외부 리소스의 관계를 명시하며, 빈 태그로 속성만을 포함한다.

<br>
head : 요소 내부에만 위치할 수 있다.
<br>
rel : relations 관계, 대상 파일의 속성을 나타낸다. <br>
(css 파일은 stylesheet)
<br>
href : hyper-references 경로, 연결 시 참조할 파일의 위치를 나타낸다.

<br>

```html
<!-- index.html -->
<!DOCTYPE html>
<html lang="ko-KR">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	<title>외부 스타일</title>
	<link rel="stylesheet" href="style.css">
</head>
<body>
	<p>Hello world</p>
</body>
</html>
```
```css
/* style.css */
p {
		color:yellow; 
		background-color:black;
}
```
해당 방법을 가장 권장한다.
<br>
HTML과 CSS를 분리하면 코드의 가독성과 효율성이 모두 높아지기 때문이다!

<br></br>

# CSS 선택자
## 전체 선택자
---
<br>
* (별표, 애스터리스크) 로 나타내며, head를 포함한 HTML 문서 내의 모든 요소를 선택한다.

<br>

```css
* {
	margin:0;
	padding:0;
}
```

<br>
</br>

## 타입 선택자 (태그, 요소)
---
<br>
특정 태그를 선택한다.

<br>

```css
h1 {
	font-weight:bold;
}
p{
	font-size: 24px;
}
```

<br>
</br>

## 아이디 선택자 (#)
---
<br>

**<u>[주의 사항] HTML 페이지 내에 id는 유일해야 한다!</u>**

HTML안에서 한 번만 사용되기 때문에 재사용성은 떨어진다.

<br>

```html
<header id="header">
...
</header>
```

```css
#header {
	padding: 10px;
}
```

<br>
</br>

## 클래스 선택자 (.)
---
<br>

클래스 선택자는 아이디 선택자와 다르게 한 페이지에 여러 개가 존재할 수 있다.
<br>
재사용성이 높다.

<br>

```html
<h1 class="fc-red">hello wolrd</h1>
<p>Lorem ipsum dolor sit amt</p>
<p class="fc-red">Lorem ipsum dolor sit amt</p>
```

```css
.fc-red {
	color: red;
}
```

**id, class는 숫자로 시작하면 안 된다!
<br> 하이픈(-)과 언더바(_) 문자로만 시작할 수 있다.
<br> 숫자 또는 하이픈 뒤에 숫자로 시작할 수 없다.**

<br>
</br>

## 그룹 선택자 (,)
---
<br>
<br>

```css
h1 {font-weight:bold;}
h2 {font-weight:bold;}
h3 {font-weight:bold;}
h4 {font-weight:bold;}
h5 {font-weight:bold;}
h6 {font-weight:bold;}
```

```css
h1, h2, h3, h4, h5, h6{ font-weight:bold}
```

<br>
</br>

## 자손 선택자 ()
---
<br>

자식, 자손 모두 선택할 수 있다.
<br>
공백, 띄어쓰기를 통해 구분하자!

<br>

```css
section p{
  font-weight:bold;
}
```

<br>
</br>

## 자식 선택자 (>)
---
<br>

```css
section > p{
  color:royalblue;
}
```

<br>
</br>

## 일반 형제 선택자 (~)
---
<br>

```css
h1 ~ p{
  text-decoration:underline;
}
```

<br>
</br>

## 인접 형제 선택자 (+)
---
<br>

```css
h1 + p{
  background:yellow;
}
```

<br></br>

# CSS 상속
## 상속(Inheritance)
---
<br>

CSS에는 상속되는 속성이 있고, 상속되지 않는 속성이 있다.
<br>
앞에 본 section의 color 속성은 자식인 h1, h2, p에게 상속이 된다.
<br>
하지만, width, height, margin, padding, border와 같은 것은 상속되지 않는다.

```html
<section>
	<h1>Hello</h1>
	<h2>Hello</h2>
	<p>Hello</p>
</section>
```

```css
section {
	color: red;
	border: 5px solid pink;
}
```
에서 inherit 속성을 사용하여 부모와 동일하게 상속 받게하여 속성값을 같게 할 수 있다.

```css
section {
	color: red;	
	border: 5px solid pink;
}
h1 { border: inherit; }
```
와 같이 예시를 들 수 있다.

<br></br>

# 단위
## px
---
<br>

디바이스 화면에서 이미지를 표현하는 가장 작은 단위

<br>

**<u>px 단위만 사용하면 안되나요?</u>**
<br>

다양한 디바이스 생겨나며 픽셀 밀도도 다양해졌다.
<br>
따라서, 다양한 단위들을 사용하기도 한다.

<br>
</br>

## %
---
<br>

부모 요소를 기준으로 하는 백분율 단위이다.

<br>
</br>

## vw, vh
---
<br>

뷰포트(화면) 넓이(w), 높이(h)를 기준으로 하는 백분율 단위이다.
<br>

1vw = 화면의 1%

<br>
</br>

## vmin, vmax
---
<br>

화면의 넓이와 높이 중 작은 값(min), 큰 값(max)을 기준으로 하는 백분율 단위이다.

<br>
</br>

## em
---
<br>

부모요소로부터 상속받은 요소의 글자 크기를 기준으로 하는 배수 단위이다.

<br></br>

# 텍스트 꾸미기
## color 색상
---
<br>

폰트의 색상을 나타낸다.
<br>

키워드(red, blue), 16진수 표기법, rgb(), rgba()등 다양한 방법으로 표기할 수 있다.

```html
<div>
    <p>안녕하세요</p>
</div>
```
```css
div {	color: sandybrown;}
p {	
	border: 1px solid currentColor;
}
```
부모에 color 값이 있다면 상속으로 처리된다.

<br>
</br>

## font-family 글꼴 종류
---
<br>

```css
p {
    font-family: 'Pretendard-Regular', Verdana, sans-serif;
}
```

<br>
</br>

## 폰트 적용 방법
---
<br>

link로 삽입
```html
<!-- 사용예시1 : href 참고 -->
<head>
		<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300&display=swap" rel="stylesheet">
    <style> 
				body {font-family: 'Noto Sans KR', sans-serif;}
		</style>
</head>
```

import로 삽입
```css
/*사용예시2 : url 참고 */
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300&display=swap");

body{
	font-family: "Noto Sans KR", sans-serif;
}
```

<br>
</br>

## font-size 글꼴 크기
---
<br>

px : 절대 단위
<br>
em : 현재 요소의 부모 요소에 설정된 글꼴 크기 상대 단위
<br>
rem : 루트요소(html)에 설정된 글꼴 크기 상대 단위

<br>

**<u>왜 em, rem 같은 단위를 쓰는 건가요?</u>**
<br>

em, rem 단위는 반응형 웹페이지 개발, 유지보수 등에 용이하다!

<br>
</br>

## font-weight
---
<br>

텍스트 굵기 설정
<br>

normal : 기본
<br>
bold : 굵게
<br>
lighter : 현재 요소의 굵기를 부모 요소 굵기 보다 한 단계 가볍게
<br>
border : 현재 요소의 굵기를 부모 요소 굵기 보다 한 단계 두껍게

<br>
</br>

## text-transform
---
<br>

uppercase : 모든 텍스트를 대문자로
<br>
lowercase : 모든 텍스트를 소문자로
<br>
capitalize : 모든 단어의 첫글자를 대문자로

```css
p::first-letter{
	text-transform: uppercase;	
}
```

<br>
</br>

## text-decoration (단축 속성)
---
<br>

color, line, style, thickness 순서

<br>

underline : 밑줄
<br>
overline : 윗줄
<br>
line-through : 취소선
<br>

style : solid, wavy, dashed

```css
.dashed {
  text-decoration: lime underline overline dashed auto;
}

.wavy{
	text-decoration-color: royalblue;
  text-decoration-line: line-through underline overline;
  text-decoration-style: wavy;
	text-decoration-thickness:5px;
}
```

<br>
</br>

## text-shadow
---
<br>

텍스트에 그림자를 추가한다.
<br>

offset-x, offset-y, blur-radius, color
<br>
```css
text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
```

<br>
</br>

## text-align
---
<br>

left : 왼쪽 정렬
<br>
right : 오른쪽 정렬
<br>
center : 중앙 정렬
<br>
justify : 양쪽 정렬

<br>
</br>

## vertical-align
---
<br>

텍스트의 세로 정렬을 설정한다.
<br>

**<u>인라인, 인라인 블록 및 테이블 셀 요소에만 적용된다</u>**
<br>

**<u>블록 레벨에서 수직 정렬을 하고 싶으면 flex를 사용하자!</u>**
```css
.block { 
	display:flex;
  	align-items: center;
}
```

<br>
</br>

## line-height
---
<br>

행간을 설정하며, 단위나 배수 및 % 등의 값으로 설정한다.

<br>
</br>

## letter-spacing
---
<br>

자간을 설정한다.

<br>
</br>

## word-spacing
---
<br>

단어와 단어 사이의 간격을 설정한다.

<br>
</br>

## word-break
---
<br>

텍스트가 자신의 콘텐츠 박스 밖으로 넘칠 경우 <br> 줄바꿈 여부를 지정한다.

<br>

normal : 기본 줄 바꿈 규칙을 사용한다.
<br>
break-all : 글 넘침을 방지하기 위해서 어떠한 두 문자 사이에서도 줄바꿈이 발생할 수 있다.

<br>
</br>

## font (단축 속성)
---
<br>

font : font-style, font-variant, font-weight, <br> font-stretch, font-size / line-height, font-family

```css
p {
	font: italic normal bold normal 3em/1.5 Helvetica, Arial, sans-serif;
}
```

<br></br>

# CSS 선택자 <br> (가상 클래스 / 가상 요소)
## 가상 클래스 선택자
---
<br>

<br>
</br>

## :first-child
---
<br>
형제 요소 그룹 중 첫 번째 요소

<br>
</br>

## :last-child
---
<br>
형제 요소 그룹 중 마지막 요소

<br>
</br>

## :nth-child
---
<br>
형제 사이에서의 순서에 따라 요소를 선택한다.

<br>

```css
/* 2번째 li */
li:nth-child(2) {
  color: lime;
}
/* 홀수번째 li */
li:nth-child(odd) {
  color: lime;
}

/* 짝수번째 li */
li:nth-child(even) {
  color: lime;
}
/* 2n+1번째 li */
li:nth-child(2n+1) {
  color: lime;
}
```

<br>
</br>

## :nth-of-type
---
<br>
형제 그룹 안에서 위치를 기반으로 형제 요소 선택

<br>
</br>

## :only-of-type
---
<br>
동일한 유형의 형제가 없는 형제 요소 중 유일하게 사용된 태그

<br>
</br>

## :not
---
<br>
부정 선택자이다.

<br>

```css
/* li 중 첫번째가 아닌 li */
li:not(:first-child){
	margin-top:20px;
}
```

<br>
</br>

## 가상 요소 (::)
---
<br>
선택자에 추가하는 키워드이다.
<br>
특정 요소의 일부분에만 스타일을 입힐 수 있다.

<br>
</br>

## ::after과 ::before
---
<br>
선택한 요소에 자식을 생성한다.
<br>
보통 content 속성과 짝을 지어 요소에 장식용 콘텐츠를 추가할 때 사용한다.

<br>
빈 태그 img, br, input 에는 적용할 수 없다.

<br>
</br>

## ::placeholder
---
<br>
자리 표시자이며, input과 textarea 요소에 정보를 <br>제공한다.

<br></br>

# CSS 선택자 우선 순위
## 후자 우선의 원칙
---
<br>
동일한 선택자에 동일한 속성이 사용되었을 경우 뒤에 적힌 속성을 따른다.

<br>

```html
<p>선택자 우선순위</p>
```
```css
p {color: red; font-size:20px;}
p {color: blue;}
```
color 속성이 동일하기 때문에, 결과는 blue 색으로 <br> 적용이 된다.

<br>
</br>

## 우선 순위 계산
---
<br>
inline-style : 1000점
<br>
id 선택자 "#" : 100점
<br>
class ".", 가상 클래스, 속성 선택자 : 10점
<br>
타입, 가상요소 선택자 : 1점
<br>
전체 선택자 "*" : 0점

<br>
예시를 들어보자!

```html
<div>
  <p id="id" class="class">
		1. 이 글자는 어떤 색일까요?
	</p>
  <p id="id" class="class" style="color:red">
		2. 이 글자는 어떤 색일까요??
	</p>
</div>
```
```css
div #id{
  color:green;
}
p{
  color:black;
}
#id{
  color:blue;
}
.class{
  color:yellow;
}
```
여기서 1번 문장은 #id, .class와 같이 단독으로 쓰이는 것보다 유형 선택자와 아이디 선택자가 함께 쓰인 <br> div #id처럼 더 구체적으로 작성된 선택자 속성이 <br> 적용되어 "초록색"으로 적용이 된다.

2번 문장은 inline-style 속성이 적용되어 "빨간색"으로 적용이 된다.

<br>
</br>

## 중요성의 원칙 (!important)
---
<br>
이 선언은 다른 CSS의 어떤 선언 보다도 우선된다.

<br>

**<u>하지만, CSS의 자연스러운 상속을 깨뜨리기 때문에 오류 및 버그 발생 시 수정을 어렵게 만들어서 important의 사용은 좋지 못한 습관이다!</u>**

<br>
</br>

# 블록 레벨 요소 vs 인라인 레벨 요소
## block
---
<br>
부모 요소의 전체 공간을 차지하여 블록을 만든다.

<br>
언제나 새로운 줄에서 시작, 좌 우 양측으로 최대한 <br> 늘어나 가능한 모든 너비를 차지한다.

<br>
앞 뒤 요소 사이에 새로운 줄을 만들고, 이전 이후 <br> 요소 사이에 줄 바꿈이 일어난다.

<br>
블록 요소는 인라인 요소안에 중첩 될 수 없지만, <br> 인라인 요소는 블록 요소 안에 중첩 될 수 있다.

**<u>a 태그 안에는 블록 요소 중첩 가능!</u>**

<br>
width, height 크기를 지정할 수 있으며 <br> padding, border, margin 속성을 사용할 수 있다.

<br>
div, p, li, nav, footer 등이 있다.

<br>
</br>

## inline
---
<br>
항상 블록 레벨 요소 내에 포함된다.

<br>
컨텐츠의 흐름을 끊지 않으며, 컨텐츠에 따라 할당된 공간만 차지한다.

<br>
문장, 단어 같은 작은 부분에 대해서 적용된다.

<br>
새로운 줄을 만들지 않는다.

<br>
width, height 크기를 지정할 수 없으며 <br> padding, border, margin 속성을 사용할 수 있지만, <br> 상하 margin 속성은 사용할 수 없다.

<br>
span, a, em, strong 등이 있다.

<br>
</br>

# CSS Box Model
## 기본 요소
---
<br>
CSS Box Model은 HTML 요소를 감싸는 상자로, <br> 요소, 패딩, 테두리, 마진으로 구성되어 있다.

<br>
요소 : 텍스트, 사진 등 보여줄 대상이다.
<br>
패딩 : 요소 주변 영역을 감싼다.
<br>
테두리 : 요소와 패딩을 감싸는 테두리이다.
<br>
마진 : 테두리 밖의 영역을 감싼다.

<br>
</br>

## width
---
<br>
요소의 너비를 설정한다.

<br>
기본 값은 컨텐츠 영역의 너비이지만, <br> box-sizing 속성을 사용하여 테두리 영역의 너비를 설정한다.

<br>
auto : 기본값으로 브라우저가 계산하여 지정  <br> (요소의 부모 크기 기준으로 가득 채우기)

<br>
min-content : 최소 너비
<br>
max-content : 컨텐츠 내용의 선호 너비

<br>
</br>

## height
---
<br>
요소의 높이를 설정한다.

<br>
auto : 기본값으로 브라우저가 계산하여 지정  <br> (요소의 자식 기준으로 조절)

<br>
</br>

## padding
---
<br>
단축 속성이다.

<br>
4가지를 모두 설정할 경우에는 padding-top, padding-right, padding-bottom, padding-left 순으로 작성한다.

```css
p{
	padding: 10px; /* top, right, bottom, left 모두 10px */
	padding: 10px 20px; /* top, bottom :10px,  left, right:20px */
	padding: 10px 20px 30px; /* top:10px, left,right:20px, bottom:30px */
	padding: 10px 20px 30px 40px;
}
```

<br>
</br>

## margin
---
<br>
단축 속성이다.

<br>
4가지를 모두 설정할 경우에는 margin-top, <br> margin-right, margin-bottom, margin-left 순으로 <br> 작성한다.

<br>
가운데 배치

```css
p{
	width: 400px;
	margin: auto; 
}
```
오른쪽 배치

```css
p{
	width: 400px;
	margin: auto 0 auto auto;
}
```

**<u>margin auto는 수평 정렬을 할 수 있지만, <br> 세로 정렬을 적용할 수는 없다!</u>**

<br>
</br>

## 마진 병합 현상 (Margin Collapsing)
---
<br>
요소와 요소 사이에 마진 탑(margin-top) 혹은 <br> 마진 바텀(margin-bottom)의 공간이 있을 경우 더 높은 값의 마진 값이 적용되는 현상

<br>
부모 요소와 자식 요소가 존재할 때, <br> 자식 요소의 마진 탑 혹은 마진 바텀 값이 부모의 높이에 영향을 미치지 않는 현상

<br>

**<u>마진 병합 현상 해결방법</u>**

1. 부모 요소에 overflow 속성 값을 적용해준다.
2. 부모 요소에 display: inline-block 값을 <br> 적용해준다.
3. 부모 요소에 border 값을 적용해준다.

<br>
</br>

## border
---
<br>
테두리를 지정한다.

<br>
테두리는 요소가 차지하는 전체 너비, 높이의 일부이다.

<br>
선의 두께, 스타일, 색상을 지정할 수 있다.

<br>
</br>

## box-sizing
---
<br>
content-box : 기본값.width, height에 border과 padding을 포함하지 않는다.

<br>
border-box : width, height에 border과 padding을 포함한다.
<br>
[예를 들어, width = 컨텐츠 너비 + border + padding]

<br>
</br>

## overflow, overflow-x, overflow-y
---
<br>
박스보다 컨텐츠가 더 커서 컨텐츠가 넘칠 경우, <br> 어떻게 처리할지를 지정한다.

<br>
visible : 기본값, 박스를 넘는 컨텐츠를 자르지 않는다.
hidden : 요소의 크기만큼 맞추기 위해 잘라낸다. <br> [스크롤바를 제공하지 않는다.]

scroll : 요소의 크기만큼 잘라낸다. <br> [스크롤을 제공한다.]

<br>
</br>

## border-radius
---
<br>
상자의 모서리를 둥글게 처리한다.

<br>
</br>

## background
---
<br>
background-attachment

<br>
1. fixed : 뷰포트에 고정
<br>
2. local : 요소 컨텐츠에 대해 고정, 스크롤이 존재하면 배경은 컨텐츠와 함께 스크롤이 된다.
<br>
3. scroll : 배경 요소 자체에 대해 고정, 스크롤이 존재해도 배경은 함께 스크롤 되지 않는다.

<br>

background-color : 배경 색상 설정
<br> 
background-image : 배경 이미지 설정
<br> 
background-position : 배경 위치 설정

<br>
background-repeat : 배경 이미지를 어떻게 반복할 것인지 설정한다.

<br>
1. repeat : 반복
<br>
2. no-repeat : 반복하지 않음
<br>
3. repeat-x : x축으로만 반복
<br>
4. repeat-y : y축으로만 반복

<br>
background-size

<br>
contain : 이미지가 잘리거나 찌그러지지 않는 한도 내에서 제일 크게 설정한다. <br> [다만, 여백 발생 가능]

<br>
cover : 이미지가 찌그러지지 않는 한도 내에서 제일 크게 설정한다. <br>
이미지의 가로세로비가 요소와 다르다면, <br> 이미지를 세로 방향 또는 가로 방향으로 잘라내어 <br> 여백이 생기지 않도록 설정합니다.

```css
div{
	...생략
	background-size: 100%;
	background-size: 100px 400px;
}
```
<br>

**<u>웹페이지에 이미지를 넣는 방법에는 주로 img 태그나 CSS background 속성을 사용한다. <br> 하지만, 가급적이면 img 태그를 사용하자!</u>**

<br>
</br>

## box-shadow
---
<br>
그림자 효과를 추가한다.

<br>
offset-x, offset-y, blur-radius, spread-radius, color <br> 등이 있다.

<br>
</br>

## opacity
---
<br>
불투명도를 설정한다.

<br>
0 ~ 1 사이의 숫자를 지정할 수 있다. <br> (0: 투명, -1 : 불투명)

<br>
</br>

## display 속성
---
<br>
block : 요소 전후에 줄 바꿈을 생성한다.

<br>
inline : 요소 전후에 줄 바꿈을 생성하지 않는 인라인 요소 상자를 생성하며, 정상적인 흐름에서 공간이 <br> 있으면 다음 요소는 같은 줄에 있다.

<br>
inline-block : inline 줄 바꿈 없이 한 줄에 놓이지만, block처럼 box-model의 width, height, margin, padding 값을 모두 설정할 수 있다.

<br>
flex : 내부 자식 요소들의 위치를 부모 컨테이너 요소 안에서 x, y축 단방향(1차원적)으로 설정한다.

<br>
grid : 내부 자식 요소들의 위치를 부모 컨테이너 요소 안에서 x, y축 모두 이용해(2차원적) 설정한다.

<br>
none : 해당 속성은 접근성 트리에서 해당 요소가 <br> 제거된다. 이렇게 되면 해당 요소 및 해당 하위 요소가 사라지고, 스크린리더에도 읽히지 않는다.

<br>
</br>

# 이미지 img
## img
---
<br>
문서에 이미지를 삽입한다.

<br>
src : 경로
<br>
alt : 대체 텍스트, 이미지에 대한 설명

<br>

**<u>주의 사항! 이미지 하단에 빈 공간이 생긴다면?</u>**
<br>
해당 현상은 img가 **인라인 요소**라서 발생하는 현상

인라인 요소이기 때문에 img의 세로 정렬이 글자의 baseline을 따르게 된다.

따라서, 해당 현상을 해결하기 위해서는 아래와 같은 초기값을 넣어주면 된다.
```css
img{
	vertical-align:top;
}
```

<br>
</br>

# 이미지 비율 유지하기
## 방법1) aspect-ratio
---
<br>
기본 가로와 세로 비율을 설정한다.

```css
img{
  width:300px;
  aspect-ratio: 2 / 1;
  object-fit:cover;
}
```

<br>
</br>

## 방법2) padding %값 이용하기
---
<br>

padding의 top과 bottom % 값은 부모의 세로가 아닌, **가로 너비** 기준으로 한다.

```html
<div class="thumbnail">
  <img src="https://github.com/stronger-deer/myBlog/blob/main/img/main-visual.jpg?raw=true"
       alt="한 성인이 스케이트보드를 타고 있다" />
</div>
```

```css
.thumbnail {
  position: relative;
  height: 0;
  padding-top: 50%; 
  overflow: hidden;
}

.thumbnail  img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

<br>
</br>

# position
## static
---
<br>
기본값이며, 의미는 변화 움직임이 없이 고정되고 정적인 상태이다.

<br>
</br>

## relative
---
<br>
비교 상의, 상대적인의 의미를 가진다.

<br>
자신이 있어야 하는 위치에 상대적이며, 다른 컨텐츠들의 위치에 영향을 미치지 않는다.

<br>
</br>

## absolute
---
<br>

**조상의 위치**를 기준으로 자리를 잡는다.

<br>
static을 제외한 position 속성값을 가진 가장 가까운 조상이다.

<br>
</br>

## fixed
---
<br>
브라우저 화면(뷰포트)을 기준으로 위치를 저장한다.

<br>

**<u>단, 요소의 조상 중 하나가 transform, perspective, filter 속성 중 어느 하나라도 none이 아니라면 뷰포트 대신 그 조상을 컨테이닝 블록으로 삼는다.</u>**

일반적인 문서 흐름에서 자신의 요소를 제거하고 자리를 잡으며, 스크롤을 내리거나 올리거나 해도 <br> 화면의 같은 위치에 고정되어 있다.

header, 하단 top 버튼에 사용한다.

<br>
</br>

## z-index
---
<br>

position이 static 외의 값을 가진 박스에 대해 <br> z축의 위치를 지정한다.

<br>
값이 클 수록 제일 위로 배치된다.

<br>
부모가 z-index를 높여 자식 앞으로 나올 수 없다.

<br>
자식은 z-index를 음수값으로 주어 부모 뒤로 갈 수 있다.

<br>
유지보수를 위해 100단위로 작업하면 좋다.

<br>
</br>

# Sections
## header
---
<br>
소개 및 탐색에 도움을 준다.

<br>
회사명, 제목, 로고, 검색 폼, 작성자 이름 등의 요소가 포함된다.

<br>
</br>

## nav
---
<br>
문서의 부분 중 현재 페이지 내, 또는 다른 페이지로의 링크를 보여준다.

<br>
메뉴, 목차, 브레드크럼(breadcrumb)으로 사용된다.

<br>
메뉴

```html
<nav>
	<ul>
		<li><a href="#">위니브</a></li>
		<li><a href="#">About</a></li>
		<li><a href="#">Contact</a></li>
	</ul>
</nav>
```
브레드크럼
```html
<nav>
	<ol>
		<li><a href="#">위니브</a></li>
		<li><a href="#">캐릭터소개</a></li>
		<li>라이캣</li>
	</ol>
</nav>
```
문서의 모든 링크가 nav 안에 있을 필요는 없으며, <br> 페이지의 주요 탐색 링크를 위한 태그이다.

하나는 사이트 전체 탐색, 다른 하나는 현재 페이지 내 탐색으로 사용하는 등, 하나의 웹페이지에 여러 개의 nav 태그를 가질 수 있다.

<br>
</br>

## footer
---
<br>
페이지의 작성자, 저작권 정보, 관련 문서 등의 내용을 담는다.

<br>
</br>

## main
---
<br>
body의 주요 컨텐츠를 나타낸다.

<br>
웹페이지에서 한 번만 사용할 수 있다.

<br>
사이드 바, 탐색 링크, 저작권 정보, 사이트 로고, 검색 폼 등 여러 페이지에 반복되는 컨텐츠를 포함해서는 <br> 안된다.

<br>

**<u>검색 폼이 주요 기능이라면 예외!</u>**

<br>
</br>

## article
---
<br>
독립적으로 구분해 배포하거나 재사용할 수 있는 구획을 나타낸다.

<br>

<li>사이트의 다른 기능에 영향을 주지 않고, 독립적인 기능을 수행한다.
</li>

<li>
article 영역을 제거해도 페이지는 정상적으로 돌아간다.
</li>

<br>
article이 대표적으로 사용되는 곳은 뉴스 홈페이지이다.

<br>

<li>다양한 기사들이 한 페이지에 담겨 있지만, <br> 이 기사들은 각각 독립적으로 사용된다. 
</li>

<li>
시간마다 노출되는 기사가 달라져도 홈페이지는 정상적으로 운영된다.
</li>

<br>
게시판, 블로그 글, 매거진, 뉴스 기사, 위젯, 등 <br> 사용된다.

<br>

**<u>제목 요소를 자식으로 포함해야 한다!</u>**

<br>
</br>

## article
---
<br>
제목 요소를 자식으로 포함해야 한다.

<br>

```
article vs section

일단 article 사용을 우선 고민해보자.

독립적으로 사용한다면 article 사용하고,
웹페이지의 앞뒤 문맥이 연결성이 필요하거나, 더 적합한 의미를 가진 요소가 없을 때 section을 사용하자.

단순 스타일링이 목적이라면 div 요소를     사용하자.
```

<br>
</br>

## aside
---
<br>
문서의 주요 내용과 간접적으로 연관된 부분을 <br> 나타낸다.

<br>
문서의 주요 흐름을 따라가지 않고, 보조적인 역할만 <br> 하는 공간이다.

<br>
각주, 광고 배너등에 사용한다.

<br>
</br>

# 스타일링을 위해서만 사용하는 태그!
## div
---
<br>
division 영역 나눔, 컨텐츠 분할 요소이다.

<br>
블록 컨테이너이며, 영역을 구분 짓거나 무리를 짓는 <br> 태그로 상당히 광범위하게 사용된다.

<br>
공간을 나누는 것 외에 별다른 기능은 없다.

<br>
정리를 도와주는 역할 뿐이지만 HTML에 가장 큰 도움을 주며 많이 사용된다.

<br>
</br>

## span
---
<br>
인라인 컨테이너이며, 본질적으로 아무것도 나타내지 않고 스타일을 적용하거나 인라인 요소를 묶을 때 사용한다.

<br>
</br>

# float
## float이란?
---
<br>
한 요소가 보통 흐름으로부터 빠져 텍스트 및 인라인 <br> 요소가 그 주위를 감싸 해당 요소에 좌, 우측에 배치되게 한다.

<br>
left : 왼쪽으로
<br>
right : 오른쪽으로
<br>
none : 기본값

<br>
</br>

## float 해제하기
---
<br>
clear

<br>

```css
.box {
	clear:both;
}
```

**<u>주의 사항</u>**
<br>

자식 요소들이 모두 float 속성을 가지게 되면, <br> 컨테이너 요소의 높이에 자식 요소들의 높이가 포함되지 않는 것에 주의해야 한다.

<br>

**<u>해결 방법</u>**

<br>
<li>부모에게 높이 값을 지정해준다.</li>
<br>
<li>overflow-hidden</li>

```css
.container{
	overflow:hidden;
}
```


<li>clear-fix 방법</li>
부모의 가상 요소 ::after를 사용하는 방법이다.

```css
.container::after{
  content:'';
  display:block;
  clear:left;
}
```

<br>
</br>

# flex
## flex-container에 사용하는 속성
---
<br>
display : flex;

<br>
자식 요소들이 컨테이너 안 공간을 맞추기 위해서 크기를 키우거나 줄이는 방법을 설정하는 방법이다.

<br>
부모 요소를 flex-container, 자식 요소를 flex-item 이라고 부른다.

<br>
1차원적 레이아웃(x축 혹은 y축)을 위해 주로 사용한다.

![image](https://user-images.githubusercontent.com/93968241/223656320-fc5e2916-33b8-4109-8193-6cbe5aeea949.png)

<br>
</br>

## flex-direction
---
<br>
컨테이너 내 아이템을 배치할 때, 주축 및 방향을 지정한다.

<br>
row : 기본 값, 왼쪽에서 오른쪽 (주 축이 행 방향)
<br>
column : 위에서 아래 방향 (주 축이 열 방향)
<br>
row-reverse : 오른쪽에서 왼쪽
<br>
column-reverse : 아래에서 위 방향

<br>
</br>

## justify-content
---
<br>
주 축을 기준으로 배열의 위치를 조절하거나 아이템 간의 설정을 할 수 있다.

<br>
flex-start, flex-end, center, space-between, <br> space-around, space-evenly

<br>

**flex 실습 1 -> 2023.03.08.teach의 001.html**

**flex 실습 2 -> 2023.03.08.teach의 002.html**

**flex 실습 3-> 2023.03.08.teach의 003.html**

<br>
</br>

## align-items, align-content
---
<br>
align-items : 교차 축을 기준으로 정렬한다.

<br>
align-content : 컨테이너의 교차 축의 <br> 아이템들이 여러 줄일때, 사용 가능하다.
[이 속성은 flex-wrap: wrap인 상태에서 사용해야 한다.]

<br>
</br>

## gap
---
<br>
아이템 사이의 간격을 설정할 때, 사용할 수 있는 <br> 속성이다.

<br>
</br>

## flex-basis
---
<br>
flex-item의 초기 크기를 설정한다.

<br>
width, height와 다른 점은 축의 방향에 따라 달라진다는 것과 내부 컨텐츠에 따라 유연한 크기를 가진다는 <br> 것이다.

<br>
auto : 기본 값

<br>
flex-basis 값이 적용되어 있다면, row일 경우 width 값이 무시, column일 경우 height 값이 무시된다.

<br>

**<u>기본적으로 px이나 em 등의 단위 값을 사용하며, 0외에 다른 상숫값을 사용할 수 없다.</u>**

<br>
</br>

## flex-grow
---
<br>
아이템이 컨테이너 내부에서 할당할 수 있는 공간의 정도를 지정한다.

<br>
형제 요소인 아이템들이 모두 같은 flex-grow 값을 가지면, 내부에서 동일한 공간을 할당 받는다.

<br>
값을 0을 줄 경우 늘어나지 않는다.

<br>
</br>

## flex-shrink
---
<br>
아이템의 크기를 고정하거나 축소할 때 사용한다.

<br>
값을 0을 줄 경우 줄어들지 않는다.

<br>
</br>

## flex
---
<br>
단축 속성이다.

<br>
flex-grow, flex-shrink, flex-basis 순이다.

```css
flex: 1 1 100px;
```

<br>
</br>

# grid
## grid란?
---
<br>
display: grid;

<br>
자식 요소들이 컨테이너 안에 공간을 맞추기 위해서 <br> 크기를 키우거나 줄이는 방법을 설정한다.

<br>
부모 요소를 grid-container, 자식 요소를 grid-item 이라고 부른다.

<br>
그리드 레이아웃은 웹페이지를 위한 2차원 레이아웃 <br> (x축, y축) 시스템이다.

![image](https://user-images.githubusercontent.com/93968241/223665269-a6f17438-3530-4e5f-8745-c1abea371c26.png)

<br>
</br>

# grid-container에 사용하는 속성
## grid-template-columns
---
<br>
열 방향 그리드 트랙의 사이즈를 설정한다.

<br>
</br>

## grid-template-rows
---
<br>
행 방향 그리드 트랙의 사이즈를 설정한다.

```html
<div class="container"></div>
```

```css
.container{
	display:grid;
	width:300px;
	height:300px;
	grid-template-columns: 100px 100px 100px;
	grid-template-rows: 200px 100px;
}
```

```css
.container{
	display:grid;
	width:300px;
	height:300px;
	grid-template-columns: 1fr 1fr 1fr;
	grid-template-rows: 2fr 1fr;
}
```

![image](https://user-images.githubusercontent.com/93968241/223732680-06901722-1db6-4484-bea9-2fd9f97e2863.png)


**빈 화면에 그리드 라인이 생기는 것을 볼 수 있다.**

<br>

**<u>새로운 단위 fr</u>**
- fraction: 분수
- 컨테이너를 분할해준다. 
- grid 컨테이너 안에서 트랙의 비율을 지정해주는 유연한 길이 단위이다.
- 1fr 1fr 1fr은  1:1:1 의 비율을 의미한다.**

**flex 실습 1 -> 2023.03.08.teach의 005.html**

<br>
</br>

## repeat()
---
<br>
row 혹은 column 방향으로 grid-track의 사이즈를 좀 더 간단한 형태로 표현하도록 도와주는 CSS함수이다.

<br>

함수에 전달하는 첫 번째 인자는 <br> **반복 횟수(repeat count)**, 두 번째 인자는 **반복할 값**이다.

```css
.container {
    display: grid;
    width: 300px;
    height: 300px;
    /* grid-template-columns: 1fr 1fr 1fr; */
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 2fr 1fr;
  }
```

```css
/* grid-template-columns: 1fr 2fr 1fr 2fr; */
grid-template-columns: repeat(2, 1fr 2fr);
```

<br>
</br>

## minmax()
---
<br>
그리드에서 최소와 최대 사이의 범위를 설정하는 함수이며, 최소와 최대값을 의미하는 두 가지 인자를 가진다.

<br>
min 보다 크거나 같고, max 보다 작거나 같은 크기 <br> 범위를 정의한다.

<br>
</br>

## auto-fill & auto-fit
---
<br>
만약 repeat 함수를 사용할 때, 반복되는 카운트를 <br> 고정하지 않고 컨테이너의 넓이에 따라 가능한 많은 <br> 그리드 컬럼을 배치하고 싶다면 사용하는 키워드 값이다.

<br>
auto-fill : 가능한 많은 셀들을 만들어 낼려고 하며, <br> 빈 공간이 생긴다.

<br>
auto-fit : 그리드 컨테이너 내부에 공간이 남을 경우, <br> 그 공간을 각 셀들이 나눠 갖는다.

<br>
</br>

## gap
---
<br>
셀과 셀사이의 간격을 설정할 때 사용 할 수 있는 <br> 속성이고, 복잡한 레이아웃 안에서 마진 대신 편리하게 간격을 설정할 수 있으며, grid-gap은 gap으로 <br> 사용할 수 있습니다.

```css
gap : 10px 20px;
```

<br>
</br>

## align-items
---
<br>
직계 자식에 대한 수직(열) 정렬을 모두 동일하게 준다.

<br>
stretch, center, start, end

<br>
</br>

## justify-items
---
<br>
직계 자식에 대한 수평(열) 정렬을 모두 동일하게 준다.

<br>
stretch, center, start, end

<br>
</br>

# grid-itemr에 사용하는 속성
## grid-area
(grid-column-start, <br> grid-column-end, grid-row-start, grid-row-end)
---
<br>

```css
grid-row-start: 1; /* 1 */
grid-row-end: 2; /* 3 */
grid-column-start: 1; /* 2 */
grid-column-end: 4; /* 4 */


grid-row: 1/2;
grid-column: 1/4;


grid-area: 1/1/2/4;

grid-area: 1/1/1/span 3; 
```

<br>

**grid-template-areas / grid-area**


```css
.container{
	grid-template-areas: 
		"header header header"
		"section section aside"
		"footer footer footer"
}

header{
	grid-area:header;
}
```

<br>
</br>

## z-index
---
<br>
z-index 속성을 grid 안에서도 사용할 수 있으며, <br> grid 안에서는 굳이 position 속성을 사용하지 않더라도 화면에 보여지는 우선순위를 설정할 수 있다.

<br>
</br>

## align-self
---
<br>
아이템 개별로 수직(열) 정렬을 지정한다.

<br>
stretch, center, start, end

<br>
</br>

## justify-self
---
<br>
아이템 개별로 수평(핼) 정렬을 지정한다.

<br>
stretch, center, start, end

<br>
</br>

## place-self
---
<br>
align-self, justify-self 를 함께 적는 단축 속성이다.

```css
/* 수직: 중앙, 수평 : 끝(오른쪽) */
place-self: center end;
```

<br>
</br>

## grid
---
<br>
단축 속성이다.

<br>
grid-template-rows, grid-template-columns, <br> grid-template-areas, grid-auto-rows, <br> grid-auto-columns, grid-auto-flow

<br>

```css
grid: auto-flow / 1fr 1fr 1fr;

grid: auto-flow dense / 40px 40px 1fr;
```

**grid 실습 2 -> 2023.03.08.teach의 007.html**

