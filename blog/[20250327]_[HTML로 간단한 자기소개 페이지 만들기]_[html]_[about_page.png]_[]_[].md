# HTML 로 간단한 자기소개 페이지 만들기

## head 태그 살펴보기

head 는 웹페이지에 문서를 작성하기 앞서 기본적인 세팅을 준비하는 공간이라고 할 수 있다.

간단한 예로, 폰트를 설정하거나, 문서에 필요한 외부파일을 불러오거나, 웹페이지의 제목을 

설정하는 등 웹페이지에서 글이나 이미지처럼 직접적으로 보이지는 않지만 웹페이지가 제대로 표시되거나 작동하기 위해 꼭 필요한 설정들을 담고 있다.

## body 태그 살펴보기

body 는  웹페이지에서 실제로 보여지는 공간이라고 할 수 있다.

**글, 이미지, 버튼, 링크, 동영상 등** 웹페이지에서 사용자에게 보여지는 요소가 들어가 있는 공간이다.

이번 글에서는 아주 간단한 head 와 body 구조로 웹페이지를 구현해보고자 한다.

- &lt;link&gt; 태그를 이용하여 외부파일 불러오기(이미지, 폰트)
- &lt;body&gt; 에 글, 이미지, 링크 만들기

```html
<!DOCTYPE html>
<html>
<head lang="ko">
    <!-- 인코딩 설정 및 반응형 웹 설정 -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- 브라우저 제목 및 아이콘 설정 -->
    <title>About Me</title>
    <link rel = 'icon' href = 'icon_img.jpg'>
    
    <!-- Google Fonts에서 Gmarket Sans 폰트 가져오기 -->
    <link href="https://fonts.googleapis.com/css2?family=Gmarket+Sans:wght@500&display=swap" rel="stylesheet">

</head>

</html>
```

아주 간단하게, 브라우저의 제목과 아이콘을 설정하고, &lt;link&gt;태그를 통해 icon의 이미지와 폰트를 불러오는 코드를 작성하였다.

위의 코드를 시행하면, 

![image.png](img/user/icon.png)

과 같이 제목과 아이콘이 나타난다.

body 부분에는 

- **제목(`h1`)**: 자신의 이름 또는 웹페이지 주제
- **단락(`p`)**: 자기소개 및 관심사
- **이미지(`img`)**: 본인 사진 또는 대표 이미지
- **링크(`a`)**: 관심 있는 사이트로 이동하는 링크

위의 태그를 넣으려 한다.

```html

<body>
    <h1>Ohamin's Webpage</h1>

    <img src="https://eekals.github.io/da_blog/img/test_3.jpg" alt="Profile Image" width="300" />
    <h1>안녕하세요, 데이터분석가를 꿈꾸는 오다민입니다.</h1>

    <p>저는 "<strong>최대한 간결하게, 최대한 쉽게</strong>" 전달하는 것을 중요하게 생각합니다.</p>

    <h2>데이터 분석은:</h2>
    <ul>
        <li>단순히 정보를 분석하는 것이 아닌 <strong>협업을 통한 문제 해결</strong></li>
        <li>분석 결과를 <strong>쉽게 전달</strong>하는 과정</li>
    </ul>

    <p>데이터를 시각적으로 효과적으로 표현하는 방법에 대해 많은 관심을 가지고 있으며,<br>
       복잡한 정보를 누구나 쉽게 이해할 수 있도록 전달하는 방법을 고민합니다.</p>

    <p>요즘은 긴 보고서보다 짧고 임팩트 있는 정보를 선호하는 시대입니다.</p>

    
    <h2>저의 목표는:</h2>
        <ul>
            <li><strong>강한 인사이트</strong>를 전달하는 데이터분석가</li>
            <li>함께 <strong>성장</strong>하고 <strong>배움</strong>을 나누는 분석가</li>
            <li>데이터를 통해 <strong>실질적인 변화</strong>를 이끌어내는 분석가</li>
        </ul>

        <P>입니다. 함께 일하는 사람들에게 영감을 줄 수 있는 분석가가 되도록 노력하겠습니다. </P>

        <a href="https://eekals.github.io/da_blog/?menu=Portfolio.md">포트폴리오</a>

</body>
```

복잡해보이지만 위에 쓰인 태그들을 정리해보면 다음과 같다.

| 태그 | 설명 |
| --- | --- |
| `<h1>` | 가장 중요한 제목을 정의하는 태그 (헤딩1) |
| `<img>` | 이미지를 삽입하는 태그 |
| `<p>` | 문단을 정의하는 태그 |
| `<strong>` | 텍스트를 강조하는 태그 (기본적으로 굵은 글씨) |
| `<h2>` | 두 번째로 중요한 제목을 정의하는 태그 (헤딩2) |
| `<ul>` | 순서 없는 리스트를 정의하는 태그 |
| `<li>` | 리스트 항목을 정의하는 태그 |
| `<a>` | 하이퍼링크를 정의하는 태그 |

최종적인 결과물은 다음과 같다.

![image.png](img/About.png)
