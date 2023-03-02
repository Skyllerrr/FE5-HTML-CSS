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

**약 60자를 넘지 않아야 한다.**

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

**[주의 사항] HTML 페이지 내에 id는 유일해야 한다!**

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

**px 단위만 사용하면 안되나요?**
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

**왜 em, rem 같은 단위를 쓰는 건가요?**
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