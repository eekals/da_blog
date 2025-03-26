# CSS : HTML 디자인 언어

## 01_css란?

css는 Cascading Style Sheets 의 약자로, Style Seets 즉, 웹페이지를 디자인하는 문서인데 Cascading 한 문서라고 생각하면 된다. 

Cascading 은 여러 규칙이 있을 때 순차적으로 적용한다라는 의미이다.

간단한 예를 들면

```jsx
p {
color: black;
}
/* 나중에 덧붙인 스타일 */
p {
color: red;
}
```

해당 코드는 &lt;p&gt;라는 태그에 있는 글씨를 검정(black)으로 하세요.

 &lt;p&gt;라는 태그에 있는 글씨를 빨간색(red) 로 하세요. 라는 의미이다.

이렇게 똑같은 태그에 규칙이 있는 경우 나중에 쓰인 두번째 코드 (red)가 적용이 되는 것이다.

또 다른 예를 들어보자.

```jsx
/* 모든 <p> 태그에 적용될 스타일 */
p {
color: blue;
font-size: 18px;
}
/* 특정 <div> 안에 있는 <p> 태그에만 다른 스타일 적용 */
div p {
  color: red;
  font-size: 20px;
}

```

첫번째 코드는 모든 &lt;p&gt; 태그에 대해서 글자색깔(blue)과 크기(18px)를 정의했다.

두번째 코드는 &lt;div&gt; 코드 안에 있는 &lt;p&gt;  태그에 대해서 스타일을 정의했다.

Cascading 는 간단히 말하면 **나중에 온게 우선 적용된다.**라고 생각하면 된다.

따라서, &lt;div&gt;안의 &lt;p&gt; 태그는 두번째 규칙이, 그 외의 &lt;p&gt;태그는 첫번째 규칙이 적용된다.

## 02_css 구조

CSS의 구조는 다음과 같다.

선택자 {
속성: 값;
속성: 값;
}

01.선택자(selector)

- 어떤 HTML 요소에 적용할 지를 정의하는 것

자주 쓰이는 선택자들을 표로 정리하였다.

| **선택자 종류** | **설명** | **예시** | **효과** |
| --- | --- | --- | --- |
| **태그 선택자** | 특정 HTML 태그를 선택하여 스타일을 적용 | `p { color: red; }` | 모든 `<p>` 태그의 텍스트 색상을 빨간색으로 변경 |
| **클래스 선택자** | 특정 클래스 이름을 가진 요소를 선택 | `.myClass { background-color: yellow; }` | 클래스 `myClass`를 가진 모든 요소의 배경색을 노란색으로 설정 |
| **ID 선택자** | 특정 ID를 가진 요소를 선택 | `#header { font-size: 24px; }` | ID가 `header`인 요소의 글자 크기를 24px로 설정 |
| **후손 선택자** | 특정 요소의 모든 후손 요소를 선택 | `div p { color: green; }` | `div` 요소 내의 모든 `<p>` 태그의 텍스트 색상을 초록색으로 설정 |
| **자식 선택자** | 특정 요소의 직속 자식 요소를 선택 | `div > p { color: blue; }` | `div` 요소의 직속 자식인 `<p>` 태그의 텍스트 색상을 파란색으로 설정 |
| **가상 클래스 선택자** | 특정 상태에 있는 요소를 선택 | `a:hover { color: red; }` | 링크에 마우스를 올렸을 때 텍스트 색상을 빨간색으로 변경 |
| **그룹화 선택자** | 여러 선택자를 한 번에 스타일을 적용 | `h1, h2, h3 { color: darkblue; }` | `<h1>`, `<h2>`, `<h3>` 태그 모두 텍스트 색상을 어두운 파란색으로 설정 |
1. 속성 : 값
- 속성은 스타일의 종류를, 값은 구체적인 값

자주 쓰이는 속성값

| **속성** | **값** | **설명** |
| --- | --- | --- |
| `color` | `red`, `blue`, `green`, `#ff0000`, `rgb(255,0,0)` | 텍스트의 색상을 지정 |
| `background-color` | `yellow`, `#f0f0f0`, `rgba(0,0,0,0.1)` | 요소의 배경 색상을 설정 |
| `font-size` | `12px`, `16px`, `1.5em`, `1rem` | 텍스트의 크기를 설정 |
| `font-family` | `Arial`, `sans-serif`, `Times New Roman` | 텍스트에 사용할 폰트를 설정 |
| `line-height` | `1.5`, `normal`, `20px` | 텍스트 줄 간격을 설정 |
| `margin` | `10px`, `1em`, `auto` | 요소의 바깥 여백을 설정 |
| `padding` | `10px`, `2em` | 요소의 안쪽 여백을 설정 |
| `width` | `100px`, `50%`, `auto` | 요소의 너비를 설정 |
| `height` | `100px`, `50%`, `auto` | 요소의 높이를 설정 |
| `border` | `1px solid black`, `2px dashed red` | 요소의 테두리를 설정 |
| `display` | `block`, `inline`, `flex`, `none` | 요소의 디스플레이 방식을 설정 |
| `text-align` | `left`, `center`, `right`, `justify` | 텍스트의 정렬을 설정 |
| `position` | `static`, `relative`, `absolute`, `fixed`, `sticky` | 요소의 배치 방법을 설정 |
| `z-index` | `1`, `10`, `auto` | 요소의 쌓임 순서를 설정 (주로 `position`과 함께 사용) |
| `box-shadow` | `2px 2px 5px rgba(0,0,0,0.3)` | 요소에 그림자 효과를 추가 |
| `opacity` | `0`, `1`, `0.5` | 요소의 투명도를 설정 (0은 투명, 1은 불투명) |
| `border-radius` | `5px`, `50%`, `10px 20px 30px 40px` | 요소의 모서리를 둥글게 만듦 |
| `flex` | `1`, `0`, `auto`, `grow`, `shrink` | flex 컨테이너에서 flex 아이템의 크기 조정 |

## 03_HTML 문서의 &lt;style&gt; 과의 차이는?

html 문서 내에서도 &lt;style &gt; 태그를 이용하여 웹페이지를 꾸며줄 수 있다. 

```jsx
<head>
<style>
body {
background-color: lightblue;
}
h1 {
color: green;
}
</style>
</head>
```

하지만, 이런 방식은 해당 html 문서 내에서만 적용이 가능하다. 

즉, 다른 html에 똑같은 스타일을 적용하기 위해서는 매번 해당 코드를 재작성해야하는 번거로움이 있다.

반면, css파일을 해당 html 파일에 불러오는 방식으로 하면,

```jsx
<head>
<link rel="stylesheet" href="styles.css">
</head>
```

위와 같이 &lt;link&gt; 태그를 이용해서 styles.css라는 외부 css파일을 불러오기만 하면,

styles.css에 저장되어 있는 스타일을 바로 적용할 수 있다.

## 03_CSS와 HTML

CSS는 HTML의 구조적인 콘텐츠에 스타일을 추가하는 중요한 역할을 한다. HTML은 웹페이지의 내용과 구조를 정의하지만, CSS는 그 내용을 어떻게 보일지 디자인한다.. 웹페이지의 색상, 글꼴, 레이아웃을 조정하여 사용자에게 더 나은 경험을 제공하고, 다양한 기기에서 웹페이지가 잘 보이도록 만들어준다.

## 04_ 관련 툴

요즘에는 **Figma**나 **Webflow**와 같은 툴을 사용하면, HTML에 대한 복잡한 이해 없이도 디자인 중심으로 웹 개발을 할 수 있다. 이러한 툴들은 드래그 앤 드롭 방식(원하는 요소를 클릭하고, 원하는 위치로 드롭)으로 직관적인 웹 디자인을 가능하게 하고, HTML과 CSS 코드가 자동으로 생성되기 때문에 웹페이지를 빠르고 쉽게 만들 수 있다. 이와 같은 툴들을 활용하여 간단한 웹페이지를 만들어보는 것도 좋은 학습 방법이 될 것이다.

[https://eekals.github.io/da_blog/?post=[20250325]_[Webflow+로+웹페이지만들기_1]_[webflow]_[탬플릿.JPG]_[]_[].md](https://eekals.github.io/da_blog/?post=%5B20250325%5D_%5BWebflow+%EB%A1%9C+%EC%9B%B9%ED%8E%98%EC%9D%B4%EC%A7%80%EB%A7%8C%EB%93%A4%EA%B8%B0_1%5D_%5Bwebflow%5D_%5B%ED%83%AC%ED%94%8C%EB%A6%BF.JPG%5D_%5B%5D_%5B%5D.md) ( Webflow의 탬플릿을 활용하여 웹페이지만들기)


