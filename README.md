# [\[groom\]\[웹퍼블리싱 실습\] 웹 표준 사이트 만들기](https://edu.goorm.io/learn/lecture/16941/%EC%9B%B9%ED%8D%BC%EB%B8%94%EB%A6%AC%EC%8B%B1-%EC%8B%A4%EC%8A%B5-%EC%9B%B9-%ED%91%9C%EC%A4%80-%EC%82%AC%EC%9D%B4%ED%8A%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0/info)

## 강의 소개
- groom 사이트에 있는 웹퍼블리싱 강의를 직접 실습하고 필요한 내용을 정리했습니다.

- [\[groom\]\[웹퍼블리싱 실습\] 웹 표준 사이트 만들기](https://edu.goorm.io/learn/lecture/16941/%EC%9B%B9%ED%8D%BC%EB%B8%94%EB%A6%AC%EC%8B%B1-%EC%8B%A4%EC%8A%B5-%EC%9B%B9-%ED%91%9C%EC%A4%80-%EC%82%AC%EC%9D%B4%ED%8A%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0/info)

- HTML 태그와 CSS 속성에 대한 자세한 설명은 강사님이 정리 해놓으신 레퍼런스에서 찾아서 링크 걸어놓았습니다.
자세한 내용들은 링크에 들어가서 보시면 훨씬 이해 하시기 좋으실꺼 같습니다.

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

- * 선택자
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

````
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="rutgo">
    <meta name="description" content="웹 표준을 준수한 사이트 예제입니다.">
    <meta name="keywords" content="럿고, 웹표준, 웹접근성, 사이트 만들기">
    <title>Document</title>
</head>
<body>

</body>
</html>
````

- 크롤러(검색 로봇)

- <link> - CSS 외부파일 연동