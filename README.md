## CSS란
---
1. CSS는 Cascading Style Sheets의 약자이다.
2. CSS는 HTML태그들이 각종 미디어에서 어떻게 보이는가를 정의하는데 사용한다.
3. 스타일을 HTML문서로부터 분리하는 것이 가능해진다.
### CSS를 사용하는 이유
- HTML만으로 웹 페이지를 제작할 경우 HTML 태그의 세부 스타일을 일일이 따로 지정해주어야 하기 때문에 많은 시간이 걸려야 하며, 완성한 후에도 스타일의 변경 및 유지보수가 힘들어 진다.
이문제점을 해결하기 위해서 W3C에서 만든 스타일 시트 언어가 바로 CSS이다.
- 웹페이지의 스타일을 별도의 파일로 저장할 수 있게 해줌으로써 사이트의 전체 스타일을 손쉽게 제어할 수 있게 된다. 또한 웹 사이트의 스타일을 일관성있게 유지할 수 있도록 해주고 그로 인해 유지보수도 보다 쉬워진다.
---


### CSS 문법
[선택자] 속성명  속성값  속성명  속성값
                [선언부]

- CSS의 문법은 선택자와 선언부로 구성된다.
- 선택자는 CSS를 적용하고자 하는 HTML 태그를 가리키고 선언부는 중괄호({})를 사용하여 전체를 둘러싼다.
- 각 선언은 CSS 속성명과 속성 값을 콜론(:)으로 연결한다.
- CSS 선언은 언제나 마지막에 세미콜론(;)으로 끝마친다.

### CSS 주석
- 주석을 표시할 떄에는 /* */ 사이에 내용을 입력한다.
- CSS 선택자
- 전체 선택자
  - 스타일을 모든 요소에 적용할 때 사용한다
  - 주로 모든 하위 요소에 한꺼번에 스타일을 적용할 때 사용하고, 전체 선택자는 asterisk(*) 기호를 사용한다.
- 태그 선택자
  - 특정 태그가 쓰인 모든 요소에 스타일을 적용한다.
  - 선택자 위치에 태그명을 작성하면 사용된 모든 해당 태그에 동일한 스타일이 적용된다.
- 클래스 선택자
  - 클래스 선택자는 특정 집단의 여러 요소를 한번에 선택할 때 사용한다.
  - 같은 클래스 이름(class="")을 가지는 요소들을 모두 선택해주고 스타일 적용 시 선택자에 ".클래스명"을 작성해준다.
- 아이디 선택자
  - 아이디 선택자는 특정 요소를 선택할 때 사용한다.
  - 스타일을 지정할 때 사용되며, 선택자 부분에 "#아이디명"을 입력한다.
- 그룹 선택자
  - 여러 선택자에 같은 스타일을 적용할 경우 쉼표로 구분해서 여러 선택자를 나열한 후 스타일을 한 번만 정의한다.

#### 캐스케이딩(Casecading)
  - 하나의 요소는 CSS선언에 영향을 받을 수 있다
  - 이때 충돌을 피하기 위해 CSS적용 우선순위가 필요하다

#### 우선순위

  - 중요도: CSS가 어디에 선언되어 있는지에 따라서 우선 순위가 달라진다.

    1. 인라인 스타일(HTML 태그 내부에 style 속성으로 사용)
    2. 내부 인라인 스타일(HTML 문서의 style 태그 안에 위치)
    3. 외부 인라인 스타일(CSS 파일을 외부에 따로 만들어서 불러오는 방법)
    4. 웹 브라우저 기본 스타일
    5. 명시도: 명확하게 특정할수록 우선 순위가 높아진다.
       - !important
       - 인라인 스타일
       - 아이디 선택자
       - 틀래스 선택자
       - 태그 선택자
       - 전체 선택자
       - 상속받은 속성
       - 선언 순서 : 나중에 선언된 스타일이 우선 적용된다
#### 시맨틱 태그
- 시맨틱: "의미가 있는"
  - HTML5에 도입된 시맨틱 태그는 개발자와 브라우저에세 의미있는 대트를 제공한다.
    
#### 태그 종류
  - <div>: non-semantic 태그, 안에 들어간 내용의 의미를 유추하기 어렵다.
  - <header>, <footer>, <main>, ..: semantic 태그, 특정 형태의 글이 포함될 것이라는 유추가 가능하다.
  - header: 상단, 헤더를 의미
  - nav: 메뉴, 내비게이션을 의미
  - main: 내용의 중심을 의미
  - aside: 사이드에 위치하는 공간을 의미
  - section: 여러 중심 내용을 감싸는 공간을 의미
  - article: 글자가 많이 들어간 부분을 의미
  - footer: 하단, 푸터를 의미
