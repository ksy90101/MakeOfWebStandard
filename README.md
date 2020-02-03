# [\[groom\]\[웹퍼블리싱 실습\] 웹 표준 사이트 만들기](https://edu.goorm.io/learn/lecture/16941/%EC%9B%B9%ED%8D%BC%EB%B8%94%EB%A6%AC%EC%8B%B1-%EC%8B%A4%EC%8A%B5-%EC%9B%B9-%ED%91%9C%EC%A4%80-%EC%82%AC%EC%9D%B4%ED%8A%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0/info)

## 강의 소개

- groom 사이트에 있는 웹퍼블리싱 강의를 직접 실습하고 필요한 내용을 정리했습니다.

- HTML 태그와 CSS 속성에 대한 자세한 설명은 강사님이 정리 해놓으신 레퍼런스에서 찾아서 링크 걸어놓았습니다.
자세한 내용들은 링크에 들어가서 보시면 훨씬 이해 하시기 좋으실꺼 같습니다.

- [제작한 포트폴리오 사이트 dothome Pages](http://ksy90101.dothome.co.kr/web/)

- [제작한 포트폴리오 사이트 Github Pages](https://ksy90101.github.io/MakeOfWebStandard/web/)

- 직접 실습한 코드들은 [Github Repository](https://github.com/ksy90101/MakeOfWebStandard)에 있습니다.

- [강의자 webstroyboy Blog](https://webstoryboy.co.kr/)

## 1. Layout01

- [layout01 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout01.html)

- HTML 요소(Content Element)
    - meta, self-closing, block, inline으로 분류
    - block, inline 두개의 구조를 구분을 잘 해야 함.
    - block 구조는 박스라고 생각하면 되며, inline 구조는 텍스트라고 생각하면 쉬움.
    - block 구조는 위에서 아래로 태그들이 쌓이는 것이라고 생각하면 됨.
    - inline 구조는 왼쪽에서 오른쪽으로 배치된다고 생각하면 됨.
    
- [div 태그](https://webzz.tistory.com/264)
    - 문서의 섹션을 만들거나 영역을 나눌때 사용
    - 시맨틱한 태그의 활용이 절적하지 않은 경우에 사용함.
    - block 요소를 그룹화 한다고 생각하면 좋음.
    
- [float 속성](https://webzz.tistory.com/452)
    - block 요소의 정렬 상태를 설정
    - none(기본값), left, right 속성값을 가지고 있음.
    - float을 쓴 블록요소는 height값을 0으로 인식하기 때문에 깨지는 현상이 발생
        - 가장 기초적인 해결 방법은 깨진 블록 요소에 float:left를 똑같이 주는 방법이다.

- [margin 속성](https://webzz.tistory.com/490)
    - 바깥쪽 여백을 설정
    - 속성값 중에 auto를 이용하면 가운데 정렬을 할 수 있음
    
- [text-transform 속성](https://webzz.tistory.com/544)
    - 텍스트를 대문자나 소문자로 변경
    - uppercase, lowercase, capitalize(첫글자만 대문자) 3개의 속성값이 존재


- [text-align 속성](https://webzz.tistory.com/534) 
    - 텍스트 정렬 방식을 설정

- [line-height](https://webzz.tistory.com/485)
    - 문장과 문장 사이의 간격을 설정
    - 텍스트가 한줄일때, 세로 가운데 정렬을 하기 위해 감싸고 있는 블록의 높이값과 똑같이 즐때 사용
    - 한줄일때만 가능하며, 두줄 이상일 경우에는 세로 가운데 정렬이 안됨
    
## 2. layout02

- [layout02 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout02.html)

- [clear 속성](https://webzz.tistory.com/424)
    - float요소의 성질을 차단
    - float을 쓴 블록요소는 height값을 0으로 인식하기 때문에 깨지는 현상이 발생했는데, 그걸 해결할 수 있는 방법중 하나

## 3. layout03

- [layout03 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout03.html)

## 4. layout04

- [layout04 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout04.html)

## 5. layout05

- [layout05 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout05.html)

- [\* 선택자](https://webzz.tistory.com/662)
    - 모든 선택자에게 같은 값을 넣어줌
    - 모든 태그들은 각자 가지고 있는 고유 속성들이 있음. 그 속성들을 초기화 시킬때 사용함.(예를 들면, margin / padding)
    - 그러나 전체 선택자는 실무에서 잘 사용하지 않음. 그냥 있다는 것만 알고 계시면 좋음.
    
- 부모와 자식의 속성값이 똑같다면, 생략이 가능함.(중복코딩 피하기!)
    - 예를들어 부모의 높이가 100px이고, 자식의 높이가 100px이면, 자식 높이는 생략 가능
    
- width값의 기본값은 100%이기때문에 생략가능

## 6. layout06

- [layout06 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout06.html)

- inherit 속성값
    - 부모의 속성값을 상속받는다는 의미

- 코드 간략화
    - 최대한 코드가 중복되는 것들은 하나의 클래스를 생성해서 모아두는 것이 좋음

## 7. layout07

- [layout07 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout07.html)

- 주석을 적어주면서, 남이 코드를 봤을때 최대한 이해를 도와야 하며, 선택자명을 잘 적어준다면 주석도 최소화 할 수 있음.

## 8. layout08

- [layout08 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout08.html)

- [파일질라](https://filezilla-project.org/)

- Intelli J 웹서버 접근(Remote Host) -> 사용법 차후 포스팅

- [!doctype html](https://www.w3schools.com/tags/tag_doctype.asp)
    - html5 버전에 대해 웹 브라우저에게 알려주는 것
    - html 태그 앞에 먼저 선언해야 함.

- [html 태그](https://webzz.tistory.com/282)
    - 웹 문서의 최상위 요소 문서의 루트를 나타내며, 다른 모든 요소들은 html 태그의 자식 요소이여야 함.
    - 화면 판독에 필요한 언어를 설정해야 하며, 이 기능이 없으면 화면 판독기가 운영체제에 언어를 기본언어로 설정하여 잘못된 언어를 표현할 수도 있음
    - lang 속성으로 언어를 설정합니다. (한국어 "ko", 영어 "en")
    
- [head 태그](https://webzz.tistory.com/278)
    - 제목과 스크립트, 스타일 시트, 메타 정보 등을 제공
    - 화면에 보이지 않는 정보들을 넣음
    
- [meta 태그](https://webzz.tistory.com/300)
    - 웹 문서에 대한 정보를 제공
    - author(제작자), charset(언어셋), description(사이트에 대한 설명), keywords(사이트에 대한 키워드) 등등에 대해 정의
    - 자세한 내용은 위의 링크에서 확인

- [link 태그](https://webzz.tistory.com/293)
    - 외부 파일을 연결할 때 설정
    - 보통 CSS를 연결할 때 사용함.
    - 외부 스크립트 파일을 연결할때는 \<script\> 태그를 사용함.(헷갈리지 말것!)

## 9. layout9

- [layout09 소스코드](https://github.com/ksy90101/MakeOfWebStandard/blob/master/layout09.html)

## 10. 스킵메뉴

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- 웹 접근성은 모든 사람이 정보통신 기기나 서비스를 손쉽게 활용할 수 있게 하는 것이 목적이다.

- 우리나라는 2013년 웹 접근성이 의무화 됨.

- 데스크톱 웹사이트뿐만 아니라 모바일 웹사이트도 웹접근성 지침이 모두 존재

- 웹표준 및 웹접근성 관련 참고사이트
    - [웹접근성 연구소](https://www.wah.or.kr:444/index.asp)
    - [네이버 웹표준 널리](https://nuli.navercorp.com/)
    - [다음 웹표준 다룸](http://darum.daum.net/)
    
- 웹접근성에 따라 스킵메뉴를 만들어 줘야 함. (tab key를 누르면, 스킵메뉴가 보임)

- 링크값에 클래스값은 먹히지 않지만, 아이디 값은 사용 가능합니다.(해당 태그로 이동할려고 할때) 따라서 아이디는 항상 중복이 되지 않도록 사용하는 것이 좋습니다.

- [position 속성](https://webzz.tistory.com/528)
    - 요소의 위치를 설정합니다.
    - static : 기본값
    - absolute : 절대 위치
    - relative : 상대 위치
    - fixed : 고정 위치
    - [참고자료](https://developer.mozilla.org/ko/docs/Web/CSS/position)
    
- [\<a\> 태그](https://webzz.tistory.com/229)
    - 하이퍼 링크를 정의합니다.
    - 인라인 구조 중 하나입니다.
    - a(nchor)는 뜻으로 닻이라는 뜻입니다.
    
- [text-decoration 속성](https://webzz.tistory.com/536)
    - 글자 라인 속성을 정의합니다.
    - 밑줄(underline)이나 취소선(line-through) 등을 적용 시킵니다.
 
- [:hover 선택자](https://webzz.tistory.com/667)
    - 링크 위에 마우스를 올려 놓았을 경우
    
- [:active 선택자](https://webzz.tistory.com/667)
    - 링크가 활성화되었을 경우
    
- [:focus 선택자](https://developer.mozilla.org/ko/docs/Web/CSS/:focus)
    - 사용자가 요소를 클릭하거나 탭하거나 키보드의 Tap 키로 요소를 선택할때

# 11. 헤더 배경 & 메뉴

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [상대경로 vs 절대경로](https://88240.tistory.com/122)
    - 절대경로란 웹페이지나 파일이 가지고 있는 고유한 경로를 말한다.
    - 상대경로란 현재 위치한 곳을 기준으로 해서 경로를 정하는 것이다.
        - / : 루트
        - ./ : 현재 위치
        - ../ : 현재 위치의 상단 폴더

- [background : url()](https://webzz.tistory.com/380)
    - 주소를 설정하여 이미지를 보여줍니다.
    - 처음에 이미지가 반복되어 있습니다.

- [background-repeat](https://webzz.tistory.com/383)
    - background-img의 반복 여부를 설정
    - repeat : x축과 y축으로 반복 설정
    - repeat-x : x축으로 반복 설정
    - repeat-y : y축으로 반복 설정
    - no-repeat : 반복하지 않음

- [background-position](https://webzz.tistory.com/382)
    - background-img의 위치 영역을 설정
    
- [background](https://webzz.tistory.com/375)
    - background가 붙은 모든 속성값을 한번에 정의 할 수 있습니다.
    
- [padding 속성](https://webzz.tistory.com/517)
    - 안쪽 여백을 설정
    - 순서대로 4개를 적으면, 위쪽, 오른쪽, 아래쪽, 왼쪽 순으로 적을수 있음
    - inline구조의 padding값은 위아래는 적용되지 않고 양옆만 적용됩니다.
    
- [display 속성](https://webzz.tistory.com/442)
    - 요소의 성질을 정의함.
    - inline을 block을 block을 inline으로 서로 변경 가능합니다.
    - inline-block : 인라인 성질 + 블록 성질
    - inline, block 속성값 말고도 많은 속성값이 존재함.
    
- 부모와 자식 관계로 해서 CSS 선택자를 적는 것이 CSS를 봐도 구조를 알 수 있기 때문에 훨씬 더 좋음

## 12. 헤더 타이틀 & 웹 폰트

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [font-family](https://webzz.tistory.com/454)
    - 폰트 종류를 설정
    - 폰트명이 한글이거나 여러 단어인 경우는 큰따옴표("")로 설정
    - 쉼표(,)를 통해 여러개의 폰트를 설정 가능합니다.
    - 가장 먼저 쓴 폰트부터 적용이 되며, 폰트가 설치가 되어 있지 않는다면 다음 적은 폰트로 넘어갑니다.
    - 속성값에 있는 폰트가 모두 없다면 브라우저 기본 폰트로 설정이 됩니다.

- [웹폰트](https://www.opentutorials.org/course/2418/13372)
    - 사용자가 가지고 있지 않은 폰트를 웹페이지에서 사용 할 수 있는 방법
    - 구글에서 제공하는 무료 웹폰트 서비스 google fonts 등이 있습니다.
    
- [\<br\> 태그](https://webzz.tistory.com/247)
    - 줄바꿈할때 사용합니다.
    
- [font-weight: normal](https://webzz.tistory.com/460)
    - 폰트 두깨를 설정하는데, 기본값으로 설정한다는 의미

## 13. 헤더 아이콘 수정

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- 이미지를 표현하는 방법
    1. img 태그로 표현(의미가 있을 때)
        - alt 속성으로 대체 문자를 표현할 수 있음 따라서 의미가 있을때 사용함
        - [img 태그 자세히 보기](https://webzz.tistory.com/285)
    2. background 속성으로 표현(의미가 없을 때)
        - [background-image 속성 자세히 보기](https://webzz.tistory.com/380)
    3. 최근 웹사이트는 background 속성을 이용하여 이미지를 표현하며, 가상으로 대체 문자를 만들어줌(IR 효과)
    왜냐하면 웹 접근성을 만족시켜야 하기 때문에 인데, 왜 background 속성을 사용하는 이유는~~~~ 이미지 스프라이트를 사용하여 서버 요청을 최소화 하기 위해서입니다.
        - [IR 효과](http://ui.daum.net/convention/css/css_ir)
        - [이미지 스프라이트](http://tcpschool.com/css/css_basic_imageSprites)

- IR효과 태그

````
/* 의미있는 이미지의 대체 텍스트를 제공하는 경우*/
. ir_pm {
    display: block;
    overflow: hidden;
    font-size: 0;
    line-height: 0;
    text-indent: -9999px;
}

/* 의미있는 이미지의 대체 텍스트로 이미지가 없어도 대체 텍스트를 보여주고자 할 때 */
. ir_wa {
    display: block;
    overflow: hidden;
    position: relative;
    z-index: -1;
    width: 100%;
    height: 100%;
}

/* 대체 텍스트가 아닌 접근성을 위한 숨김 텍스트를 제공 할 때 */
.ir_su {
    overflow: hidden;
    position: absolute;
    width: 0;
    height: 0;
    line-height: 0;
    text-indent: -9999px;
}
````

- [z-index](https://webzz.tistory.com/563)
    - 요소의 위치가 겹칠 경우 순서를 정의
    - 음수도 설정 가능
    - 99999까지만 설정 가능
    - z-index를 적용하지 않은 경우 CSS 우선순위에 따라 나중에 설정한 속성이 위로 올라옴
    
- [text-indent](https://webzz.tistory.com/540)
    - 문단 들여쓰기 속성 설정
    
- [overflow](https://webzz.tistory.com/514)
    - 지정한 영역에 요소들이 벗어났을 때 속성을 설정
    - hidden값은 값을 안보이게 하는 것

- [Web Developer 크롬 확장 프로그램](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?utm_source=chrome-ntp-icon)
    - 유효성 검사하는 프로그램

## 14. 전체 메뉴 수정

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [ol 태그](https://webzz.tistory.com/306)
    - Order List로써 순서가 있는 목록형 태그
    
- [li 태그](https://webzz.tistory.com/292)
    - List Item으로 목록의 항목을 나타냄
    
- [list-style 속성](https://webzz.tistory.com/486)
    - 목록 스타일 속성을 설정
    - type(유형), position(위치), image(이미지)를 설정
    
- ['>' 선택자](https://webzz.tistory.com/663)
    - 자식선택자로, 첫번째 자식만 선택함
    
- [' ' 선택자](https://webzz.tistory.com/663)
    - 하위 선택자로 모든 자식을 선택함

- float: left로 인한 영역깨짐(height : 0) 방지법
    1. 깨지는 영역에 똑같이 float: left를 사용
        - 모든 박스에 float: left를 사용하게 되기 때문에 권장하지 않습니다.
    2. float의 성징을 차단하는 clear: both 사용
        - 박스 구조가 복잡해졌을때 어떤 영역이 깨졌는지 찾기 어렵기 때문에 사용하는데 권장하지 않습니다.
    3. float을 사용한 상위박스한테 overflow: hidden을 사용
        - 100%좋지는 않지만, 현재는 우리 기준으로 제일 많이 사용함
        - 내가 지정한 영역외에는 안보이게 된다보니, height: 0이 안됨
        - 그러나, 2단메뉴를 사용할때는 사용을 하지 못함
    4. clearfix를 사용
        -[clearfix란?](https://takeuu.tistory.com/60)
        - 가장 좋은 방법!

- [:last-child 선택](https://webzz.tistory.com/666)
    - ie9부터 사용 가능
    - 마지막 자신만 선택

## 15. 전체 타이틀

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- position : absolute;
    - 항상 기준점이 필요하기 때문에, 기준점이 되는 곳에 position: relative를 적어줘야함.

- [letter-spacing](https://webzz.tistory.com/484)
    - 글자 사이의 간격을 설정

## 16. 전체 배너

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [:nth-child() 선택자](https://webzz.tistory.com/666)
    - ie9부터 적용
    - 자식을 직접 선택할 수 있는 선택자
    
## 17. 컨텐츠 레이아웃

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

## 18. 게시판 1

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- 한줄효과 CSS 속성
````
overflow: hidden; text-overflow: ellipsis; white-space: nowrap;  
````

- a링크에 title을 이용하여 접근성을 위해 적어두는것이 좋음
    - 마우스 올려놓을시, 창으로 title에 적은 글이 나옴.

## 19. 게시판 2

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

## 20. 게시판 3

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

## 21. 마우스오버 효과 1

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [em 태그](https://webzz.tistory.com/267)
    - 텍스트를 강조하는 데 사용
    - 시각적으로 기울임꼴로 표시가 됩니다.

- [strong 태그](https://webzz.tistory.com/329)
    - 텍스트의 중요성, 심각성, 긴급성의 의미를 가지고 있으며 텍스트는 시각적으로 굵게 표현

- [visibility 속성](https://webzz.tistory.com/557)
    - 요소를 보이지 않게 정의함
    - visible(기본값) / hidden(보이지 않게 함(영역은 유지)), collapse(테이블 요소를 보이지 않게 하며 영역 제거)
    
## 22. 마우스오버 효과 2

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- 미리 만들어놓은 구성요소를 재사용 하는 것이 좋음. 그러나 margin이나 padding같은 경우를 다르게 줘야 할 경우가 있을 수 있음.
그럴때는 reset.css에 미리 클래스를 만들어 놓는 것이 줗음 그러면 그 클래스만 넣으면 margin이 적용되기 때문이다.

- [!important](https://www.codingfactory.net/10372)
    - CSS는 같은 속성을 여러번 정의했을때 우선순위에 따라 값이 적용됩니다.
    - 혹시 가장 높은 우선순위로 속성을 적용시키고 싶다면, 
    > property(속성): value(속성값) !important
                                  
    처럼 적어주면 된다.

## 23. 탭메뉴

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- 콘텐츠 요소를 보이지 않게 하는 방법
    - display:none -- display: block ==> 영역 제거
    - visibility: hidden -- visibility: visible ==> 영역은 유지
    - opacity: 0 -- opacity: 1 (영역 유지)
    - width:0; height:0; overflow:hidden (영역 제어 가능)

- border가 위아래로 2개씩 있다면, 한줄로 보이게 하는 방법 중 하나는 위치에 맞게 margin을 -1px을 주는 방법이다.

## 24. 게시판 4

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

## 25. 갤러리

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

## 26. 로그인

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [form 태그](https://webzz.tistory.com/274)
    - 웹 서버에 정보를 제공하는 유형을 정의합니다.
    - action속성과 method 속성이 중요합니다.
    - action속성이란 폼 양식이 제출될 때 데이터가 전달 혹은 받을 경로를 설정합니다.
    - method속성이란 전송 방식을 설정하며 get방식과 post방식이 있습니다.
    
- [fieldset 태그](https://webzz.tistory.com/269)
    - 폼 요소의 그룹 내부 영역을 설정합니다.
    - 폼 요소의 여러 컨트롤과 label을 그룹화 하는데 사용합니다.
    
- [legend 태그](https://webzz.tistory.com/291)
    - fieldset 요소의 영역 제목을 정의합니다.
    
- [input 태그]()

- [label 태그](https://webzz.tistory.com/290)
    - input 요소의 제목을 설정하며 태그를 서로 연결합니다.
    
- [vertical-align 속성](https://webzz.tistory.com/556)
    - 상하 정렬 방식을 설정합니다.
    - inline구조에서만 적용이 되며, 블럭 구조에서는 정렬이 되지 않습니다.
    - 글씨와 이미지 및 글씨와 input의 정렬상태가 맞지 않는다면, 이미지 요소 및 input에게 vertical-align을 주어야 합니다.

## 27. 팝업

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

## 28. 푸터 & W3C 수정

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [address 태그](https://webzz.tistory.com/232)
    - 웹 페이지의 연락처 정보를 설정하는 시맨틱 태그입니다.
    
- [::before 가상 선택자](https://webzz.tistory.com/665)
    - 문단 시작 부분에 요소를 추가하는 선택자

## 29. 전체 메뉴 스크립트

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- jQuery 란?
    - 자바스크립트 라이브러리를 이용해 만든 언어로 자바스크립트를 좀 더 효율적이고 쉽게 이용할 수 있도록 제작된 라이브러리입니다.
    
- 이용방법(CDN 방식)
    - [jQuery Google CDN](https://developers.google.com/speed/libraries#jquery)
    - 위의 사이트에서 버전에 맞게 script를 추가해주면 됩니다.
        
- script 태그 사용시 type을 지정해야 하는데, HTML5부터는 생략이 가능합니다.

- [intelli J jQuery 자동완성 사용](https://stackoverrun.com/ko/q/10211240)

- [event.preventDefault()]()

- [jQuery Selectors](https://www.w3schools.com/jquery/jquery_selectors.asp)
    - jQuery 요소 선택자는 이름, 클래스, 유형, 속성, 속성 값 등을 기반으로 HTML 요소를 선택합니다.
    - 달러 기호화 괄호로 시작합니다. 
    - 문법 : $()

- [click 이벤트](https://www.w3schools.com/jquery/event_click.asp)
    - 요소를 클릭하면 click 이벤트를 발생시킵니다.
    
- [css()](https://www.w3schools.com/jquery/jquery_css.asp)
    - css의 속성 값을 반환하기 위해 사용하는 구문입니다.
    - css("속성", "속성값") 형태로 사용합니다.

- [show & hide](https://www.w3schools.com/jquery/jquery_hide_show.asp)
    - show() 메소드는 HTML 요소를 표시 하는 메소드입니다.
    - hide() 메소드는 HTML 요소를 숨기는 메소드입니다.
    - 둘다 매개 변수는 speed(속도)와 callback(메소드 완료 후에 실행될 함수)를 가집니다.
    
- [fadeIn()](https://www.w3schools.com/jquery/eff_fadein.asp)
    - 요소에 대한 불투명도를 설정하여 페이딩 효과로 점차 변화시킵니다.

- [slideDown & slideUp & slideToggle()](https://www.w3schools.com/jquery/jquery_slide.asp)
    - slideDown()메소드는 요소를 아래로 슬라이드 하는데 사용합니다.
    - 매개 변수는 speed(속도)와 callback(슬라이딩이 완료된 후에 실행될 함수)를 가집니다.

- [toggle()](https://www.w3schools.com/jquery/eff_toggle.asp)
    - hide와 show 메소드를 전환하는 메소드입니다.
    - 요소가 숨겨져 있으면 show를 실행하며, 요소가 보이면 hide를 실행합니다.
    
- [slideToggle()](https://www.w3schools.com/jquery/eff_slidetoggle.asp)
    - slideUp과 slideDown 사이트를 전환하는 메소드입니다.
    - 요소가 숨겨져 있으면 slideDown이 실행되며 요소가 표시되어 있으면 slideUp을 실행합니다.
    
- [toggleClass](https://www.w3schools.com/jquery/html_toggleclass.asp)
    - 선택 요소에 클래스 이름을 추가하거나 제거할 수 있도록 전환합니다.
    
- 숨겨져 있는 태그를 보여주게 하는 방법
````
$("선택자").css("display", "block");
$("선택자").show();
$("선택자").fadeIn();
$("선택자").slideDown();
$("선택자").toggle();
$("선택자").slideToggle(200);
$("선택자").toggleClass("on");
````

## 30. 배너 스크립트

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [slick 홈페이지](https://kenwheeler.github.io/slick/)

- slick 사용법
    1. slick을 다운받아 프로젝트에 추가합니다.(slick.min.js 파일과 slick.css 파일 추가)
    2. css와 javascript파일을 추가하세요.(jquery도 필요합니다.)
    3. HTML markup을 설정합니다.
    
    ````
    <div class="your-class">
      <div>your content</div>
      <div>your content</div>
      <div>your content</div>
    </div>
    ````
    4. jQuery를 작성합니다.
    
    ````
    $(document).ready(function(){
      $('.your-class').slick({
        setting-name: setting-value
      });
    });
    ````

- 코드에서 사용한 속성값
    - infinite : true / false 값을 가지며, 루프를 무한으로 작동할지를 설정
    - slidesToshow : 한번에 슬라이드 몇개를 보여줄지 설정
    - slidesToScroll : 한번에 스크롤 할 슬라이드 수
    - autoplay : true / false 값을 가지며, 슬라이드 자동 재생 활성화
    - autoplaySpeed : 자동 재생시 변경 시간
    - dots : 현재 슬라이드 표시기를 보여줄 지 확인

## 31. 탭메뉴 스크립트

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [jQuery - chain](https://www.w3schools.com/jquery/jquery_chaining.asp)
    - 액션이나 메소드를 함께 연결할 수 있는 기능입니다.
    - 동일한 요소에 한번에 여러 jQuery 명령을 하나씩 실행할 수 있습니다.
    
- [find()](https://www.w3schools.com/jquery/traversing_find.asp)
    - 섡택 요소의 자식 요소를 리턴하는 메소드
    
- [parent()](https://www.w3schools.com/jquery/traversing_parent.asp)
    - 선택 요소에서 부모 요소를 리턴하는 메소드
    
- [addClass()](https://www.w3schools.com/jquery/html_addclass.asp)
    - 선택 요소에서 클래스 이름을 추가하는 메소드
    
- [removeClass()](https://www.w3schools.com/jquery/html_removeclass.asp)
    - 선택 요소에서 클래스 이름을 제거하는 메소드
    
- [focus()](https://www.w3schools.com/jquery/event_focus.asp)
    - 요소에 포커스가 있을 때 발생합니다.
    
- focus()준 이유는 웹표준을 지키기위해입니다. tab을 클릭했을때 공지사항1 버튼 -> 공지사항 1,2,3 -> 공지사항 2 -> 공지사항2 1,2,3...

- [siblings()](https://www.w3schools.com/jquery/traversing_siblings.asp)
    - 선택 요소의 모든 형제 요소를 반환합니다.

## 갤러리 스크립트

- [포트폴리오 소스코드](https://github.com/ksy90101/MakeOfWebStandard/tree/master/web)

- [slick 홈페이지](https://kenwheeler.github.io/slick/)

- 사용한 slick 옵션
    - fade : 페이드 활성화
    - pauseOnHover : hover시 자동 실행 일시 중지
    - arrows : 다음, 이전 화살표 사용 여부
    - infinite : 무한 루프 여부
    - autoplay : 자동 재생 여부
    - speed : 재생 속도
    - slidesToShow : 한 번에 표시할 수 있는 슬라이드 수 설정
    
- slick 버튼 연결

    - Method 이용하여 버튼에 연결 가능
    - slickPlay : 자동재생
    - slickPause : 일시정지
    - slickNext : 다음
    - slickPrev : 이전

````
$(".play").click(function () {
    $(".gallery_img").slick("slickPlay");
});

$(".pause").click(function () {
    $(".gallery_img").slick("slickPause");
});

$(".prev").click(function () {
    $(".gallery_img").slick("slickPrev");
});

$(".next").click(function () {
    $(".gallery_img").slick("slickNext");
});
````

## 33. 레이어 팝업
[box-shadow]()

## 34. 윈도우 팝업
[window.open](https://www.w3schools.com/jsref/met_win_open.asp)
    - 브라우저 창 또는 새 탭을 여는 메소드입니다.
    - window.open("파일명", "팝업이름", "옵션설정");
    - 옵션 : left(왼쪽 위치), top(위쪽 위치), width(넓이), height(높이), status(상태 바 여부), toolbar(툴바 설정), location(주소필드 설정), menubar(메뉴 바 설정), scrollbars(스크롤 바 설정), fullscreen(전체화면 여부 설정)

## 35. 라이트 박스

- [lightGallery Homepage](https://sachinchoolur.github.io/lightGallery/)

- 사용 방법
    1. lightGallery 다운로드
    2. script  / css 추가
    ````
    <script src="js/lightgallery.min.js"></script>
    <script src="js/lightgallery-all.min.js"></script>
    
    <link rel="stylesheet" href="css/lightgallery.css">
    ````
    3. mark up 추가
    ````
    <div id="lightgallery">
      <a href="img/img1.jpg">
          <img src="img/thumb1.jpg" />
      </a>
      <a href="img/img2.jpg">
          <img src="img/thumb2.jpg" />
      </a>
      ...
    </div>
    ````
    4. jQuery로 plugin Call
    ````
        $(document).ready(function() {
            $("#lightgallery").lightGallery(); 
        });
    ````
  
- 사용한 기능
    - thumbnail : 갤러리 썸네일 사용 여부
    - autoplay : 갤러리 자동 재생 여부
    - pause : 자동 전환 사이간 시간 설정
    - progressBar : 자동 실행 진행 표시줄 여부

## 36. 마무리
- [OpenWAX 크롬 확장 프로그램](https://chrome.google.com/webstore/detail/openwax/bfahpbmaknaeohgdklfbobogpdngngoe)
    - 웹 접근성 여부 점수로 알려주는 프로그램입니다.

## 후기
- 퍼블리셔 관련 강의를 처음 들었는데, 재미도 있었고 너무 즐겁게 들은 강의였다.

- 총 4개의 강의로 이루어져 있으며 하나의 강의를 1월간 열심히 들어서 끝났지만, 꾸준히 못들은 감도 있어서 그 점이 아쉬웠다.

- 다음 강의는 반응형 강의인데, 이번 강의보다 더 효율적으로 들어볼 생각이다.

- 긴 강의 수고해주신 강의자 분께 감사드립니다.