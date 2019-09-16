# Markdown Syntax 마크다운 작성법
마크다운(Markdown)은 일반 텍스트 문서의 양식을 편집하는 문법입니다.<br><br> 
README파일이나 온라인 문서, 혹은 일반 텍스트 편집기로 문서 양식을 편집할 때 쓰입니다.<br><br>
마크다운을 이용해 작성된 문서는 쉽게 HTML 등 다른 문서형태로 변환이 가능합니다.<br><br>
존 그루버는 2004년에 문법 면에서 [에런 스워츠](https://ko.wikipedia.org/wiki/%EC%97%90%EB%9F%B0_%EC%8A%A4%EC%9B%8C%EC%B8%A0)와
중대한 협업을 통해 마트다운 언어를 만들었으며, 사람들이 일기 쉽고 쓰기 쉬운 플레인 텍스트 포맷을 사용하여 쓸 수 있으면서 구조적으로 유효한 HTML로 선택적 변환이 가능합니다.[John Gruber
(DaringFireball)](http://daringfireball.net/projects/markdown/syntax).
## Markdown Pros 마크다운 장점
* `읽기 쉽다.` 확실히 마크다운은 다른 마크업 언어에 비해 가독성이 좋습니다. 문법도 단순하고, HTML은 작성하면서 브라우저에서 어떻게 보여
질지 예상하는게 쉽지 않지만, 마크다운을 사용한 텍스트는 브라우저에 보여질 내용을 쉽게 상상할 수 있습니다.
* `익히기 쉽다.` 존 그루버는 사람들이 많이 사용하는 것은 마크다운으로 사용하고, 복잡한 것은 HTML로 사용하기 바랬습니다. 그래서 문법이 매우 간단합니다. 그리고 마크다운으로 글을 작성할 때, 제한적인 기능 몇 개를 제외하고 HTML을 함께 사용해도 상관없습니다.
* `모바일 친화적이다.` 단순히 텍스트만 작성하는 것이 아닌 에디터를 이용해 모바일로 작성하는 것은 쉽지 않습니다. 하지만 마크다운을 이용하면 모바일에서도 태그로 쉽게 서식을 넣을 수 있어서, 에디터보다 훨씬 편합니다. 
## Markdown Cons 마크다운 단점
* `문법이 너무 단순하다.` 문법이 단순한 나머지 결국에는 HTML을 써야하는 경우가 생깁니다. 테이블 정렬 기능은 있지만, 이미지 정렬 기능이 없어서 HTML의 img 태그를 사용해야합니다. 태그에 클래스 지정등이 불가능하기 때문에, 클래스나 id를 지정하려면 HTML을 사용해야합니다.
* `표준이 없어 사용자마다 문법이 상이할 수 있다.` 문법이 단순하다 보니, 이러한 점을 해결하기 위해 확장문법들이 생겼고, 이러한 것들 때문에 한 곳에서 작동하는 마크다운 문서가 다른 곳에서는 잘 작동하지 않는 경우가 생기기도 합니다.

# Markdown Elements
## Table of contents 목차
[1. Headers 헤더](#1-headers-헤더)<br>
[2. Emphasis 강조](#2-emphasis-강조)<br>
[3. Blockquotes 인용](#3-blockquotes-인용)<br>
[4. Lists 목록](#4-lists-목록)<br>
[5. Backslash Escapes 백슬래쉬 이스케이프](#5-backslash-escapes-백슬래쉬-이스케이프)<br>
[6. Images 이미지](#6-images-이미지)<br>
[7. Links (Anchor) 링크](#7-links-anchor-링크)<br>
[8. Fenced Code Blocks 코드 블럭](#8-fenced-code-blocks-코드-블럭)<br>
[9. Task Lisk 체크 리스트](#9-task-lisk-체크-리스트)<br>
[10. Horizontal Rules 수평선](#10-horizontal-rules-수평선)<br>
[11. Emoji 이모티콘](#11-emoji-이모티콘)<br>
[12. Table 테이블](#12-table-테이블)<br>
[13. Line Breaks 줄바꿈](#13-line-breaks-줄바꿈)<br>
[14. Reference 참고 링크](#14-reference-참고-링크)<br>

## 1. Headers 헤더
* `#`으로 시작하는 텍스트.
* `#`은 하나부터 여섯개까지 가능.
* `#`이 늘어날때마다 제목의 스케일 낮아집니다.
* H1은 `===`로도 만들 수 있습니다.
* H2는 `---`로도 만들 수 있습니다.
### Syntax 마크다운 사용법 
    This is an H1
    ===
    This is an H2
    ---
    # This is an H1 
    ## This is an H2
    ### This is an H3
    #### This is an H4
    ##### This is an H5
    ###### This is an H6   
### Demonstration 실행결과
This is an H1<br>
===
This is an H2<br>
---
# This is an H1; 부(parts)에 사용<br>
## This is an H2; 장(chapters)에 사용<br>
### This is an H3; 페이지 섹션에 사용<br>
#### This is an H4; 하위 섹션에 사용<br>
##### This is an H5; 하위 섹션 아래의 하위 섹션에 사용<br>
###### This is an H6; 문단에 사용<br>

## 2. Emphasis 강조
* 기울여 쓰기(italic) : `*` 또는 `_`로 감싼 텍스트.
* 두껍게 쓰기(bold) : `**` 또는 `__`로 감싼 텍스트.
* 취소선 : `~~`로 감싼 텍스트.
* 이탤릭체와 두껍게를 같이 사용할 수 있습니다.
### Syntax 마크다운 사용법
      *This text will be italic*
      _This will also be italic_
      **This text will be bold**
      __This will also be bold__
      ~~This is canceled~~
      *You **can** combine them*
### Demonstration 실행결과
*This text will be italic*<br>
_This will also be italic_<br>
**This text will be bold**<br>
__This will also be bold__<br>
~~This is canceled~~<br>
*You **can** combine them*<br>

## 3. Blockquotes 인용
* `>`으로 시작하는 텍스트.
* `>`는 3개까지 가능합니다.
* `1개`는 인용문.
* `2개`는 인용문 안에 인용문.
* `3개`는 인용문 안에 인용문 안에 인용문.
### Syntax 마크다운 사용법
    As Grace Hopper said:
    > I’ve always been more interested in the future than in the past.    
    > This is a first blockquote.
    > > This is a second blockquote.
    > > > This is a third blockquote.
### Demonstration 실행결과
As Grace Hopper said:
> I’ve always been more interested in the future than in the past.
> This is a first blockquote.
> > This is a second blockquote.
> > > This is a third blockquote.

## 4. Lists 목록
### 4.1. Unordered lists 순서가 없는 목록
* `*`, `+`, `-` 를 이용해서 순서가 없는 목록을 만들 수 있습니다.
* 들여쓰기를 하면 모양이 바뀝니다.
### 4.2. Ordered lists 순서가 있는 목록
* 숫자를 기입하면 순서가 있는 목록이 됩니다.
* 들여쓰기를 하면 모양이 바뀝니다.
### Syntax 마크다운 사용법
    * Item 1
    * Item 2
      * Item 1
      * Item 2
        * Item 1
        * Item 2
     1. Item 1
     2. Item 2
     3. Item 3
       1. Item 1
       2. Item 2
       3. Item 3
         1. Item 1
         2. Item 2
         3. Item 3
### Demonstration 실행결과
* Item 1
* Item 2
    * Item 1
    * Item 2
      * Item 1
      * Item 2
1. Item 1
2. Item 2
3. Item 3
    1. Item 1
    2. Item 2
    3. Item 3
       1. Item 1
       2. Item 2
       3. Item 3
       
## 5. Backslash Escapes 백슬래쉬 이스케이프
* 특수문자를 표현할 때, 표시될 문자 앞에 `\`를 넣고 특수문자를 쓰면 됩니다.
* 주의할 점은 앞과 뒤에가 형식이 똑같이 백슬래쉬 뒤에 특수문자입니다. `감싸는 형태가 아닙니다.`
* 백슬래쉬는 아래의 특수문자를 표현할 수 있습니다.
* \ backslash, \ backtick, * asterisk, _ underscore, {} curly braces, [] square brackets,
() parentheses, # hash mark, + plus sign, - minus sign (hyphen), . dot, ! exclamation mark
### Syntax 마크다운 사용법
	\*literal asterisks\*
	\#hash mark\#
	\[squre brackets\]
### Demonstration 실행결과
\*literal asterisks\*<br>
\#hash mark\#<br>
\[squre brackets\]<br>

## 6. Images 이미지
* <img>로 변환됩니다.
* 링크와 비슷하지만 앞에 `!`가 붙습니다.
* 인라인 이미지 \![alt text](/test.png\)
* 링크 이미지 \![alt text](image_URL\)
* 이미지의 사이즈를 변경하기 위해서는 `<img width="OOOpx" height="OOOpx"></img>`와 같이 표현합니다.
### Syntax 마크다운 사용법
	![alt 토마토](/img/tomato.jpg)
	![alt Concrete Buildings](https://github.com/jinkyukim-me/open-tutorial/blob/master/img/concrete_building.jpg)
### Demonstration 실행결과
![alt 토마토](/img/tomato.jpg)
![alt Concrete Buildings](https://github.com/jinkyukim-me/open-tutorial/blob/master/img/concrete_building.jpg)

## 7. Links (Anchor) 링크
## 7.1. External Links 외부 링크 
	인라인 링크: [링크](http://example.com "링크 제목")
	url 링크: <example.com>, <example@example.com>; 꺽쇠 괄호 없어도 자동으로 링크를 사용
### Syntax 마크다운 사용법
	[Google](http://www.google.com "구글")
	[Naver](http://www.naver.com "네이버")
	[Github](http://www.github.com "깃허브")
	구글 www.google.com; 꺽쇠없음 
	네이버 <www.naver.com>; 꺽쇠있음 
	My mail <jinkyukim.dev@gmail.com>
### Demonstration 실행결과
[Google](http://www.google.com "구글")<br>
[Naver](http://www.naver.com "네이버")<br>
[Github](http://www.github.com "깃허브")<br>
구글 www.google.com <br>
네이버 <www.naver.com> <br>
My mail <jinkyukim.dev@gmail.com><br>
## 7.2. Internal Links 내부 링크 
	[보여지는 내용](#이동할 헤드(제목))
	괄호 안의 링크를 쓸 때는 띄어쓰기는 -로 연결, 영어는 모두 소문자로 작성
### Syntax 마크다운 사용법
	[1. Headers 헤더](#1-headers-헤더)
	[2. Emphasis 강조](#2-emphasis-강조)
	[3. Blockquotes 인용](#3-blockquotes-인용)
### Demonstration 실행결과
[1. Headers 헤더](#1-headers-헤더)<br>
[2. Emphasis 강조](#2-emphasis-강조)<br>
[3. Blockquotes 인용](#3-blockquotes-인용)<br>

## 8. Fenced Code Blocks 코드 블럭
* 간단한 인라인 코드는 텍스트를 앞뒤로 \`기호로 감싸면 됩니다.
* \`\`\` 혹은 ~~~ 코드.
* 첫 줄과 마지막 줄에 Back quote ( \` ) 또는 물결( ~ ) 3개 삽입.
* 코드가 여러 줄인 경우, 줄 앞에 공백 네 칸을 추가하면 됩니다.
* \`\`\` 옆에 언어를 지정해주면 syntax color가 적용됩니다.
### Syntax 마크다운 사용법
	```
	This is code blocks.
	```
	~~~
	This is code blocks.
	~~~
		4 spaces 
	```javascript
	function test() {
	 console.log("look ma’, no spaces");
	}
	```
### Demonstration 실행결과
```
This is code blocks.
```
~~~
This is code blocks.
~~~
	4 spaces
```javascript
function test() {
 console.log("look ma’, no spaces");
}
```

## 9. Task Lisk 체크 리스트
* 줄 앞에 `- [x]`를 써서 완료된 리스트 표시.
* 줄 앞에 `- [ ]`를 써서 미완료된 리스트 표시.
* 체크 안에서 강조 외에 여러 기능을 사용할 수 있습니다.
### Syntax 마크다운 사용법
	- [x] this is a complete item
	- [ ] this is an incomplete item
	- [x] @mentions, #refs, [links](),
	**formatting**, and <del>tags</del>
	supported
	- [x] list syntax required (any
	unordered or ordered list
	supported)
### Demonstration 실행결과
- [x] this is a complete item
- [ ] this is an incomplete item
- [x] @mentions, #refs, [links](),
**formatting**, and <del>tags</del>
supported
- [x] list syntax required (any
unordered or ordered list
supported)

## 10. Horizontal Rules 수평선
* \- 또는 * 또는 _ 을 3개 이상 작성.
* 단, -을 사용할 경우 header로 인식할 수 있으니 이 전 라인은 비워두어야 합니다.
### Syntax 마크다운 사용법
	* * *
	***
	*****
	- - -
	-------------------
### Demonstration 실행결과
* * *
***
*****
- - -
-------------------

## 11. Emoji 이모티콘
* 마크다운을 이용해 이모티콘을 표현가능.
* 깃허브도 적용가능.
* 더 많은 리스트는 아래의 사이트로 방문.
* www.emoji-cheat-sheet.com
### Syntax 마크다운 사용법
	GitHub supports emoji!
	:+1: :sparkles: :camel: :tada:
	:rocket: :metal: :octocat: 
### Demonstration 실행결과
GitHub supports emoji!
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat: 

## 12. Table 테이블
* 헤더와 셀을 구분할 때 3개 이상의 `-`(hyphen/dash) 기호가 필요합니다.
* 헤더 셀을 구분하면서 :(Colons) 기호로 셀(열/칸) 안에 내용을 정렬할 수 있습니다.
* 가장 좌측과 가장 우측에 있는 |(vertical bar) 기호는 생략 가능합니다.
### Syntax 마크다운 사용법
	테이블 생성

	헤더1|헤더2|헤더3|헤더4
	---|---|---|---
	셀1|셀2|셀3|셀4
	셀5|셀6|셀7|셀8
	셀9|셀10|셀11|셀12

	테이블 정렬

	헤더1|헤더2|헤더3
	:---|:---:|---: 
	Left|Center|Right 
	1|2|3
	4|5|6
	7|8|9
### Demonstration 실행결과
테이블 생성

헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

테이블 정렬

헤더1|헤더2|헤더3
:---|:---:|---: 
Left|Center|Right 
1|2|3
4|5|6
7|8|9

## 13. Line Breaks 줄바꿈
* `<br>`를 활용해서 줄바꿈을 할 수 있습니다.
### Syntax 마크다운 사용법
	Oh my my my oh my my my
	You got me high so fast <br>
	네 전부를 함께하고 싶어
	Oh my my my oh my my my <br>
	You got me fly so fast
	이제 조금은 나 알겠어 <br>
### Demonstration 실행결과
Oh my my my oh my my my
You got me high so fast <br>
네 전부를 함께하고 싶어
Oh my my my oh my my my <br>
You got me fly so fast
이제 조금은 나 알겠어 <br>

## 14. Reference 참고 링크
* [Matering Markdown](https://guides.github.com/features/mastering-markdown/)
* [마크다운 위키백과](https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)
* [존 그루버의 웹사이트](https://daringfireball.net/projects/markdown/)
