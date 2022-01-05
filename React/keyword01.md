# REACT KEYWORD
<br>

### 🗝 1/3일 STUDY KEYWORD
```
jsx,component, dom, 라이브러리/프레임워크, angular, vue
```
<br>

### * JSX란(JavaScript eXtension)?


- 쉽게 말해 HTML 문법을 JavaScript 코드 내부에 쓴 것이다. JavaScript의 확장 버전이고 결론은 자바스크립트이다.

 - "React에서 HTML을 표현할 때, JSX를 사용한다. 외관상 HTML같은 마크업 언어를 리터럴로 입력하는 것으로 보이는데,
빌드 시 Babel에 의해 자바스크립트로 변환된다. 자바스크립트 코드를 HTML처럼 표현할 수 있기 때문에 용이한 개발이 가능하다." (나무위키曰)

``` React
const element = <h1>hello</h1>

ReactDom.render(
    element
    document.getElementById('root')
);
```
##### 즉, JSX는 자바스크립트 안에서 HTML 문법을 사용해서 view를 구성할 수 있게 도와주는 자바스크립트 문법으로, 리액트 개발에 엄청난 도움을 주고 있다.
<br>

### * component란?
- "독립적인 기능을 수행하는 단위 모듈"
- 소프트웨어의 재사용성을 높이고 유지보수를 용이하게 하기 위해 나온 기술이 바로 컴포넌트

<br>

### * React component란?
- 리액트에서 컴포넌트는 앱을 이루는 최소한의 단위이다.
- 또한 props나 state와 같은 데이터를 입력받아 DOM 노드를 생성한다. 
- 이러한 컴포넌트들이 유기적으로 잘 연결되고 동작되어야 훨씬 효율적인 앱이 될 수 있다. 
 <br>
 
### * 리액트 컴포넌트의 props와 state는 무엇일까?

-컴포넌트는 두 가지 인스턴스 속성으로 props와 state를 가지고 있다. 

1. props
 - props는 부모 컴포넌트가 자식 컴포넌트에게 주는 값이다.
- 어떠한 값을 컴포넌트에 전달해 줘야 할때 사용하며 할당된 후 컴포넌트 내부에서 값을 변경할 수 없다.

2. state
- state는 컴포넌트 내부에서 선언하며 내부에서 값을 변경할 수 있다.
- 동적인 데이터를 다룰 땐 state를 사용한다.

이러한 기능을 통해 컴포넌트 간에는 무조건 props를 통해서만 데이터를 주고받고, 변경되는 값은 state만큼만 확인하면 되므로 개발자가 더 편리하게 개발을 할 수 있게 되었다.

<br>

### * Dom이란?
- 문서 객체 모델(Document Object Model)은 HTML, XML document와 상호작용하고 표현하는 API이다.
- 웹 페이지를 구성하는 요소(문서)를 구조화하고 Javascript(객체)를 이용하여 웹 페이지 구성요소를 제어할 수 있다
![다운로드](https://user-images.githubusercontent.com/76805997/147996665-217e0ddf-e9d1-47a7-aa62-bfa1a45f56ef.png)

- 자바스크립트는 이러한 문서 객체 모델을 이용하여 document에 접근해 작업을 할 수 있다.
- 즉, DOM은 HTML과 스크립팅언어(자바스크립트)를 서로 이어주는 역할을 한다.
<br>

### * Virtual Dom?
- 가상 DOM은 실제 DOM의 가벼운 사본이다.
- 변화가 많은 View를 실제 DOM에서 직접 처리하는 방식이 아닌 Virtual Dom과 메모리에서 미리 처리하고 저장한 후 실제 DOM과 동기화 하는 프로그래밍 개념
- DOM의 상태를 메모리에 저장하고 변경 전과 변경 후의 상태를 비교한 뒤 최소한의 내용만 반영 하는 기능

```
DOM 자체는 빠르지만 요소의 개수가 수 백 개, 수 천 개로 늘어날 경우, 느려지기 때문에 DOM을 최소한으로 조작
=> 리액트에서는 이러한 문제점을 해결하기 위해 virtual DOM 방식을 사용해 DOM의 업데이트를 추상화하여 처리횟수 최소화

1) 업데이트된 전체 UI를 Virtual Dom에 리렌더링
2) 실제 DOM과 생성된 Virtual Dom 을 비교
3) 바뀐 부분만 실제 DOM에 적용
```
<br>

### * 라이브러리/프레임워크?
1. Framework(프레임워크)
> #### 소프트웨어의 특정 문제를 해결하기 위해서 상호 협력하는 클래스와 인터페이스의 집합
- 프레임워크는 뼈대나 기반구조를 뜻하는데, Application 개발 시 필수적인 코드, 알고리즘, 데이터베이스 연동 등과 같은 기능들을 위해 어느정도 뼈대(구조)를 제공
-  그러므로 그러한 뼈대 위에 프로그래머가 코드를 작성하여 Application을 완성시켜야 함.
-  어느정도 뼈대를 제공해 주기 때문에, 객체 지향 개발을 하면서 일관성 부족 등의 문제해결 가능.
<br>

2. Library(라이브러리)
> #### 단순 활용이 가능한 도구들의 집합
- Library는 특정 기능에 대한 도구 or 함수들을 모은 집합. 즉, 프로그래머가 개발하는데 필요한 것들을 모아둔 것.
<br>

3. Framework와 Library의 차이 - Inversion Of Control
- #### Framework와 Library의 차이는 Flow(흐름)에 대한 제어 권한이 어디에 있느냐의 차이. 
- 프레임워크는 전체적인 흐름을 자체적으로 가지고 있으며, 프로그래머가 그 안에 필요한 코드를 작성
- 라이브러리는 사용자가 흐름에 대해 제어를 하며 필요한 상황에 가져다 씀.
- 이 내용을 한 문장으로 정리하자면 프레임워크에는 제어의 역전(Inversion Of Control)이 적용되어있다는 것입니다.

```
제어의 역전(Inversion Of Control)이란 어떠한 일을 하도록 만들어진 프레임워크에 제어의 권한을 넘김으로써 클라이언트 코드가 신경서야 할 것을 줄이는 전략입니다. 
일반적으로 우리는 프로젝트를 생성하고 Main함수를 만들어서 시작지점을 형성합니다.
그리고 Main 함수에서 프로그램의 흐름을 정하는 것은 프로그래머의 몫으로 우리가 어떠한 순서를 부여하느냐에 따라서 흐름을 제어하는 것이 일반적인 사고입니다. 

하지만 여기서 프레임워크는 실행의 흐름을 프레임워크 자체가 가지고 있어서 우리의 코드를 프레임워크안에 넣어서 개발을 진행해야 합니다. 
실제로 Maven과 같은 프레임워크의 프로젝트를 생성해보면 어느정도 뼈대를 만들어서 그 안에 필요에 따라 우리의 코드를 넣습니다. 
일반적으로 프로그래머가 가지고 있어야하는 제어의 권한을 프레임워크에게 주었기 때문에 우리는 이를 제어의 역전이라고 말합니다.
```

<br>

#### 참고
1) [state를 활용해서 컴포넌트에서 동적인 데이터를 다루는 방법](https://moonsbeen.tistory.com/210?category=1200619)<br>
2) [리액트의 기본, 컴포넌트를 알아보자](https://medium.com/little-big-programming/react%EC%9D%98-%EA%B8%B0%EB%B3%B8-%EC%BB%B4%ED%8F%AC%EB%84%8C%ED%8A%B8%EB%A5%BC-%EC%95%8C%EC%95%84%EB%B3%B4%EC%9E%90-92c923011818)

<br>
<br>


# 리액트/노드

# 정리

---

- react
    
    `jsx,component, dom, 라이브러리/프레임워크, angular, vue`
    
    ## 라이브러리, 프레임워크 차이
    
    ### 라이브러리
    
    - 단순 활용이 가능한 도구들의 집합
    - 소프트웨어 개발할 때 컴퓨터 프로그램이 사용하는 비휘발성 자원
    - 미리 작성된 코드, 변수, 함수, 클래스 등 포함
    - 개발자가 필요할 때 호출하여 사용
    
    ### 프레임워크
    
    - 뼈대니 기반구조
    - 소프트웨어의 특정 문제를 해결하기 위해서 상호 협력하는 클래스와 인터페이스의 집합
    - 개발을 수월하게 하기 위해 소프트웨어의 구체적인 기능들에 해당하는 부분의 설계와 구현을 재사용 가능하도록 협업화된 형태로 제공하는 소프트웨어 환경
    - 개발 시 필수적인 코드, 알고리즘, 데이터베이스 연동 등과 같은 기능를 위해 어느정도 뼈대 제공
    - 제어의 역전 ( 프레임 워크 위에 개발한 클래스를 등록해두고, 프레임워크가 흐름을 주도하는 중에 개발자가 만든 애플리케이션 코드를 사용하도록 만드는 방식 )
    
    ### 라이브러리와 프레임워크 차이
    
    - flow에 대한 제한 권한이 어디에 있느냐의 차이
    - 프레임워크 - 전체적인 흐름을 자체적으로 가지고 있으며, 프로그래머가 그 안에 필요한 코드 작성
    - 라이브러리 - 사용자가 흐름에 대한 제어를 하여 필요한 상황에 가져다 쓰는 것
    
    ## react, angular, vue 차이
    
    ### React
    
    - 라이브러리
    - 페이스북 개발자가 개발, 페이스북에서 유지 보수
    - [Virtual Dom](https://www.youtube.com/watch?v=BYbgopx44vo) 지원
    - SSR - [Next.js](https://nextjs.org/)
    - [JSX](https://ko.reactjs.org/docs/introducing-jsx.html) (JavaScritp + XML)
    - [React Native](https://reactnative.dev/) (앱 개발까지 가능)
    - 라이브러리이지만 컴포넌트를 사용한다면, 프레임워크처럼 규칙을 지켜야함
    - 장점 - [Virtual Dom](https://ko.reactjs.org/docs/faq-internals.html) ⇒ Dom 트리를 추상화하여 자바스크립트 객체로 만들어 두고 변경되는 부분은 virtual dom에서 처리하여 성능을 높힘
        - virtual DOM(변경된 부분 처리) ————→ real DOM(virtual DOM에서 받으거랑 비교 했을 때 달라지 부분만 변경, 안달라졌으면 변경 X) / 유튜브보고 정리한거 더 자세히 공부해봐야함
    - SPA(Single Page Application) 방식으로 진행한다면 검색엔진 노출(SEO : Search Engine Optimization)에 관련된 문제를 생각 했을 때 SSR을 염두해 둘 수 밖에 없었는데 Next.js를 사용하여 해결 가능
    - UI를 구성하는 개별적인 뷰 단위인 컴포넌트 단위로 작성하여 생산성과 유지보수에 좋음
    - JSX(자바스크립트 확장 문법)을 사용하여 컴포넌트를 생성 가능
    
    ### Angular
    
    - 타입스크립트 기반 오픈소스 프레임워크
    - 구글 앵귤러팀 개발, 구글에서 유지보수
    - 양방향 바인딩 지원
    - TypeScript 기반
    - [RxJs](https://github.com/ReactiveX/rxjs) (Reactive Extensions For JavaScript) : 스트림을 통한 비동기 처리 방식 지원
    - 가장 체계적이고 잘 정리되어있는 문서와 튜토리얼
    - 큰 러닝커브
    - 라우팅, 상태관리, 폼 유효성 등 필요한 도구를 모아놓은 All In One 프레임워크
    - React와 Vue.js와 비교했을 때 가장 배울 것이 많고 어려운
    - 가볍고 빠르게 작업을 해야하는 프로젝트 보다는 큰 프로젝트에 사용하기 적합
    - TypeScript를 기반으로 하기 때문에 엄격하지만 그만큼 직관적이고 오류를 줄일 수 있음
    - 웹사이트가 빠르고 효율적으로 렌더링 되게 설계되어있음
    - MPA를 구성하기에는 복잡하고, SPA에서는 매우 빠르게 작동한다. 애초에 구글이 SPA를 위해 만든 것이라고 한다.
    
    ### Vue
    
    - 오픈소스 자바스크립트 프레임워크이며
    - Google의 전 개발자 Even You 개발, 그를 주축으로 유지보수
    - Virtual Dom 지원
    - SSR - [Nuxt.js](https://ko.nuxtjs.org/)
    - 양방향과 단방향의 바인딩 지원
    - [TypeScript 지원](https://kr.vuejs.org/v2/guide/typescript.html)
    - [NativeScript](https://nativescript-vue.org/ko/docs/introduction/)
    - [Single File Component](https://kr.vuejs.org/v2/guide/single-file-components.html)
    - 작은 러닝커브(학습 및 적응이 빠름)
    - React의 장점인 Virtual Dom과 Angular의 양방향 바인딩을 가져옴
    - 자바스크립트의 기본 스타일을 적극적으로 적용하고 있어서 학습하고 적응하기 쉬움
    - 그리고 Single File Component는 `.vue` 파일에 HTML과 CSS 그리고 Script까지 하나로 묶어서 컴포넌트 단위로 직관적인 구성이 가능하다는 것
    - 디자이너나 퍼블리셔와 협업하는 과정에서는 생산성이나 유지보수에 큰 도움이 될 것
    
    ## DOM, 가상 DOM
    
    ## JSX
    
    ## Component
    

# 참고자료

---

- 리액트 면접질문
    
    [https://appear.github.io/2018/10/20/REACT/react-translate-01/](https://appear.github.io/2018/10/20/REACT/react-translate-01/)
    
- es6 달라진 점
    
    [https://blog.naver.com/doredome/222587484066](https://blog.naver.com/doredome/222587484066)
    
- 라이브러리, 프레임워크
    
    [https://webclub.tistory.com/458](https://webclub.tistory.com/458)
    
- react, angular, vue.js
    
    [https://velog.io/@goblin820/TIL-2-Vue-React-Angular](https://velog.io/@goblin820/TIL-2-Vue-React-Angular)
    
