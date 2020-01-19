# [\[groom\]\[웹퍼블리싱 실습\] 웹 표준 사이트 만들기](https://edu.goorm.io/learn/lecture/16941/%EC%9B%B9%ED%8D%BC%EB%B8%94%EB%A6%AC%EC%8B%B1-%EC%8B%A4%EC%8A%B5-%EC%9B%B9-%ED%91%9C%EC%A4%80-%EC%82%AC%EC%9D%B4%ED%8A%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0/info)

## 강의 소개

- groom 사이트에 있는 웹퍼블리싱 강의를 직접 실습하고 필요한 내용을 정리했습니다.

- [\[groom\]\[웹퍼블리싱 실습\] 웹 표준 사이트 만들기](https://edu.goorm.io/learn/lecture/16941/%EC%9B%B9%ED%8D%BC%EB%B8%94%EB%A6%AC%EC%8B%B1-%EC%8B%A4%EC%8A%B5-%EC%9B%B9-%ED%91%9C%EC%A4%80-%EC%82%AC%EC%9D%B4%ED%8A%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0/info)

- HTML 태그와 CSS 속성에 대한 자세한 설명은 강사님이 정리 해놓으신 레퍼런스에서 찾아서 링크 걸어놓았습니다.
자세한 내용들은 링크에 들어가서 보시면 훨씬 이해 하시기 좋으실꺼 같습니다.

- [제작한 포트폴리오 사이트](http://ksy90101.dothome.co.kr/web/)

- 직접 실습한 코드들은 [Github Repository](https://github.com/ksy90101/MakeOfWebStandard)에 있습니다.

## 1. Layout01

- HTML 요소(Content Element)
    - meta, self-closing, block, inline으로 분류
    - block, inline 두개의 구조를 구분을 잘 해야 함.
    - block 구조는 박스라고 생각하면 되며, inline 구조는 텍스트라고 생각하면 쉬움.
    - block 구조는 위에서 아래로 태그들이 쌓이는 것이라고 생각하면 됨.
    - inline 구조는 왼쪽에서 오른쪽으로 배치된다고 생각하면 됨.
    
- \<div>태그
    - 문서의 섹션을 만들거나 영역을 나눌때 사용
    - [div태그 설명](https://webzz.tistory.com/264)
    
- float 속성
    - 블록오쇼의 정렬 상태를 설정
    - none(기본값), left, right 속성값을 가지고 있음.
    - float을 쓴 블록요소는 height값을 0으로 인식하기 때문에 깨지는 현상이 발생
        - 가장 기초적인 해결 방법은 깨진 블록 요소에 float:left를 똑같이 주는 방법이다.
    - [float 속성 설명](https://webzz.tistory.com/452)

- margin 속성
    - 바깥쪽 여백을 설정
    - 속성값 중에 auto를 이용하면 가운데 정렬을 할 수 있음
    - [margin 속성 설명](https://webzz.tistory.com/490)
    
- text-transform 속성
    - 텍스트를 대문자나 소문자로 변경
    - uppercase, lowercase, capitalize(첫글자만 대문자) 3개의 속성값이 존재
    - [text-transform 속성 설명](https://webzz.tistory.com/544)

- text-align 속성
    - 텍스트 정렬 방식을 설정
    - [text-align 속성 설명](https://webzz.tistory.com/534) 

- line-height
    - 문장과 문장 사이의 간격을 설정
    - 텍스트가 한줄일때, 세로 가운데 정렬을 하기 위해 감싸고 있는 블록의 높이값과 똑같이 즐때 사용
    - 한줄일때만 가능하며, 두줄 이상일 경우에는 세로 가운데 정렬이 안됨
    - [line-height 속성 설명](https://webzz.tistory.com/485)
    
## 2. layout02

- clear 속성
    - float요소의 성질을 차단
    - float을 쓴 블록요소는 height값을 0으로 인식하기 때문에 깨지는 현상이 발생했는데, 그걸 해결할 수 있는 방법중 하나
    - [clear 속성 설명](https://webzz.tistory.com/424)

## 3. layout03

## 4. layout04

## 5. layout05

- \* 선택자
    - 모든 선택자에게 같은 값을 넣어줌
    - 모든 태그들은 각자 가지고 있는 고유 속성들이 있음. 그 속성들을 초기화 시킬때 사용함.(예를 들면, margin / padding)
    - 그러나 전체 선택자는 실무에서 잘 사용하지 않음. 그냥 있다는 것만 알고 계시면 좋음.
    
- 부모와 자식의 속성값이 똑같다면, 생략이 가능함.(중복코딩 피하기!)
    - 예를들어 부모의 높이가 100px이고, 자식의 높이가 100px이면, 자식 높이는 생략 가능
    
- width값의 기본값은 100%이기때문에 생략가능

## 6. layout06

- inherit 속성값
    - 부모의 속성값을 상속받는다는 의미

- 코드 간략화
    - 최대한 코드가 중복되는 것들은 하나의 클래스를 생성해서 모아두는 것이 좋음

## 7. layout07

- 주석을 적어주면서, 남이 코드를 봤을때 최대한 이해를 도와야 하며, 선택자명을 잘 짓는 것이 중요함.

## 8. layout08

- 이제부터 웹 서버에 올려서 예제를 공유할 예정

- 웹서버를 이용하기 위해서는 파일질라가 필요함

- [파일질라](https://filezilla-project.org/)

- Intelli J 웹서버 접근(Remote Host) -> 사용법 차후 포스팅

- \<!doctype html\>
    - html5 선언

- \<html lang="ko"\> 
    - 언어 설정 및 html 문서 시작(가장 최상위 태그)
    
- [\<head\>](https://webzz.tistory.com/278)
    - 제목과 스크립트, 스타일 시트, 메타 정보 등을 제공
    - 화면에 보이지 않는 정보들을 넣음
    
- [\<meta\>](https://webzz.tistory.com/300)
    - 웹 문서에 대한 정보를 제공
    - author(제작자), charset(언어셋), description(사이트에 대한 설명), keywords(사이트에 대한 키워드) 등등에 대해 정의
    - 자세한 내용은 위의 링크에서 확인

- [\<link\>](https://webzz.tistory.com/293)
    - 외부 파일을 연결할 때 설정
    - 보통 CSS를 연결할 때 사용함.
    - 외부 스크립트 파일을 연결할때는 \<script\> 태그를 사용함.(헷갈리지 말것!)

## 9. layout9

## 10. 스킵메뉴

- 참고사이트
    - [웹접근성 연구소](https://www.wah.or.kr:444/index.asp)
    - [네이버 웹표준 널리](https://nuli.navercorp.com/)
    - [다음 웹표준 다룸](http://darum.daum.net/)
    
- 참고사이트에 가면 웹 접근성에 대한 자세한 이야기들이 있음.

- 웹 접근성은 모든 사람이 정보통신 기기나 서비스를 손쉽게 활용할 수 있게 하는 것이 목적이다.

- 우리나라는 2013년 웹 접근성이 의무화 됨.

- 데스크톱 웹사이트뿐만 아니라 모바일 웹사이트도 웹접근성 지침이 모두 존재

- 따라서 웹접근성에 따라 스킵메뉴를 만들어 줘야 함. (Tap을 누르면, 스킵메뉴가 보임)

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

- 상대주소 vs 절대주소

- background : url();
    - 처음에 이미지가 반복되어 있음

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
- 이미지를 표현하는 방법
    1. img 태그로 표현(의미가 있을 때)
        - alt 속성으로 대체 문자를 표현할 수 있음 따라서 의미가 있을때 사용함
        - [img 태그 자세히 보기](https://webzz.tistory.com/285)
    2. background 속성으로 표현(의미가 없을 때)
        - [background-image 속성 자세히 보기](https://webzz.tistory.com/380)
    3. 최근 웹사이트는 background 속성을 이용하여 이미지를 표현하며, 가상으로 대체 문자를 만들어줌(IR 효과)
    왜냐하면 웹 접근성을 만족시켜야 하기 때문에 인데, 왜 background 속성을 사용하는 이유는 이미지 스프라이트를 사용하여 서버 요청을 최소화 하기 위해서입니다.
        - [IR 효과](http://ui.daum.net/convention/css/css_ir)
        - [이미지 스프라이트](http://tcpschool.com/css/css_basic_imageSprites)

- IR효과

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
