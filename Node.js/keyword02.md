# Node.js KEYWORD 02
<br>

### 🗝 **[1/5일 STUDY KEYWORD](Node.js/keyword02.md)**
```
npm ,webpack , package.json, 클래스형 컴포넌트, 함수형 컴포넌트
```
<br>

### * npm 이란?
- #### npm이란 Node Package Manager의 약자로, 노드의 패키지 매니저이다. 
- #### 다른 사람들이 만든 소스 코드들을 모아둔 저장소.
- 남의 코드를 사용하여 프로그래밍 가능
- 이미 있는 기능을 다시 구현할 필요가 없어 효율적이다.
- 오픈 소스 생태계를 구성중
- 패키지 : npm에 업로드된 노드 모듈
- 모듈이 다른 모듈을 사용할 수 있듯, 패키지도 다른 패키지를 사용할 수 있다.
 
```
//npm을 통해 설치한 모듈(패키지) 들은 Common JS의 문법 형식으로 불러와 쓸 수 있다. 형식은 다음과 같다
//npm install을 통해 다운받은 express를 사용하고 싶다면

var express = require('express');
```
<br>


### * package.json 이란?
- #### 현재 프로젝트에 대한 정보와 사용 중인 패키지에 대한 정보를 담은 파일.
- #### 프로젝트(해당 디렉토리)가 의존하고 있는 모듈들의 목록과 버전정보를 제공
- 같은 패키지라도 버전별로 기능이 다를 수 있으므로 버전을 기록해두어야 함
- 동일한 버전을 설치하지 않으면 문제가 생길 수 있다.
- 노드 프로젝트 시작 전 package.json부터 만들고 시작함 (package.json 생성 명령어 : npm init)

<br>

### * webpack 이란?
<img width="600" alt="1_F070uzOYIL8LXzAGf5zy9A" src="https://user-images.githubusercontent.com/76805997/148311774-59766a42-579e-4cb7-b70f-c2e577937133.png">

- #### 웹팩은 오픈 소스 자바스크립트 모듈 번들러
- 여러개로 나누어져 있는 파일들을 하나의 자바스크립트 코드로 압축하고 최적화하는 라이브러리
- 여러 파일의 자바스크립트 코드를 압축하여 최적화 할 수 있기 때문에 로딩에 대한 네트워크 비용을 줄일 수 있음
- 모듈 단위로 개발이 가능하여, 가독성과 유지보수가 쉬움
<br>

### * Webpack을 왜 사용해야 할까 ?
- 옛날에는 페이지마다 새로운 html을 요청해서뿌려 주는 방식이였다면, 요새는 SPA 하나의 html 페이지에 여러개의 자바스크립트 파일들이 포함한다. 연관 되어 있는 자바스크립트 종속성 있는 파일들을 하나의 파일로 묶어줘서 관리하기 편하다.
- 파일을 컴파일 할 때, 여러 모듈들의 파일을 읽어오는데 시간이 오래 걸린다. 그 부분을 해결하기 위해 여러 파일을 하나의 파일로 번들링 해준다.
- 하나의 자바스크립트 파일로 만들어서 네트워크 접속의 부담을 줄이고 , 더 빠른 서비스 제공 가능
<br>

### * SPA vs MPA
- SPA(Single Page Application)는 한 개(Single)의 Page로 구성된 Application이다.
- MPA(Multiple Page Application)는 여러 개(Single)의 Page로 구성된 Application이다.
- MPA는 새로운 페이지를 요청할 때마다 정적 리소스가 다운로드된다. 매번 전체 페이지가 다시 렌더링 된다.
- #### 반면 SPA는 웹 에플리케이션에 필요한 모든 정적 리소스를 최초 한 번에 다운로드한다.
- #### 그 이후 새로운 페이지 요청이 있을 때, 페이지 갱신에 필요한 데이터만 전달 받아서 페이지를 갱신한다.
- 그래서 SPA를 CSR(Client Side Rendering) 방식으로 렌더링한다고 말한다.
- 그래서 MPA를 SSR(Server Side Rendering) 방식으로 렌더링한다고 말한다.
<br>

### * 컴포넌트(Component)란?
- 리액트로 만들어진 앱을 이루는 최소한의 단위
- 컴포넌트는 데이터(props)를 입력받아 View(state) 상태에 따라 DOM Node를 출력하는 함수.
- 그래서 합성을 통해 UI를 재사용할 수 있고, 독립적인 단위로 쪼개어 생각할 수 있게 한다.  
<br>


### * 클래스형 컴포넌트 vs 함수형 컴포넌트?

### 🚩 1) 차이: 선언방식

#### (1) 클래스형 컴포넌트

![1](https://user-images.githubusercontent.com/76805997/148317012-d1921af7-5efd-4603-b77f-258034f4850f.png)

1. class 키워드 필요
2. Component로 상속을 받아야한다.
3. render() 메소드가 반드시 필요하다.
4. state, lifeCycle 관련 기능사용이 가능하다.
5. 함수형보다 메모리 자원을 더 사용한다.
6. 임의 메소드를 정의할 수 있다.


#### (2) 함수형 컴포넌트

![2](https://user-images.githubusercontent.com/76805997/148317088-e05ca3ee-30ff-4f96-a518-38f85a62d3b2.png)

1. state, lifeCycle 관련 기능사용 불가능하다. [Hook을 통해 해결]
2. 클래스형보다 메모지 자원을 덜 사용한다.
3. 컴포넌트 선언이 편하다.

<br>


###  🚩2) 차이: State
- State 란? 컴포넌트 내부에서 바뀔 수 있는 값


#### (1) 클래스형 컴포넌트

![3](https://user-images.githubusercontent.com/76805997/148317716-a04e8b03-3409-4e61-ba72-d92b28cd9930.png)

1. constructor 안에서 this.state 초기 값 설정 가능
2. counstructor 없이도 바로 state 초기값을 설정 가능
3. this.setState() 를 통해 state값을 변경
4. 클래스형의 state는 객체형식

#### (2) 함수형 컴포넌트

![4](https://user-images.githubusercontent.com/76805997/148317717-f6e84398-97ca-48dc-95ae-535b2292315a.png)

1. useState 함수로 state를 사용한다.
2. useState 함수를 호출하면 배열이 반환되는데 첫 번째 원소는 현재 상태, 두번째 원소는 상태를 바꿔주는 함수이다.
<br>

### 🚩 3) 차이: props
- Props 란? 컴포넌트의 속성을 설정


#### (1) 클래스형 컴포넌트

![5](https://user-images.githubusercontent.com/76805997/148318028-13755ecd-f092-4cf0-beff-92dbfe525c43.png)
1. this.props로 통해 값을 불러올 수 있다.

#### (2) 함수형 컴포넌트

![6](https://user-images.githubusercontent.com/76805997/148318030-458db084-758e-4085-9989-f066f6e20901.png)

1. props를 불러올 필요 없이 바로 호출 할 수 있다.
<br>

###  🚩4) 차이: 이벤트 핸들링

#### (1) 클래스형 컴포넌트

![7](https://user-images.githubusercontent.com/76805997/148318561-aa8e2f00-c78b-4d2d-94b3-a1af393748ec.png)

1. 함수 선언시 화살표 함수로 바로 선언 가능하다.
2. 요소에 적용할때 this.를 붙여줘야한다.

#### (2) 함수형 컴포넌트

![8](https://user-images.githubusercontent.com/76805997/148318569-d487dfa3-eb91-4263-8903-3733cd90f1c6.png)

1. const + 함수 형태로 선언해야 한다.
2. 요소에 적용할때 this가 필요없다.
<br>

###  🚩5) 차이: Life Cycle
* #### Life Cycle 이란?
- React에서 컴포넌트는 여러 종류의 "생명주기 메소드" 를 가지며 이 메소드를 오버라이딩(상속하여 재정의) 하여 특정 시점에 코드가 실행되도록 설정 합니다.
- 클래스 컴포넌트에만 해당되는 내용이며, 함수형 컴포넌트는 Hook를 사용하여 생명주기에 원하는 동작을 합니다
<br>

### * 함수형 컴포넌트를 선호하는 이유?
- 클래스형 컴포넌트는 로직과 상태를 컴포넌트 내에서 구현하기 때문에 상대적으로 복잡한 UI 로직을 갖고 있는 반면,
- 함수형 컴포넌트는 state를 사용하지 않고 단순하게 데이터를 받아서(props) UI에 뿌려준다. 
- Hook들을 필요한 곳에 사용하며 Logic의 재사용이 가능하다는 장점이 있어 함수형 컴포넌트+Hook을 주로 사용한다고 한다.
<br>

### * Props and state?
1. #### 공통점
> 두 객체 모두 렌더링 결과물에 영향을 주는 정보를 가지고 있다.
2. #### 차이점
> - props는 (like 함수 매개변수) Component에 전달된다.
> - state는 (like 함수 내에 선언된 변수) Component안에서 관리된다.
3. #### props
- 부모 Component-> 자식 Component로 전달해주는 읽기 전용 데이터.
- 자식 Component에서 props는 변경이 불가능하고, props를 전달해준 최상위 부모 component만 변경가능
4. #### state
- 동적인 데이터를 다룰 때 사용.
- 독립적이라 다른 component의 접근이 불가능
<br>

### 참고
- [SPA vs MPA와 SSR vs CSR 장단점 뜻정리](https://hanamon.kr/spa-mpa-ssr-csr-%EC%9E%A5%EB%8B%A8%EC%A0%90-%EB%9C%BB%EC%A0%95%EB%A6%AC/)
- [함수형 컴포넌트 vs 클래스형 컴포넌트](https://born-dev.tistory.com/27)
- [React란 무엇인가?](https://shin1303.tistory.com/entry/React-React%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C)
