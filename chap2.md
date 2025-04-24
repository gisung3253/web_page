# HTML 기초

## 개요
- 마크업 작동 방식에 대한 이해(요소와 속성 포함)
- 브라우저가 HTML 문서를 해석하는 방법 이해
- HTML 문서의 기본 구조 학습


## 필요 도구
- **텍스트 에디터** - 코드 작성용
  - VS Code: https://code.visualstudio.com
- **웹 브라우저** - 결과물 확인용
  - Chrome: www.google.com/chrome


## HTML 요소(Elements)
- HTML 요소는 텍스트 소스에서 태그로 식별된다.
- 태그는 꺾쇠 괄호(< >) 내에 요소 이름으로 구성된다.
- 요소는 콘텐츠와 마크업(시작 태그와 종료 태그) 모두로 구성된다.
- 일부 요소는 정의상 비어 있다. 예를 들어 이미지를 페이지에 추가하는 데 사용되는 img 요소가 이에 해당한다.


## 기본 문서 구조(Basic Document Structure)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>Title here</title>
</head>
<body>
    Page content goes here.
</body>
</html>
```

1. **문서 유형 선언(DOCTYPE)**: `<!DOCTYPE html>`
   - 이 문서를 HTML5 문서로 식별한다

2. **html 또는 루트 요소**: `<html lang="en">`
   - 문서의 모든 요소를 포함한다

3. **head 요소**: `<head>`
   - 문서에 대한 메타데이터를 포함한다

4. **meta 요소**: `<meta charset="utf-8">`
   - 문서 자체에 대한 정보를 제공한다 (이 경우 문자 인코딩)

5. **제목(title) 요소**: `<title>Title here</title>`
   - 브라우저 탭에 표시되는 페이지 제목

6. **본문(body) 요소**: `<body>Page content goes here.</body>`
   - 브라우저 창에 표시될 정보를 포함한다


## 텍스트 요소 식별하기(Identify Text Elements)

- HTML의 목적은 콘텐츠에 의미와 구조를 추가하는 것이다.
- 콘텐츠가 어떻게 보여야 하는지(표현)에 대한 지시사항을 제공하기 위한 것이 아니다.
- 콘텐츠를 마크업할 때 해당 콘텐츠를 가장 의미 있게 설명하는 HTML 요소를 선택하는 것이 중요하다.
- 이를 시맨틱 마크업(semantic markup)이라고 한다.
- 또한 마크업은 문서에 구조를 부여한다.
- 요소들이 서로 따르거나 중첩되는 방식은 요소 간의 관계를 생성한다.
- 이것을 개요(outline)로 생각할 수 있다 (기술적인 이름은 DOM, Document Object Model이다).

![문서 객체 모델(DOM) 구조](images/dom.png)


## 블록 요소와 인라인 요소(Block and inline elements)

### 블록 요소(Block elements)
- 브라우저는 블록 요소를 사각형 박스처럼 처리하여 페이지에 쌓아 올린다.
- 각 블록 요소는 새로운 줄에서 시작하며, 기본적으로 요소 위아래에 약간의 공간이 추가된다.
- 예시: 제목(headings), 단락(paragraphs) 등
- 블록 요소는 문서의 구조적인 요소로 사용된다.

### 인라인 요소(Inline elements)
- 인라인 요소는 새로운 줄을 시작하지 않고 텍스트 흐름을 따라간다.
- 예시: `<em>` 요소 (강조)
- 인라인 요소는 주로 텍스트의 일부를 스타일링하거나 특별한 의미를 부여하는 데 사용된다.

![블록과 인라인 요소](images/block_inline.png)


## 빈 요소(Empty elements)

- 일부 요소는 텍스트 내용을 갖지 않으며, 단순한 지시사항을 제공하는 용도로 사용된다.
- 이러한 요소를 '빈 요소'라고 한다.
- 빈 요소는 시작 태그만 가지며, 종료 태그가 없다.

### 주요 빈 요소
- **img**: 이미지 요소는 서버에서 이미지 파일을 가져와 텍스트 흐름 내에 삽입한다.
- **br**: 줄바꿈(line break) 요소는 텍스트에 줄바꿈을 삽입한다.
- **hr**: 주제 구분선(thematic break) 요소는 내용 사이에 구분선을 추가한다.
- **meta**: 문서에 대한 정보를 제공하지만 표시되는 내용에는 영향을 주지 않는다.

```
<p>1005 Gravenstein Highway North<br>Sebastopol, CA 95472</p>
```


## HTML 속성(Attributes)

- 속성은 요소를 명확히 하거나 수정하는 지시사항이다.
- 속성은 요소에 추가 정보를 제공한다.
- 속성은 이름과 값으로 구성되며, 등호(=)로 구분된다.
- 속성 값은 따옴표(" ")로 묶는다.
- 여러 속성은 공백으로 구분한다.

### img 요소의 속성
- `img` 요소에는 `src` 속성이 필수이며, 이미지 파일의 위치(URL)를 지정한다.
- `src`는 "source"의 약자이다.
- `alt` 속성은 이미지를 표시할 수 없을 때 대체 텍스트를 제공한다.

```
<img src="bird.jpg" alt="photo of bird">
```
![속성의 구조](images/attributes.png)


## HTML 문서 기본 구조 요약

HTML 문서는 다음과 같은 기본 구조 요소로 구성된다:

| 요소 | 설명 |
|------|------|
| html | 모든 요소를 포함하는 루트 요소 |
| head | 문서에 대한 정보를 포함하는 영역 |
| title | 페이지 제목을 정의 |
| meta | 문서에 대한 메타데이터 제공 |
| body | 브라우저에 표시될 모든 콘텐츠를 포함하는 영역 |


## 단락 요소(Paragraphs)

- 단락은 텍스트 문서의 가장 기본적인 요소이다.
- 단락은 텍스트, 이미지 및 기타 인라인 요소를 포함할 수 있지만, 제목, 목록, 섹션 요소 또는 기본적으로 블록으로 표시되는 요소는 포함할 수 없다.

```html
<p>Serif 서체는 글자 획의 끝에 작은 장식이 있다. 일반적으로 serif 글꼴은 많은 양의 텍스트를 읽기 쉽게 만든다.</p>

<p>Sans-serif 서체는 serif 장식이 없으며, 끝 부분이 사각형이다. Helvetica와 Arial은 sans-serif 글꼴의 예이다. 일반적으로 sans-serif 글꼴은 더 세련되고 현대적으로 보인다.</p>
```

> **참고**: 문서의 모든 텍스트에는 요소를 할당해야 한다. 다시 말해, 모든 텍스트는 어떤 형태의 요소로 감싸야 한다. 태그 내에 포함되지 않은 텍스트는 "naked" 또는 "anonymous" 텍스트라고 하며, 문서가 유효하지 않게 된다.


## 제목 요소(Headings)

- 제목은 h1부터 h6까지 6단계로 구분된다.
- 브라우저는 제목을 사용하여 페이지의 문서 개요를 생성한다.
- 스크린 리더와 같은 보조 기기는 문서 개요를 사용하여 사용자가 페이지를 빠르게 스캔하고 탐색할 수 있도록 도와준다. 또한 검색 엔진은 알고리즘의 일부로 제목 수준을 확인한다.
- 가장 좋은 방법은 수준 1 제목(h1)으로 시작하여 순서대로 내려가면서 논리적인 문서 구조와 개요를 생성하는 것이다.


## 목록 요소(Lists)

HTML은 세 가지 유형의 목록을 마크업하기 위한 요소를 제공한다:

- **순서 없는 목록(Unordered lists)**: 특별한 순서 없이 나타나는 항목의 모음이다.
- **순서 있는 목록(Ordered lists)**: 항목의 순서가 중요한 목록이다.
- **설명 목록(Description lists)**: 용어와 정의를 포함한 이름과 값 쌍으로 구성된 목록이다.

### 순서 없는 목록(Unordered Lists)

- 순서 없는 목록은 예시, 이름, 구성 요소, 생각 또는 옵션의 목록에 적합하다. 대부분의 목록이 이 범주에 속한다.
- 기본적으로 브라우저는 각 목록 항목 앞에 글머리 기호(bullet)를 표시하지만, 스타일시트를 통해 변경할 수 있다.

```html
<ul>
  <li><a href="">Serif</a></li>
  <li><a href="">Sans-serif</a></li>
  <li><a href="">Script</a></li>
  <li><a href="">Display</a></li>
  <li><a href="">Dingbats</a></li>
</ul>
```

> **참고**: 순서 없는 목록(`ul` 태그) 내에는 오직 목록 항목만 허용된다. 다른 요소나 태그가 없는 텍스트는 포함할 수 없다. 하지만 목록 항목(`li`) 내에는 모든 타입의 흐름 요소를 포함할 수 있다.

### 순서 있는 목록(Ordered Lists)

- 순서 있는 목록은 단계별 지침이나 운전 방향과 같이 특정 순서로 발생하는 항목에 적합하다.
- 브라우저는 순서 있는 목록 항목 앞에 자동으로 번호를 삽입하므로, 소스 문서에서 직접 번호를 매길 필요가 없다.

```html
<ol>
  <li>Gutenburg develops moveable type (1450s)</li>
  <li>Linotype is introduced (1890s)</li>
  <li>Photocomposition catches on (1950s)</li>
  <li>Type goes digital (1980s)</li>
</ol>
```

### 설명 목록(Description Lists)

- 설명 목록은 용어와 각 용어에 대한 설명으로 구성된 목록이다.
- `dl` 태그는 설명 목록을 정의하고, `dt` 태그는 용어(이름)를 정의하며, `dd` 태그는 각 용어에 대한 설명을 제공한다.
- `dt`는 "Definition Term"(정의 용어)의 약자이고, `dd`는 "Description Details"(설명 세부사항)의 약자이다.

```html
<dl>
  <dt>Sashimi</dt>
  <dd>Sliced raw fish that is served with condiments such as shredded daikon radish or ginger root, wasabi and soy sauce</dd>
  <dt>Scale</dt>
  <dd>A device used to accurately measure the weight of ingredients</dd>
  <dd>A technique by which the scales are removed from the skin of a fish</dd>
  <dt>Scamorze</dt>
  <dt>Scamorzo</dt>
  <dd>An Italian cheese usually made from whole cow's milk (although it was traditionally made from buffalo milk)</dd>
</dl>
```


## 문서 유효성 검사(Validating Your Documents)

- 문서의 유효성을 검사한다는 것은 사용 중인 HTML 버전의 규칙을 제대로 따랐는지 마크업을 확인하는 것이다.
- 오류가 없는 문서는 "유효한(valid)" 문서라고 한다.
- 특히 전문적인 사이트의 경우 문서의 유효성을 검사하는 것이 강력히 권장된다.
- 유효한 문서는 다양한 브라우저에서 더 일관되게 표시되고, 더 빠르게 로드되며, 접근성이 더 높다.

### 유효성 검사 중요 사항

- 문서의 모든 텍스트에는 요소를 할당해야 한다. 즉, 모든 텍스트는 어떤 형태의 요소로든 감싸져 있어야 한다.
- 태그 내에 포함되지 않은 텍스트는 "naked" 또는 "anonymous" 텍스트라고 하며, 이로 인해 문서가 유효하지 않게 된다.

### 온라인 유효성 검사 도구

- W3C는 validator.w3.org에서 무료 온라인 유효성 검사기를 제공한다.
- HTML5 문서의 경우 html5.validator.nu에 있는 온라인 유효성 검사기를 사용한다.