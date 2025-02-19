2022.10.17
# HTML
> Hyper Text Markup Language

# Emmet
* HTML 표준 구조 !
> ! 입력 후 Tab키 : 간단하고 빠르게 HTML 기본구조를 만들어 준다.

* 자식노드 >
> div>ul>li 입력 후 Tab키 : >를 사용하여 자식 요소를 생성할 수 있다.

* 형제노드 +
> div>ul+ol+div 입력 후 Tab키 : +를 사용하여 한 요소와 같은 단계에 위치한 요소를 생성할 수 있다.

* 반복하기 *
> div>ul>li*3 입력 후 Tab키 : *를 사용하여 요소를 반복해서 생성할 수 있다.

* 클래스부여 .
> div.title 입력 후 Tab키 : CSS 클래스를 갖을 요소를 생성할 수 있다. (기본이 div 이기 때문에 생략가능)

* 아이디 #
> #item 입력 후 Tab키 : id를 갖는 요소를 생성할 수 있다. (기본이 div 이기 때문에 생략가능)

* 자동 넘버링 부여 $
> p.container{item$}*5 입력 후 Tab키 : $를 사용하여 넘버링을 부여합니다.


2022.10.18
# HTML 기본태그
### 글꼴 태그
- `<h1>` ~ `<h6>` Headine / 제목
- `<p>` Paragraph / 문단표시
- `<hr>` Horizontal Rule / 가로로 선 긋기
- `<br>` Break / 개행
- `<i>` `<em>` *이텔릭체로 강조*할 때 사용
- `<b>` `<strong>` Bold **진하게 표시**할 때

### 목록 태그
- `<ol>` Ordered List / **순서가 있는 목록**
- `<ul>` Unordered Lists / **순서가 없는 목록**
- `<li>` Listed Item 목록하위 항목으로 사용, `<ul>`태그 또는 `<ol>`태그의 하위에 위치한다.
- `<dl>` Definition List / **사전처럼 용어를 설명하는 목록**
- `<dt>` Definition Term / **정의되는 용어의 제목**
- `<dd>` Definition Description / **용어를 설명**

### 표 태그
- `<table>` 표를 만드는 태그
- `<caption>` 표의 제목
- `<tr>` 표의 행을 의미하는 태그(자식으로 `<th>`태그나 `<td>`태그가 반드시 있어야 함)
- `<th>` 표의 **제목 열**을 의미
- `<td>`  표의 **일반 열**을 의미
### Table 그룹 관련 태그
- `<colgroup>` 열을 그룹으로 묶을 수 있도록 해주는 태그
- `<col>` 
 `<colgroup>`태그의 자식으로 열 단위를 나눌 수 있다.
  `span` 속성을 사용하여 열을 그룹으로 묶을지 설정. 예) <col span="3"> → 세 개의 열을 그룹으로 묶음
- `<thead>` 표의 제목 열들을 묶는 그룹 태그
- `<tbody>` 표의 일반적인 데이터들을 묶는 그룹태그
- `<tfoot>` 표의 하단 영역을 묶는 그룹태그
    
### Semantic tag
### HTML Sementic Elements

- `<header>` : 페이지에 대한 정보를 담는 태그로, 페이지 상단에 위치
- `<nav>` : 다른 페이지나 같은 페이지 안에 다른 부분으로 이어주는 네비게이션 링크로 구성된 섹션을 표현
- `<aside>` : 주요 내용과는 직접적인 연관성은 없는 분리된 내용
- `<main>` : 주 콘텐츠(main content)를 정의할 때 사용합니다.
- `<section>` : 일반적인 섹션을 표현합니다.
- `<article>` : 여러가지 아이템들을 묶어 재사용 가능하게 그룹화
- `<footer>` : 주로 저작권 정보나 서비스 제공자 정보등을 나타냄, 사이트 하단에 위치
- `<details>` : 추가적인 정보를 나타내거나 사용자가 요청하는 정보를 나타냄
- `<summary>` : 부모요소인 details요소의 내용에 대한 요약
- `<figure>` : 일러스트, 다이어그램, 사진, 코드등에 주석을 다는 용도
- `<figcaption>` : 부모요소인 figure요소의 내용들에 대한 캡션, 혹은 제목
- `<mark>` : 하나의 문서 내에서 다른 문맥과의 관련성을 나타내기 위해서 참조 목적으로 마킹되거나 하이라이트된 텍스트를 표현합니다.
- `<time>` : 24시간에서의 시간 혹은 그레고리력에서의 정밀한 날짜

22.10.28
# Inline VS  Block Element


## Block Element


블록 레벨 요소는 부모 요소의 **전체 공간**을 차지하여 "블록"을 만듭니다. `<h1>~<h6>` `<ol>` `<ul>` `<li>` `<p>` 태그 등이 블록 요소에 속한다.

- 화면 구성이나 레이아웃을 짤 때는 블록 레벨 요소를 사용합니다.
- 블록 레벨 요소는 한칸을 모두 차지하기 때문에 **세로**로 나열 됩니다.
- width, height, margin 속성이 적용됨.
- css에서 가로 세로 지정 가능 (width, height)
- 대표적인 태그 : `<div>`

## Inline Element


인라인 레벨 요소는 콘텐츠의 흐름을 끊지 않고(줄바꿈X), 요소를 구성하는 **태그에 할당된 공간만 차지**합니다. `<a>` `<em>` `<img>` `<span>` 태그 등이 인라인 요소에 속한다.

- 인라인 레벨 요소는 콘텐츠 영역 만큼 차지하기 때문에 **가로**로 나열된다.
- margin-top, margin-bottom 적용되지 않습니다. 대신에 line-height 이용
- width, height 속성이 적용되지 않는다
- 태그가 콘텐츠의 할당 된 공간만 갖고 있기 때문에 text-align과 같은 속성은 사용할 수 없다.
- css에서 가로 세로 지정 불가
- 대표적인 태그 : `<span>`

# 이미지 & 멀티미디어

## 이미지 태그

`<img>` 태그는 HTML 문서에 이미지를 넣음

```css
<img src="images/apple.jpg" alt="사과">
```
- `src`
    
    **필수**이며, 이미지로의 경로를 지정
    
- `alt`
    
    이미지의 텍스트 설명이며 필수는 아니지만, 스크린 리더가 `alt`의 값을 읽어 사용자에게 이미지를 설명하므로, 웹 접근성 차원에서 **매우 유용**하다. 또한 네트워크 오류, 콘텐츠 차단, 죽은 링크 등 이미지를 표시할 수 없는 경우에도 이 속성의 값을 대신 보여줌
    
- `height`
    
    픽셀 단위의 이미지의 고유 크기. 단위 없는 정수여야 함
    
- `width`
    
    이미지의 픽셀 기준 고유 너비. 단위 없는 정수여야 함

## 절대경로 vs 상대경로

### 절대경로리
웹 이미지 절대경로 예) - http://www.naver.com/apple.png
http 프로토콜로 시작해서 전체 경로를 입력함
웹 이미지 절대경로 예) - /apple.png
루트('/') 디렉터리 부터 시작하는 경우 현재 도메인이 자동으로 앞에 붙음

### 상대경로
상대경로는 현재 문서를 기준으로 경로를 인식하는 방법

- `index.html` 에서 동일한 위치에 있는 apple.png를 가져오는 방법 → `src="apple.png"`
- `index.html` 의 상위 폴더에 이미지가 있는 경우 → `src="../apple.png"`
- `index.html` 의 하위 폴더에 이미지가 있는 경우 → `src="하위폴더/apple.png"`

## 오디오 태그

---

`<audio>` 태그는 HTML 문서에 소리 콘텐츠를 넣을 때 사용합니다. 


```html
<!-- controls : 컨트롤 바 --> 
<audio controls src="/media/cc0-audio/t-rex-roar.mp3" controls>
```

## 비디오 태그


`<video>` 태그는 영상 콘텐츠를 HTML 문서에 삽입할 때 사용

```html
<!-- src 속성을 사용 -->
<video controls src="/media/cc0-videos/flower.mp4" type="video/mp4" controls>
```

## 오디오&비디오 태그 속성

- `controls` - 플레이어 화면에 컨트롤 바(재생막대)를 표시
- `autoplay` - 오디오나 비디오를 자동으로 실행
    
    단, 크롬, 파이어폭스 브라우저는 자동 재생을 지원하지 않습니다. 만약 자동 재생을 하고 싶다면 `muted` 속성을 사용하여 소리를 제거해야 함
    
- `loop` - 오디오나 비디오를 반복 재생
- `muted` - 오디오나 비디오의 소리를 제거
- `preload` - 페이지를 불러올 때 오디오나 비디오 파일을 어떻게 로딩할 것인지 지정. 사용할 수 있는 값은 `auto` `metadata` `none` 
    
    기본적으로 `preload="auto"` 가 사용.
    
- `width` `height` - 비디오 플레이어의 너비와 높이를 지정합니다. `width` 나 `height` 의 값 중에서 하나만 지정하면 나머지는 자동으로 계산해서 표시
- `poster="파일 이름"` - `<video>` 태그에서 사용하는 속성으로, 비디오가 재생되기 전까지 화면에 표시될 포스터 이미지를 지정

## 하이퍼링크 태그

- 이메일 보내기 하이퍼링크
  
    ```html
    <a href="mailto:bruce.lean17@gmail.com">이메일 보내기</a>
    ```
    
- ID 속성이 apple인 특정위치로 이동하는 하이퍼링크
    
    ```html
    <!-- id가 apple인 요소로 이동하는 하이퍼링크 -->
    <a href="#apple">이동</a>
    
    <!-- 해당 요소 위치로 스크롤이 이동함 -->
    <div id="apple">사과</div>
    ```

### 속성

- `href`
    
하이퍼링크가 가리키는 URL. 링크는 HTTP 기반 URL일 필요는 없고, 브라우저가 지원하는 모든 URL 스킴을 사용할 수 있다.
    
    - 페이지 구획을 가리키는 프래그먼트 URL
    - 미디어 파일 일부를 가리키는 미디어 프래그먼트
    - `tel:` URL을 사용하는 전화번호
    - `mailto:` URL을 사용하는 이메일 주소
    
    
## Form

### Input태그

### text

`<input>` 태그의 기본값으로 한줄의 텍스트를 입력 받습니다.

```html
<input type="text" id="name">
```

HTML5 에서는 text 필드가 데이터 용도에 맞게 사용할 수 있도록 다양한 타입이 추가되었음

- `text` - 일반적인 텍스트를 받기위해 사용
- `password` - 비밀번호를 받기위해 사용
- `email` - email 데이터를 받기위해 사용 (이메일 유효성 검증)
- `tel` - 전화번호를 받기위해 사용 (모바일 접근시 키패드가 다름)

### label

`<label>` 레이블 태그는 입력받는 필드를 설명할 때 사용합니다. `웹접근성 준수`

사용 방법은 `<label>` 태그 하위에 `<input>` 태그를 위치시킬 수 있고 `id` 와 `for` 속성을 사용하여 `<input>` 태그와 연결지을 수 있습니다.

```html
<!-- label 태그 하위에 놓는 법 -->
<label>
	이름 : 
	<input type="text" id="name">
</label>

<!-- for와 id속성을 사용하여 label 태그와 연결지음 / for값과 id값 일치 -->
<label for="name">이름 : </label>
<input type="text" id="name">
```

### number

`<input type="number">` 속성은 숫자를 입력하기 위한 필드입니다.

- `min` 속성으로 최소값을 지정
- `max` 속성으로 최대값을 지정
- `value` 속성은 이 요소의 현재 값 이며, 초기에 value 값이 화면에 표시됨

```html
<input type="number" min="0" max="10" value="0">
```

### range

슬라이드 막대를 움직여서 값을 입력받을 수 있습니다.

- `min` 속성으로 최소값을 지정
- `max` 속성으로 최대값을 지정
- `value` 속성은 이 요소의 현재 값 이며, 초기에 value 값이 화면에 표시됨

```html
<input type="range" min="0" max="10" value="0">f
```

### 날짜/시간

`date` `month` `week` `time` `datetime` `datetime-local` 값을 사용하여 날짜와 시간 데이터를 입력 받을 수 있습니다.

- `min` 속성으로 최소 날짜를 지정 합니다.
- `max` 속성으로 최대 날짜를 지정 합니다.

### hidden

눈에 보이지는 않지만 서버로 값을 전송하려고 할 때 사용하는 요소.

예) 가입시간, 가입경로 등

```html
<input type="hidden" name="source" value="google">
```

### file

파일을 선택할 수 있는 필드입니다. `accept` 속성을 사용하면 허용하는 파일 유형을 지정할 수 있습니다.

```html
<input type="file">
```

### image

제출 버튼으로 사용할 이미지 버튼이라고 보시면 될 것 같습니다.

```html
<input type="image" src="버튼으로 사용할 이미지 경로">
```

## Form 데이터 태그 속성


- `required`
    
    입력값이 필수라는 것을 명시할 수 있습니다.
    
- `readonly`
    
    필드를 읽기전용으로 필드로 만들 수 있습니다. / disable과 달리 서버로 값은 전송 됨
    
- `disabled`
    
    비활성화 시킬 수 있으며 해당 필드는 서버로 전송되지 않습니다. / 흐릿하게 표시 됨
    
- `autofocus`
    
    초기에 해당 필드에 커서를 위치 시킬 수 있음
    
- `placeholder`
    
    입력 필드가 비어있을 때 해당 입력값의 설명 또는 가이드 문구를 삽입할 수 있음
    

## fieldset

양식의 여러 컨트롤과 레이블(<label>)을 묶을 때 사용

### legend

 요소는 부모 `<fieldset>` 콘텐츠의 설명을 나타냄
 
 ## Textarea

`<textarea>`는 여려줄의 데이터를 입력받을 수 있다.

```html
<textarea id="story" name="story" rows="5" cols="33">
It was a dark and stormy night...
</textarea>
```

**속성**

- `rows` - 화면에 표시되는 행수를 지정합니다.
- `cols` - 화면에 표시되는 컬럼 수를 지정합니다.
