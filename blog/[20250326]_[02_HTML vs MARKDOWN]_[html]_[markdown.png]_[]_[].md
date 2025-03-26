# html vs markdown

## 01_Markdown이란?

이전 글에서 살펴보았듯 html은 결국 웹에서 문서를 작성할 수 있는 언어이다. 

html은 새로운 버전이 늘어나면서 필요한 태그도 많아졌고, ? 해서 간단한 문서를 작성하기에는 너무 어려웠다.

이에 2004년 ..?  존 그루버가 간단한 텍스트 포맷으로 작성된 문서를 HTML로 변환할 수 있는 시스템을 만들기 위해 개발하였다. 

더 간단한 문법으로 손쉽게 웹 문서를 작성할 수 있도록 돕는 것이었다.

예를 들어

```jsx
<html>
<head>
<title>페이지 제목</title>
</head>
<body>
<h1>환영합니다!</h1>
<p>HTML로 작성된 웹 페이지입니다.</p>
<a href="[https://example.com](https://example.com/)">예시 링크</a>
</body>
</html>
```

이런 HTML 문서가 markdown으로 한다면,

```jsx
# 환영합니다!
Markdown으로 작성된 문서입니다.

[예시 링크](https://example.com)

```

이런식으로 간단하게 되는 것이다.

## 02_HTML vs Markdown

HTML은 웹페이지를 구성할 때, 즉, 웹사이트를 만들 때 사용한다. 네이버, 구글과 같은 웹사이트를 만들 때 사용하는 언어가 HTML이라고 생각하면 된다. 

반면, Markdown은 주로 글을 작성할 때, 즉 웹의 콘텐츠를 작성할 때 사용된다. 주피터 노트북, 구글 코랩, 깃허브 등의 코드를 사용하는 플랫폼에서 주로 사용되며, 노션 같은 플랫폼에서도 Markdown 형식으로 글을 작성한다.


<figure>
  <img src="eekals/da_blog/img/코랩_마크다운.png" width="300" />
  <figcaption>코랩 텍스트 문서는 markdown 형식</figcaption>
</figure>

## 03_ Markdown 활용법

Markdown은 코랩, GitHub 등 개발 플랫폼에서 자주 활용되므로 그 간단한 문법을 이해하는 것이 매우 유용하다. 요즘에는 Typora, Marktext와 같은 Markdown 편집기를 사용해 글을 쓰고, 이를 Markdown 형식으로 변환해주는 프로그램들도 많다. 또한, 노션 같은 플랫폼에서도 글을 쓰고 Markdown 형식으로 내보낼 수 있어, 이를 활용해보는 것도 좋은 방법이다.

<figure>
  <img src="eekals/da_blog/img/노션.png" width="300" />
  <figcaption>노션 내보내기를 통해 글을 markdown으로 편집</figcaption>
</figure>

