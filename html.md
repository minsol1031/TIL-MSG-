# html

## html요소의 구조
- __여는 태그(Opening tag)__: 이것은 요소의 이름과(이 경우 p), 열고 닫는 꺽쇠 괄호로 구성된다. 요소가 시작(이 경우 단락의 시작 부분)부터 효과가 적용되기 시작
- __닫는 태그(Closing tag)__: 이것은 요소의 이름 앞에 슬래시(/)가 있는것을 제외하면 여는 태그(opening tag)와 같다. 이것은 요소의 끝(이 경우 단락의 끝 부분)에 위치한다. 닫는 태그를 적어주지 않는 것은 흔한 초심자의 오류이거, 이것은 이상한 결과가 나온다
- __내용(Content)__: 요소의 내용이며, 이 경우 단순한 텍스트이다.
- __요소(Element)__: 여는 태그, 닫는 태그, 내용을 통틀어 요소(element)라고한다.

## 블럭 레벨 요소 vs 인라인 요소
- __블록 레벨 요소(Block-level elements)__: 웹페이지 상에 블록을 만드는 요소
    - 블록 레벨 요소를 사용해 단락, 목록, 네비게이션 메뉴, 꼬리말 등을 표현
- __인라인 요소(Inline elements)__:  항상 블록 레벨 요소내에 포함
    - 인라인 요소에는 하이퍼링크를 정의하는 요소인 ```<a>``` , 텍스트(Text)를 강조하는 요소인 ```<em>,<strong>``` 등이 있음
```
<em>first</em>
<em>second</em>
<em>third</em>

<p>fourth</p>
<p>fifth</p>
<p>sixth</p>
```
__실행__   
<em>first</em>
<em>second</em>
<em>third</em>

<p>fourth</p>
<p>fifth</p>
<p>sixth</p>

## 빈 요소(Empty elements)
모든 요소가 여는 태그, 내용, 닫는 태그 패턴을 따르는 것은 아니다. 주로 문서에 무언가를 첨부하기 위해 단일 태그(Single tag)를 사용하는 요소도 있다. 예를 들어 ```<img>``` 요소는 해당 위치에 이미지를 삽입하기 위한 요소이다
```
<img
  src="https://raw.githubusercontent.com/mdn/beginner-html-site/gh-pages/images/firefox-icon.png" />
```
__실행__

<img
  src="https://raw.githubusercontent.com/mdn/beginner-html-site/gh-pages/images/firefox-icon.png" />

 ## 속성(Attributes)

 ### 속성 이용시 조건
 - 요소 다음에 바로 오는 속성은 사이에 공백이 있어야 하고, 한개 이상의 속성이 있을 경우 속성 사이에 공백이 있어야 한다.
- 속성 이름 다음엔 등호(=)가 붙는다.
- 속성 값은 열고 닫는 따옴표로 감싸야 한다.

### 참과 거짓 속성(Boolean attributes)
때때로 값이 없는 속성을 볼 수 있을텐데 이것은 허용되는 것, 불 속성이라고 하고, 일반적으로 그 속성의 이름과 동일한 하나의 값만을 가질 수 있다. 

## Entity references: HTML에 특수 문자 포함
| Literal character	| Character reference equivalent|
|---|---|
| <	 | ```&lt;``` |
|>	| ```&gt;``` |
| "	| ```&quot;``` |
| '	| ```&apos;```|
| & |``` &amp;```|

## HTML 주석
HTML 주석을 쓰려면 특수 마커 <!- 및 ->로 주석을 묶는다.
```
<p>I'm a sudent</p>

<!-- <p>I am!</p> -->
```
<p>I'm a sudent</p>

<!-- <p>I am!</p> -->