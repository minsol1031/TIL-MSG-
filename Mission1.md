# 마크다운
# 개요
```
마크다운은 마크업 언어의 일종으로, 존 그루버와 아론 스워츠가 만들었다.  읽기도 쓰기도 쉬운 문서 양식을 지향한다. HTML로 변환이 가능하다. 볼 수 있는 파일명은 "README.md", 파일의 확장자는 .md 또는 .markdown을 쓴다
```
# 장단점
장점
----
```
1. 간결하다.
2. 별도의 도구없이 작성가능하다.
3. 다양한 형태로 전환 가능하다.
4. 텍스트로 저장되기에 용량이 적어 보관이 편하다.
5. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다.
6. 지원 프로그램과 플랫폼이 다양하다.
```
단점
---
```
1. 표준이 없다.
2. 표준이 없기 때문에 도구에 따라서 변환방식이나 생성물이 다르다.
3. 모든 HTML 마크업을 대신하지 못한다.
```

# 사용방법

제목
----
```
# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
제목들의 크기 키움
```
__실행 결과__
# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6

```
제목 1
======

제목 2
------
```
__실행 결과__

제목 1
======

제목 2
------


# 강조
```
이텔릭체: *별 기호*, _언더바 기호_ 
두껍게: **별 기호**, __언더바 기호__ 
__*이텔릭체*,두껍게__ 같이 사용 가능
취소선: ~~물결 기호~~

<u>밑줄</u>은 마크다운에서 지원하지 않기에, 직접 `<u></u>` 태그를 사용
```
__실행 결과__

- 이텔릭체: 별 기호*, _언더바 기호_

- 두껍게: **별 기호**, __언더바 기호__ 

- 같이: __*이텔릭체*,두껍게__

- 취소선: ~~물결 기호~~

- 밑줄: `<u></u>`


# BlockQuote
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
__실행 결과__
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

__안에서 다른 마크다운 요소를 포함가능__
>This is a H3
> - List
> ``` code ```

# 목록
```
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째

글머리 기호
---
```
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
```
__실행 결과__
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑

__혼합사용 가능__
```
* 1단계
  - 2단계
    + 3단계
      + 4단계
```
__실행 결과__
* 1단계
  - 2단계
    + 3단계
      + 4단계

수평선
---
```
* * *

***

*****

- - -

---------------------------------------
```

__실행결과__
* * *

***

*****

- - -

---------------------------------------

# 표
```
| 표1 | 표2 |
| --- | --- |
| 표3 | 표4 |
| 표5 | 표6 |
```
| 표1 | 표2 |
| --- | --- |
| 표3 | 표4 |
| 표5 | 표6 |

# 코드
들여쓰기
---
```
This is a normal paragraph:

    This is a code block.
    
end code block.
```
__실행 결과__

This is a normal paragraph:

    This is a code block.
    
end code block.

# 링크

참조링크
---
```
[link keyword][id]

[id]: URL "Optional Title here"

// code
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
```
__실행결과__

* [link keyword][id]

[id]: URL "Optional Title here"

* // code
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
외부링크
---
```
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
```
__실행결과__

*사용문법: [Title](link)

*적용예: [Google](https://google.com, "google link")

자동연결
---
```
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
```
__실행결과__
* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

# 이미지
```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```
* 사이즈 조절 기능이 없기에 <img width="" height=""></img>를 이용한다.

# 줄바꿈
3칸 이상 띄어쓰기( )를 하면 줄이 바뀐다.
```
 줄 바꿈을 위해 문장 마지막에서 3칸이상을 띄어쓰기를 한다. 

ex)
 줄 바꿈을 위해 문장 마지막에서 3칸이상을 띄어쓰기를 한다.___\\ 띄어쓰기
```
 줄 바꿈을 위해 문장 마지막에서 3칸이상을 띄어쓰기를 한다. 

ex)
 * 줄 바꿈을 위해 문장 마지막에서 3칸이상을 띄어쓰기를 한다.___\\ 띄어쓰기
