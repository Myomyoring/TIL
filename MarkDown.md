# 마크다운 (markdown)

## 마크다운이란?  
마크다운(Markdown)은 일반 텍스트 기반의 경량 `마크업 언어`다. 일반 텍스트로 서식이 있는 문서를 작성하는 데 사용되며, 일반 마크업 언어에 비해 **문법이 쉽고 간단한 것이 특징**이다. HTML과 리치 텍스트(RTF) 등 서식 문서로 쉽게 변환되기 때문에 응용 소프트웨어와 함께 배포되는 README 파일이나 온라인 게시물 등에 많이 사용된다. - 위키백과   
**즉, 문서를 쉽게 작성하기 위해 만들어진 마크업 언어이다. HTML로 변환가능!**
<br/><br/>
*상세하게 보고싶다면 참고(영어)
>공식 사이트   
>https://daringfireball.net/projects/markdown/   

>마크다운 가이드   
>https://www.markdownguide.org/

<br>

***
<br>

## [마크다운 장점]
1. 문법이 간결 함
2. 에디터없이 어디서나 작성 가능
3. 텍스트로 저장되어 용량도 적고, 보관에 용이
4. 다양한 포맷으로 변경 가능
5. 지원하는 프로그램과 플랫폼 범위가 확대
   
## [마크다운 단점]
1. 표준이 없음
2. 모든 HTML의 문법을 대신하지 못함
3. 표준이 없어서 도구에 따라 변환방식이나 출력 등 생성물이 다름

<br>

### 깃허브에서 적용되지 않는 문법 (html문법으로 사용해야 함)
- 밑줄(underline) 
- 위첨자, 아래첨자

<br>

***
<br>

# 마크다운 문법
<br/>

## <제목(Headers)>
<br/>
[1~8번 output]
<br><br>

1.header   
===
2.header
---
# 3.headers1
## 4.headers2
### 5.headers3
#### 6.headers4
##### 7.headers5
###### 8.headers6

<br/>
    [1~8번 input]

    1.header   
    ===
    2.header
    ---
    # 3.headers1
    ## 4.headers2
    ### 5.headers3
    #### 6.headers4
    ##### 7.headers5
    ###### 8.headers6

- `===`로 `H1`, `---`로 `H2` 헤더를 만들 수 있음 (===와 #, ---와 ##은 동일하게 설정)
- `=`와 `-`는 각각 `2개 이상` 사용하면 **헤더로 설정** 됨
- #은 `1개부터 6개`까지 사용해서 헤더를 만들 수 있음

---
<br>

## <줄바꿈(Line Breaks)>
<br>
[output] <br><br>   

1


엔

터

쓰

기

2<br>
b<br>
r<br>
쓰<br>
기<br>

3   
스   
페   
이   
스  
바    
세   
번   
쓰   
기   

<br>
[input]   
    
    1

    엔

    터

    쓰

    기

    2<br>
    b<br>
    r<br>
    쓰<br>
    기<br>

    3   
    스   
    페   
    이   
    스  
    바    
    세   
    번   
    쓰   
    기 

- 엔터 2번 (1번하면 띄어쓰기로 설정) 대신 이건 간격이 벌어짐 (행 줄바꿈)
- \<br> 혹은 \<br/> , 한 줄의 공백을 만들 때 자주 씀 (문장 줄바꿈)
- 세칸 이상 띄어쓰기 (글자/띄어쓰기3번/) (행 줄바꿈)
---
<br>

## <수평선(Horizontal Rules)>
<br>
[output]<br><br>

--- 
***
___
- - -
* * *
<hr>

<br>
[input]

    --- 
    ***
    ___
    - - -
    * * *
    <hr>

- -바 3개 이상 (헤더나 목록으로 설정될 수 있어서 후순위 사용)
- *별 3개 이상
- _언더바 3개 이상
- \<hr> 혹은 \<hr/>

---
<br>

## <강조(Emphasis)>
<br>
[output]<br><br>

*기울이기*   
_기울이기_   
**굵게굵게**   
__굵게굵게__    
~~취소할래~~   
*섞어서 <u>예쁘게</u> **강조해서** ~~기깔나게~~ 써보자*   

<br>
[input]

    *기울이기*   
    _기울이기_   
    **굵게굵게**   
    __굵게굵게__   
    ~~취소할래~~   
    *섞어서 <u>예쁘게</u> **강조해서** ~~기깔나게~~ 써보자*    

- 이탤릭체(italic) : *또는 _로 감싸기
- 볼드체(bold) : **또는 __로 감싸기
- 취소선 : ~~로 감싸기

---
<br>

## <인용(Blockquotes)>
<br>
[output]<br><br>

> 인용인가요
> > 민용인데요
> > > 인용이 맞습니다  
> 아시겠죠?
>   
> > 잘 알겠습니다   
> 
> 네

<br>
[input]

    > 인용인가요
    > > 민용인데요
    > > > 인용이 맞습니다  
    > 아시겠죠?
    >   
    > > 잘 알겠습니다   
    > 
    > 네

- `>` 일명 꺽쇠로 표기
- 인용구 안에는 다른 마크다운 요소를 넣을 수 있음
- 인용구는 `3개까지` 중첩으로 사용 가능 
- 꺽쇠3개짜리 인용구로 쓰다가 다음 단락에 '이어서' 쓰면 꺽쇠가 몇개 건 마지막 인용구에 이어짐
- 끊고 싶으면 꺽쇠로 공백줄 만들고 작성하기 

---
<br>

## <목록(Lists)>
<br>

### *순서가 없는 목록(Unordered lists)   
[output]<br><br>

- 할머니
  + 엄마
    * 딸
      - 증손녀
        - 현손녀


[input]

    - 할머니
      + 엄마
        * 딸
          - 증손녀
            - 현손녀

- -바 +더하기 *별로 표기
- 하위로 갈 때 때 탭(tab)으로 들여쓰면 됨 (ex: (들여쓰기)+)
- -,+,* 섞어써도 됨

<br>

### *순서가 있는 목록(Ordered lists)   
[output]<br><br>

3. 일번 나오세요
2. 저요
1. 당신 2번이잖아
2. 앗 들킴

   1. 진짜 아닌데요
      1. 방금은 맞다며? 
         1. 집 보내주세요


<br>
[input]

    3. 일번 나오세요
    2. 저요
    1. 당신 2번이잖아
    2. 앗 들킴

      1. 진짜 아닌데요
         1. 방금은 맞다며? 
            1. 집 보내주세요

- `숫자`와 `.`점으로 작성
- 시작번호 기준으로 그 다음에 어떤 번호를 써도 내림차순으로 정의
- 하위로 갈 때 때 탭(tab)으로 들여쓰면 새로운 번호 시작 됨 (ex: (들여쓰기)+)

----
<br>

## <인라인코드(Inline Code)>
<br>
[output]<br><br>

그것은 `분명히 거기 있었을 것` 이다.
```
아니요 없었는데요
```
```java
public class Main {
  public static void main(String[] args){
     System.out.println("Hello MarkDown!!");
   }
 }
```

<br>
[input]

    그것은 `분명히 거기 있었을 것` 이다.
    ```
    아니요 없었는데요
    ```

    ```java
    public class Main {
      public static void main(String[] args){
        System.out.println("Hello MarkDown!!");
      }
    }
    ```

- \` `백틱`으로 감싸서 표기
- 위아래로 ```3개 씩 감싸면 블럭으로 만들어짐
- 코드 하이라이트를 사용하고 싶을 경우 `위쪽 백틱에 언어명`을 작성하면 됨
- `4칸이상 들여쓰기`(tab키)시 코드블럭 생성 가능

----
<br>

## <링크(Link, Anchor)>
<br>
[output]<br><br>
   
[Naver](https://www.naver.com "네이버")   
https://www.naver.com/   
naver@naver.com   
[네이버로 이동하려면 여기 눌러!](https://www.naver.com/)

<br>
[input]
   
    [Naver](https://www.naver.com "네이버")   
    https://www.naver.com/   
    naver@naver.com   
    [네이버로 이동하려면 여기 눌러!](https://www.naver.com/)

- 이메일이나, 주소는 자동으로 연결 됨

----
<br>

## <이미지(Image)>
<br>

[output]<br><br>

![당신의 선택은](https://cdn.pixabay.com/photo/2012/04/28/17/11/people-43575_1280.png)  
![멜크](https://cdn.pixabay.com/photo/2016/11/24/08/37/santa-1855681_1280.jpg "시원쓰")
[![링크스마일](https://cdn.pixabay.com/photo/2015/11/13/10/07/smiley-1041796_1280.jpg)](https://github.com/Myomyoring)

<br>
[input]

      ![당신의 선택은](https://cdn.pixabay.com/photo/2012/04/28/17/11/people-43575_1280.png)  
      ![멜크](https://cdn.pixabay.com/photo/2016/11/24/08/37/santa-1855681_1280.jpg "시원쓰")
      [![링크스마일](https://cdn.pixabay.com/photo/2015/11/13/10/07/smiley-1041796_1280.jpg)](https://github.com/Myomyoring)
      
      
- 이미지에 마우스 오버하면 나오는 문구는 이미지링크 뒤에 ""를 붙여주면 됨
- 이미지 클릭 시 링크를 넣고 싶으면 \[!\[이미지이름](이미지링크)](연결할링크) 적어주면 됨 

--- 
<br>

## <테이블(Table)>
<br>

[output]<br><br>

| 좌측정렬 | 중앙정렬 | 우측정렬 |
:---|:---:|---:|
 정렬이 되는 걸까요?? 안되는 걸까요? | 그럴껄요?그런다고 했잖아요 | 아니면 이거 만든사람 나오라 그래 

<br>
[input]

    | 좌측정렬 | 중앙정렬 | 우측정렬 |
    :---|:---:|---:|
     정렬이 되는 걸까요?? 안되는 걸까요? | 그럴껄요?그런다고 했잖아요 | 아니면 이거 만든사람 나오라 그래
- `|`으로 셀구분을 줄 수 있음, 가장 좌측, 우측 |은 생략 가능
- `:`콜론으로 **정렬**이 가능하다
- \---바 3개로 헤더와 셀을 구분 함

---
<br>

## <체크박스(Check Box)>
<br>

[output]<br><br>

- [ ] 명상하기
* [x] ~~밥 먹기~~
+ [x] 잠자기

<br>
[input]

    - [ ] 명상하기
    * [x] ~~밥 먹기~~
    + [x] 잠자기

- `-`, `*`, `+` 뒤에 띄어쓰기+대괄호로 표기
- 대괄호안에 **띄어쓰기 1칸**이면 `빈 체크박스`, **x**면 `체크된 체크박스`

---
<br>

## <이모지(Emoji)>
<br>

[output]<br><br>

💗   
:smile:

<br>
[input]

      💗   
      :smile:

- 맥은 `control` + `command` + `space`, 윈도우는 `윈도우키` + `.` 버튼 누르면 이모지 창 나옴
- 이모지를 그냥 복사 붙여넣기 해도 됨
- ::콜론 두개 사이에 이모지 지정어를 넣어주면 이모지로 출력

---
<br>

## <각주(Footnote)>
<br>

[output]<br><br>

첫째각주[^1]   
둘째각주[^2]

[^1]:첫째미주
[^2]:둘째미주

<br>
[input]

    첫째각주[^1]   
    둘째각주[^2]

    [^1]:첫째미주
    [^2]:둘째미주

- 대괄호안에 ^+숫자로 각주를 달고, 아래에 미주를 추가 할 수 있음

---
<br>

## <수식(Mathematical Expression)>
<br>

[output]<br><br>

$수식 = (\alpha + \beta)^2 = a^2 min_a$

$$가운데 정렬 수식 =  (\alpha + \beta)^2 = a^2 min_a$$

$\\슬래시와빨강글자어디에쓰는가$

$x$축으로 $y$만큼 이동

$
2^2\\
2_2
$

$
띄어 쓰기\\
띄어\,쓰기\\
띄어\;쓰기\\
띄어\quad쓰기\\
$

$x\times x=x$

$2\sqrt 2 \over 5+2$

$\frac{2\sqrt2}5+2$

$\frac{2\sqrt2}{5+2}$

<br>
[input]


    $수식 = (\alpha + \beta)^2 = a^2 min_a$

    $$가운데 정렬 수식 =  (\alpha + \beta)^2 = a^2 min_a$$

    $\\슬래시와빨강글자어디에쓰는가$

    $x$축으로 $y$만큼 이동

    $
    2^2\\
    2_2
    $

    $
    띄어 쓰기\\
    띄어\,쓰기\\
    띄어\;쓰기\\
    띄어\quad쓰기\\
    $

    $x\times x=x$

    $2\sqrt 2 \over 5+2$

    $\frac{2\sqrt2}5+2$

    $\frac{2\sqrt2}{5+2}$

- `$`수식`$` 달러 사이에 수식을 써주면 됨
- `$$`수식`$$` 달러 두 개를 쓰면 **가운데정렬** 됨
- 수식내에서 위첨자, 아래첨자 가능
- 수식내에서 `\\`는 `줄바꿈`
- `\,` =  1번 띄어쓰기, `\;` = 2번 띄어쓰기, `\quad` = 4번 띄어쓰기
- 수식내에서 곱하기 문자는 `\times` 로 표기
- 분수는 `\over` 과 `\frac` 로 사용, \over은 좌우 기준, \frac은 좌괄호는 분자 우괄호는 분모이나 2문자 이상의 경우 {}중괄호로 묶어주기

---

## 참고하면 좋을 사이트
<br>

- [이모지 참고 : 인파님 블로그](https://inpa.tistory.com/entry/MarkDown-%F0%9F%93%9A-Emoji-%EC%9D%B4%EB%AA%A8%ED%8B%B0%EC%BD%98-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0)
- [수식 참고 : d2h10s님 벨로그](https://velog.io/@d2h10s/LaTex-Markdown-%EC%88%98%EC%8B%9D-%EC%9E%91%EC%84%B1%EB%B2%95)
- [html테이블을 markdown테이블로 변환 : Tableconvert](https://tableconvert.com/ko/html-to-markdown)
