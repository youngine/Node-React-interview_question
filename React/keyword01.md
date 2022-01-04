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

#### 참고
1) [state를 활용해서 컴포넌트에서 동적인 데이터를 다루는 방법](https://moonsbeen.tistory.com/210?category=1200619)<br>
2) [리액트의 기본, 컴포넌트를 알아보자](https://medium.com/little-big-programming/react%EC%9D%98-%EA%B8%B0%EB%B3%B8-%EC%BB%B4%ED%8F%AC%EB%84%8C%ED%8A%B8%EB%A5%BC-%EC%95%8C%EC%95%84%EB%B3%B4%EC%9E%90-92c923011818)