# Week5

[https://www.notion.so/Week5-b764ac13078843cc99968f0dd8c40950?pvs=4](https://www.notion.so/Week5-b764ac13078843cc99968f0dd8c40950)

![html5.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bcf12882-f4f9-4c9c-974d-654c18a8fe65/html5.png)

# HTML5

→**정보와 구조화**

## HTML5에서 지원하는 기능

- **멀티미디어(Multimedia)**

→ 플래시와 같은 플러그인의 도움없이 비디오 및 오디오 기능을 자체적으로 지원한다.

- **그래픽(Graphics & Effects)**

→ SVG, 캔버스를 사용한 2차원 그래픽과 CSS3, WebGL을 사용한 3차원 그래픽을 지원한다.

- **통신(Connectivity)**

→ 기존의 HTML은 단방향 통신만이 가능하였으나 HTML5는 서버와의 소켓 통신을 지원하므로 서버와의 양방향 통신이 가능하다.

- **디바이스 접근(Device acess)**

→ 카메라, 동작센서 등의 하드웨어 기능을 직접적으로 제어할 수 있다.

- **오프라인 및 저장소(Offline & Storage)**

→ 오프라인 상태에서도 애플리케이션을 동작시킬 수 있다. 이는 HTML5가 플랫폼으로서 사용될 수 있음을 의미한다.

- **시맨틱 태그(Semantics)**
    
    ![building-structure.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dc89d15d-95c5-4e97-b624-7f5ef6eb901f/building-structure.png)
    

→  **브라우저, 검색엔진, 개발자 모두에게 콘텐츠의 의미를 명확히 설명하는 역할을 한다.**

→ 이를 통해 HTML 요소의 의미(HTML 요소의 의미)를 명확히 해석하고 그 데이터를 활용할 수 있는 시맨틱 웹을 실현할 수 있다.

→ HTML5에서 새롭게 추가된 시맨틱 태그 =  header, nav, aside, section, article, footer

→ HTML5는 CSS3를 완벽하게 지원한다.

## ****요소의 중첩 (Nested Element)****

→ 요소는 다른 요소를 포함할 수 있다. 이때 중첩 관계(부자 관계)가 성립된다. 이러한 중첩 관계(부자 관계)로 웹페이지의 구조(structure)를 표현할 수 있다.

## ****빈 요소 (Empty Element)****

→ content를 가질 수 없는 요소를 빈 요소(Empty element or Self-Closing element)라 한다.

**빈 요소 중 대표적인 요소** 

→ br, hr, img, input, link, meta

## ****어트리뷰트 (Attribute)****

![html-attribute.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/45c6622e-3712-4f5e-90a2-23a9871c89f7/html-attribute.png)

→ 요소의 성질, 특징을 정의하는 명세. 요소는 attribute를 가질 수 있으며 attribute는 요소에 추가적 정보를 제공한다. 

(추가적 정보 :  이미지 파일의 경로, 크기 등)

→ ****HTML Global Attribute**** = 모든 HTML요소가 공통으로 사용할 수 있는 Attribute

자주 사용되는 글로벌 attribute

→ id, class, hidden, lang, style, tabindex, title 

---

# ****CSS3(Cascading Style Sheets)****

![html-css.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e7122c27-ba04-4a92-af3e-67c5451f256e/html-css.png)

→ **styling의 정의**

→ HTML 요소(Element)의 style(design, layout etc)을 정의한다.

→ HTML이나 XML과 같은 구조화 된 문서(Document)를 화면, 종이 등에 어떻게 렌더링할 것인지를 정의하기 위한 언어

→ HTML과 CSS는 **각자의 문법을 갖는 별개의 언어**이나 HTML없이 단독으로 존재하는 CSS는 의미가 없다.

## ****셀렉터 (Selector, 선택자)****

![css-syntax.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b4e3cbdf-1ee4-4151-a00d-989cbf36ded1/css-syntax.png)

→  위와 같은 구문을 Rule Set(또는 Rule)이라 하고, Rule Set의 집합을 스타일시트(Style Sheet)라 한다.

→ 셀렉터에 의해 선택된 특정 HTML 요소를 어떻게 렌더링(Rendering)할 것인지 브라우저에 지시하는 역할을 한다

→ 복수개의 셀렉터를 연속하여 지정할 수 있으며 쉼표( , )로 구분한다.

### ****전체 셀렉터 (Universal Selector) ⇒ *****

→ ****HTML 문서 내의 모든 요소를 선택한다.****

### ****태그 셀렉터 (Type Selector) ⇒ 태그명****

→ 지정된 태그명을 가지는 요소를 선택한다.

### ****ID 셀렉터 (ID Selector) ⇒ #id 어트리뷰트 값****

→ id 어트리뷰트 값을 지정하여 일치하는 요소를 선택한다. 

(id 어트리뷰트 값은 중복될 수 없는 유일한 값이다.)

### ****클래스 셀렉터 (Class Selector) ⇒ .class 어트리뷰트 값****

→ class 어트리뷰트 값을 지정하여 일치하는 요소를 선택한다. 

(class 어트리뷰트 값은 중복 가능하다. → 재사용의 측면에서 유용)

### ****어트리뷰트 셀렉터 (Attribute Selector)****

- ****셀렉터[어트리뷰트]****

→ 지정된 어트리뷰트를 갖는 모든 요소를 선택한다.

- **셀렉터[어트리뷰트=”값”]**

→ 지정된 어트리뷰트를 가지며 지정된 값과 어트리뷰트의 값이 일치하는 모든 요소를 선택한다.

- **셀렉터[어트리뷰트~=”값”]**

→ 지정된 어트리뷰트의 값이 지정된 값을 (공백으로 분리된) 단어로 포함하는 요소를 선택한다.

- **셀렉터[어트리뷰트|=”값”]**

→ 지정된 어트리뷰트의 값과 일치하거나 지정 어트리뷰트 값 뒤 연이은 하이픈(“값-“)으로 시작하는 요소를 선택한다.

- **셀렉터[어트리뷰트^=”값”]**

→ 지정된 어트리뷰트 값으로 시작하는 요소를 선택한다.

- **셀렉터[어트리뷰트$=”값”]**

→ 지정된 어트리뷰트 값으로 끝나는 요소를 선택한다.

- **셀렉터[어트리뷰트*=”값”]**

→ 지정된 어트리뷰트 값을 포함하는 요소를 선택한다.

## ****복합 셀렉터 (Combinator)****

### ****후손 셀렉터 (Descendant Combinator)****

![descendant-child.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d4b0d5e6-f642-4dda-9aa3-163b12a0b279/descendant-child.png)

→ 자신의 1 level 상위에 속하는 요소를 부모 요소, 1 level 하위에 속하는 요소를 자손 요소(자식 요소)라 하고, 자신보다 n level 하위에 속하는 요소는 후손 요소(하위 요소)라 한다.

→ 후손 셀렉터는 셀렉터A의 모든 후손(하위) 요소 중 셀렉터B와 일치하는 요소를 선택한다.

### ****자식 셀렉터 (Child Combinator)****

→ 자손 셀렉터는 셀렉터A의 모든 자식 요소 중 셀렉터B와 일치하는 요소를 선택한다.

### ****형제(동위) 셀렉터 (Sibling Combinator)****

→ 형제(동위) 셀렉터는 형제 관계(동위 관계)에서 뒤에 위치하는 요소를 선택할 때 사용한다

### ****인접 형제 셀렉터(Adjacent Sibling Combinator)****

→ 셀렉터A의 형제 요소 중 셀렉터A 바로 뒤에 위치하는 셀렉터B 요소를 선택한다. A와 B 사이에 다른 요소가 존재하면 선택되지 않는다.

### ****일반 형제 셀렉터(General Sibling Combinator)****

→ 셀렉터A의 형제 요소 중 셀렉터A 뒤에 위치하는 셀렉터B 요소를 모두 선택한다.

### ****가상 클래스 셀렉터 (Pseudo-Class Selector)****

→ 가상 클래스는 요소의 특정 상태에 따라 스타일을 정의할 때 사용된다

→ 가상 클래스는 마침표(.) 대신 콜론(:)을 사용한다.

**요소의 특정한 상태** 

• 마우스가 올라와 있을때

• 링크를 방문했을 때와 아직 방문하지 않았을 때

• 포커스가 들어와 있을 때

### ****링크 셀렉터(Link pseudo-classes)와 동적 셀렉터(User action pseudo-classes)****

- :link → 셀렉터가 방문하지 않은 링크일 때
- :visited → 셀렉터가 방문한 링크일 때
- :hover → 셀렉터에 마우스가 올라와 있을 때
- :active → 셀렉터가 클릭된 상태일 때
- :focus→ 셀렉터에 포커스가 들어와 있을 때

### ****UI 요소 상태 셀렉터(UI element states pseudo-classes)****

- :checked → 셀렉터가 체크 상태일 때
- :enabled → 셀렉터가 사용 가능한 상태일 때
- :disabled → 셀렉터가 사용 불가능한 상태일 때

### ****구조 가상 클래스 셀렉터(Structural pseudo-classes)****

- :first-child → 셀렉터에 해당하는 모든 요소 중 첫번째 자식인 요소를 선택한다.
- :last-child → 셀렉터에 해당하는 모든 요소 중 마지막 자식인 요소를 선택한다.
- :nth-child(n) → 셀렉터에 해당하는 모든 요소 중 앞에서 n번째 자식인 요소를 선택한다.
- :nth-last-child(n) → 셀렉터에 해당하는 모든 요소 중 뒤에서 n번째 자식인 요소를 선택한다.
- :first-of-type → 셀렉터에 해당하는 요소의 부모 요소의 자식 요소 중 첫번째 등장하는 요소를 선택한다.
- - :last-of-type → 셀렉터에 해당하는 요소의 부모 요소의 자식 요소 중 마지막에 등장하는 요소를 선택한다.
- :nth-of-type(n) → 셀렉터에 해당하는 요소의 부모 요소의 자식 요소 중 앞에서 n번째에 등장하는 요소를 선택한다.
- :nth-last-of-type(n) → 셀렉터에 해당하는 요소의 부모 요소의 자식 요소 중 뒤에서 n번째에 등장하는 요소를 선택한다.
- 

### ****부정 셀렉터(Negation pseudo-class)****

- :not(셀렉터) → 셀렉터에 해당하지 않는 모든 요소를 선택한다.
- 

### ****정합성 체크 셀렉터(validity pseudo-class)****

- :valid(셀렉터) → 정합성 검증이 성공한 input 요소 또는 form 요소를 선택한다.
- :invalid(셀렉터) → 정합성 검증이 실패한 input 요소 또는 form 요소를 선택한다.

### ****가상 요소 셀렉터 (Pseudo-Element Selector)****

→ 요소의 특정 부분에 스타일을 적용하기 위하여 사용

- ::first-letter → 콘텐츠의 첫글자를 선택한다.
- ::first-line → 콘텐츠의 첫줄을 선택한다. 블록 요소에만 적용할 수 있다.
- ::after → 콘텐츠의 뒤에 위치하는 공간을 선택한다. 일반적으로 content 프로퍼티와 함께 사용된다.
- ::before → 콘텐츠의 앞에 위치하는 공간을 선택한다. 일반적으로 content 프로퍼티와 함께 사용된다.
- ::selection → 드래그한 콘텐츠를 선택한다. iOS Safari 등 일부 브라우저에서 동작 않는다.

**요소의 특정 부분**

• 요소 콘텐츠의 첫글자 또는 첫줄

• 요소 콘텐츠의 앞 또는 뒤

## ****프로퍼티 (Property / 속성)****

→ 셀렉터로 HTML 요소를 선택하고 {} 내에 프로퍼티(속성)와 값을 지정하는 것으로 다양한 style을 정의할 수 있다

→ 여러 개의 프로퍼티를 연속해서 지정할 수 있으며 세미콜론(;)으로 구분한다.

→ 프로퍼티는 [표준 스펙](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#Keyword_index)으로 이미 지정되어 있는 것을 사용하여야하며 사용자가 임의로 정의할 수 없다.

### 대표적인 크기 단위

- **px** → px은 [픽셀(화소)](https://ko.wikipedia.org/wiki/%ED%99%94%EC%86%8C) 단위이다. **1px은 화소 1개 크기**를 의미
- **%** →  %는 백분률 단위의 상대 단위이다. 요소에 지정된 사이즈(상속된 사이즈나 디폴트 사이즈)에 상대적인 사이즈를 설정한다.
- **em →** em은 배수(倍數) 단위로 상대 단위이다. 요소에 지정된 사이즈(상속된 사이즈나 디폴트 사이즈)에 상대적인 사이즈를 설정한다.
- **rem** → rem은 최상위 요소(html)의 사이즈를 기준으로 삼는다. rem의 r은 root를 의미한다.

### ****Viewport 단위(vh, vw, vmin, vmax)****

| 단위 | Description |
| --- | --- |
| vw | viewport 너비의 1/100 |
| vh | viewport 높이의 1/100 |
| vmin | viewport 너비 또는 높이 중 작은 쪽의 1/100 |
| vmax | viewport 너비 또는 높이 중 큰 쪽의 1/100 |

## 박스모델(****Box Model****)

![box-model.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/03903b85-9d59-4335-9388-bedd26bf2821/box-model.png)

| 명칭 | 설명 |
| --- | --- |
| Content | 요소의 텍스트나 이미지 등의 실제 내용이 위치하는 영역이다. width, height 프로퍼티를 갖는다. |
| Padding | 테두리(Border) 안쪽에 위치하는 요소의 내부 여백 영역이다. padding 프로퍼티 값은 패딩 영역의 두께를 의미하며 기본색은 투명(transparent)이다. 요소에 적용된 배경의 컬러, 이미지는 패딩 영역까지 적용된다. |
| Border | 테두리 영역으로 border 프로퍼티 값은 테두리의 두께를 의미한다. |
| Margin | 테두리(Border) 바깥에 위치하는 요소의 외부 여백 영역이다. margin 프로퍼티 값은 마진 영역의 두께를 의미한다. 기본적으로 투명(transparent)하며 배경색을 지정할 수 없다. |

## ****Link style****

→ 가장 일반적으로 사용된다.
→ HTML에서 외부에 있는 CSS 파일을 로드하는 방식

### ****Embedding style****

→ HTML 내부에 CSS를 포함시키는 방식

→ HTML과 CSS는 서로 역할이 다르므로 다른 파일로 구분되어 작성하고 관리되는 것이 바람직하다

### ****Inline style****

→ HTML요소의 style 프로퍼티에 CSS를 기술하는 방식

→ JavaScript가 동적으로 CSS를 생성할 때 사용하는 경우가 있지만 일반적인 경우 Link style을 사용하는 편이 좋다.

[https://poiemaweb.com/](https://poiemaweb.com/)
