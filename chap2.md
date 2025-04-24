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

