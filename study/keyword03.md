# KEYWORD 03
<br>

### 🗝 **[1/5일 STUDY KEYWORD](study/keyword03.md)**
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

<br>


## npm

- Node Package Manager
- 자바스크립트 프로그래밍 언어를 위핸 패키지 관리자
- 패키지를 관리해주는 도구
- 자바스크립트 런타임 환경 node.js의 기본 패키지 관리자
- node.js 에서 사용하는 모듈들을 패키지로 만들어 npm을 통하여 관리하고 배포
    - 모듈 → 애플리케이션을 구성하는 개별적 요소
- 다른 사람들이 만들어 놓은 모듈들 npm으로 설치하여 사용
- 설치한 모듈이 사용하고 있는 다른 모듈의 의존성 또한 자동으로 해결해줌
- 다른 언어들의 비슷한 개념
    - ruby의 Gem
    - php의 Composer
    - C#의 NuGet
    - java의 Jpm
    - python의 pip

### 버전

- [**LTS**(Long Term Supported) 버전] - (프론트엔드 개발 추천)
    
    짝수 버전이 LTS 버전(현재 4.X)
    
    안정성과 보안성에 초점을 두어 개발
    
- [**Stable** 버전] - (서버)
    
    Stable 버전은 잦은 업데이트를 진행
    
    홀수 버전(현재 6.X)
    

### 모듈화와 CommonJs

- 자바스크립트는 웹페이지에 있어서 보조적인 기능을 수행하기 위해 한정적인 용도로 만들어진 태생적 한계로 다른 언어에 비해 부족한(나쁜) 부분이 있는 것이 사실이다. 그 대표적인 것이 모듈 기능이 없는 것이다.
- C언어는 #include, Java는 import 등 대부분의 언어는 모듈 기능을 가지고 있다. 하지만 Client-side JavaScript의 경우, script 태그를 사용하여 외부의 스크립트 파일을 가져올 수는 있지만 파일마다 독립적인 파일 Scope를 갖지 않고 하나의 전역 객체(Global Object)에 바인딩되기 때문에 전역변수가 중복되는 등의 문제가 발생할 수 있다. 이것으로는 모듈화를 구현할 수 없다.
- JavaScript를 Client-side에 국한하지 않고 범용적으로 사용하고자 하는 움직임이 생기면서 모듈 기능은 반드시 해결해야하는 핵심 과제가 되었고 이런 상황에서 제안된 것이 [CommonJS](http://www.commonjs.org/)와 [AMD(Asynchronous Module Definition)](https://github.com/amdjs/amdjs-api/wiki/AMD)이다.
- CommonJS과 AMD는 사양(spec)으로 CommonJS 또는 AMD라는 라이브러리가 존재하는 것은 아니다.
- CommonJS 방식은 AMD에 비해 문법이 간단하며 동기 방식(synchronous loading)으로 동작한다.
- AMD 방식은 CommonJS에 비해 문법이 다소 까다로우며 CommonJS와는 달리 비동기 방식(asynchronous loading)으로 동작한다. AMD 방식을 지원하는 대표적인 모듈 로더는 [RequireJS](http://requirejs.org/)이다.
- Node.js는 사실상 모듈 시스템의 사실상 표준(de facto standard)인 CommonJS를 채택하였고 현재는 독자적인 진화를 거쳐 CommonJS 사양과 100% 동일하지는 않지만 기본적으로 CommonJS 방식을 따르고 있다. Node.js에서 모듈의 사용 방법에 대해서는 [Node.js module](https://poiemaweb.com/nodejs-module)을 참고하기 바란다.
- 브라우저에서의 모듈 사용은 대부분의 브라우저가 ES6의 모듈을 지원하지 않고 있으므로 [Browserify](http://browserify.org/) 또는 [webpack](https://webpack.github.io/)과 같은 모듈 번들러를 사용하여야 한다.

## webpack
- **번들러~**
- **JavaScript 모듈화 도구**
- JavaScript는 언어 자체가 지원하는 모듈 시스템이 없습니다. 이런 한계를 극복하려 여러 가지 도구를 활용하는데 그 도구 가운데 하나가 **webpack**
- [Node.js](https://nodejs.org/)가 설치된 환경에서 실행 가능

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/70d62db6-35aa-498e-a82e-25bb4daed378/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074255Z&X-Amz-Expires=86400&X-Amz-Signature=4b3943981e535ff90131f6cbd8dca1253dde54204ba4e4aa40496d863afef9cd&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- webpack을 사용할 때 브라우저에서 실행되는 코드는 실제 작성한 코드가 아니라 webpack으로 컴파일된 코드

### 장점

- 모듈 시스템을 구성하는 기능
- 로더 사용
- 빠른 컴파일 속도

### webpack 사용방법

- **엔트리 파일 →** 다음 그림과 같이 서로 의존 관계에 있는 다양한 모듈을 사용하는 시작점이 되는 파일
- **번들 파일 →** 브라우저에서 실행할 수 있게 모듈을 컴파일한 파일

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/f41490b5-cb52-419d-947f-ca947a19e92c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074404Z&X-Amz-Expires=86400&X-Amz-Signature=353c9eb7ad1325bb3c0d035c5edda5b41fd5ef13bfbeaa3a0d268d54d439183a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- webpack에서 컴파일은 엔트리 파일을 시작으로 의존 관계에 있는 모듈을 엮어서 하나의 번들 파일을 만드는 작업
- JavaScript를 사용하는 HTML 코드에서는 컴파일 결과로 만들어진 번들 파일만 포함하면 됨

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/fe7ed023-e492-4c9f-877a-be274f04c80c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074419Z&X-Amz-Expires=86400&X-Amz-Signature=cb3afadfd139eff1c7607ed27fae655b1af13bb36c7d2a5934ccd1954525d768&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- 엔트리 파일이 여러 개일 때는 엔트리 파일마다 번들 파일이 생성

[https://d2.naver.com/helloworld/0239818](https://d2.naver.com/helloworld/0239818)

여담

- 웹을 개발하다보면 다양한 확장자의 파일을 만들게 된다. 이렇게 다양한 소스는 웹 어플리케이션을 무겁게 만든다. 통신이 있을 때마다 이 소스들을 로딩하는 작업은 고비용이다. 많은 JS 패키지를 사용하다보면 예상하지 못한 충돌로 인해 어플리케이션이 깨지게 될 수도 있다(같은 이름을 변수를 사용하는 등). 이를 해결하기 위해 등장한 도구가 Bundler이다. bundle은 묶는다는 뜻이다. **여러개의 파일을 묶어주는 어떠한 정리 방법**이다. 구체적인 기술로는 WebPack, Broserify, Parcel이 있다. WebPack은 가장 인기있는 도구이다. 하나의 JS파일에 .js뿐만 아니라 .css나 image파일 등을 모듈을 모두 몰아넣을 수 있다. 동시에 성능을 향상시키기 위해 필요하다면 다시 분리할 수 있다. 특히, WebPack을 둘러싼 방대한 생태계 덕분에 다양한 확장 기능 등이 있다. 따라서 많은 작업들을 자동화 시킬 수 있다.

### SPA

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/52d72e86-78b8-40ec-add1-edae7209ec18/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T082626Z&X-Amz-Expires=86400&X-Amz-Signature=702a5815794c1120fd504b2bb0da2b5a5311cf8daf3a77776b3dfc458d45d4e6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- SPA(Single Page Application)는 한 개(Single)의 Page로 구성된 Application
- 웹 에플리케이션에 필요한 **모든 정적 리소스를 최초 한 번에 다운로드**
- 그 후에는 데이터를 받아올 때만 서버와 통신
- 그 이후 새로운 페이지 요청이 있을 때, 페이지 갱신에 **필요한 데이터만 전달 받아서 페이지를 갱신**
- 필요한 부분만 갱신하기 때문에 네이티브 앱에 가까운 자연스러운 페이지 이동과 사용자 경험(UX)을 제공

⇒ SPA를 **CSR(Client Side Rendering)** 방식으로 렌더링이라 함

### 장점

- 자연스러운 사용자 경험 (UX) → 전체 페이지를 업데이트 할 필요가 없기 때문에 빠르고 ‘깜빡’ 거림이 없음
- 필요한 리소스만 부분적으로 로딩 (성능) → SPA의 Application은 서버에게 정적리소스를 한 번만 요청 그리고 받은 데이터는 전부 저장**(캐시=Cache)**
- 서버의 템플릿 연산을 클라이언트로 분산 (성능)
- 컴포넌트별 개발 용이 (생산성)
- 모바일 앱 개발을 염두에 둔다면 동일한 API를 사용하도록 설계 가능 (생산성)

### 단점

- JavaScript 파일을 번들링해서 한 번에 받기 때문에 초기 구동 속도가 느림 (Webpack의 code splitting으로 해결 가능)
- 검색엔진최적화(SEO)가 어려움 (SSR로 해결 가능) → SPA 앱을 검색로봇 입장에서 보면 모든 페이지의 소스가 아래와 같이 보임, 검색엔진이 색인을 할 만한 컨텐츠가 존재하지 않는 것
    
    ```html
    <html>
    <head>
      <title>Single Page Application</title>
      <link rel="stylesheet" href="app.css" type="text/css">
    </head>
    <body>
      <div id="app"></div>
      <script src="app.js"></script>
    </body>
    </html>
    ```
    

### **SPA 방식이 모두 CSR인 것은 아님**

### MPA

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/70ca152a-8f1f-4dff-b9f8-e5ed0dab1b2e/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T082643Z&X-Amz-Expires=86400&X-Amz-Signature=ac9d74de29283ee4893004ed3134cb922bdd2ff55d12b13d0b7c036c099dc0df&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- MPA(Multiple Page Application)는 여러 개(Multiple)의 Page로 구성된 Application
- **새로운 페이지를 요청**할 때마다 **정적 리소스(HTML, CSS, JavaScript)**가 다운로드
- **매번 전체 페이지가 다시 렌더링**

⇒ MPA를 **SSR(Server Side Rendering)** 방식으로 렌더링이라 함

### 장점

- SEO 관점에서 유리 → MPA는 완성된 형태의 HTML 파일을 서버로부터 전달받음 따라서 검색엔진이 페이지를 크롤링하기에 적합
- 첫 로딩이 매우 짧음 → 서버에서 이미 렌더링해 가져오기 때문, 그러나 클라이언트가 JS 파일을 모두 다운로드하고 적용하기전 까지는 각각의 기능은 동작하지 않음

### 단점

- 새로운 페이지를 이동하면 ‘깜빡’인다 (UX) → 매 페이지 요청마다 리로딩(새로고침) 발생, 새로운 페이지를 요청할 때마다 전체 페이지를 다시 렌더링하기 때문
- 페에지 이동시 불필요한 템플릿도 중복해서 로딩 (성능)
- 서버 렌더링에 따른 부하
- 모바일 앱 개발시 추가적인 백엔드 작업 필요 (생산성) 개발이 복잡해질 수 있음

### SSR, CSR 차이 → 초기렌더링속도, SEO, 보안

### SSR이 렌더링 하는 방식

- 모든 템플릿은 서버 연산을 통해서 렌더링하고 완성된 페이지 형태로 응답 → 이 과정을 **서버 사이드 렌더링(SSR)**이라고 부름

### CSR이 렌더링하는 방식

- 최초에 한번 서버에서 전체 페이지를 로딩하여 보여주고 이후에는 사용자의 요청이 올 때마다, 리소스를 서버에서 제공한 후 클라이언트가 해석하고 렌더링하는 방식

## package.json

- 프로젝트의 정보를 정의하고, 의존하는 **패키지 버전 정보**를 명시하는 파일
- 배포한 모듈 정보를 담고자 만들어짐
- 노드로 작성하는 애플리케이션도 package.json 파일을 사용하여 관리할 수 있음
- 사용하는 확장 모듈에 대한 의존성 관리가 가능하기 때문에 편리해짐

### 영역

- 프로젝트의 정보 - name, version 영역
- 패키지 버전 정보 - **dependencies 또는 devDependencies** 영역

### 패키지 지정

- "dependencies": **프로덕션 환경**에서 응용 프로그램에 필요한 패키지
- "devDependencies": **로컬 개발 및 테스트**에만 필요한 패키지

### 시멘틱 버저닝 규칙

**틸드(~)**

```json
"devDependencies": {
  "@vue/cli-service": "~4.3.0",
},
```

- 해당 패키지의 패치 레벨 변경을 허용하겠다는 의미
- 즉, 4.4.0 미만의 패치 레벨 변경을 허용하겠다는 의미

**캐럿(^)**

```json
"dependencies": {
  "vue": "^2.6.11"
}
```

- 해당 패캐지의 마이너, 패치 변경을 허용하겠다는 의미
- 즉, 3.0.0 미만의 마이너, 패치 변경을 허용하겠다는 의미

## 컴포넌트

### 기본구조

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/5c9fd55b-16b0-444b-a9e7-8bc7c264c537/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074448Z&X-Amz-Expires=86400&X-Amz-Signature=e07ea3936693d45fb53558d0aa23847354b9b947cb53cdc18b0d7a42b3463e7d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- 클래스형 컴포넌트 → render 함수를 사용해서 retrun안의 코드를 화면에 보이도록 함
- 함수형 컴포넌트 → 자신이 렌더 함수이기 때문에 render 함수 사용없이 return 값만 사용

### props 값 전달 받기

- App.js 설정 → App.js 컴포넌트는 함수형 컴포넌트로 구현

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/130d7713-cc3c-4a8f-b94a-3281b37174bc/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074504Z&X-Amz-Expires=86400&X-Amz-Signature=2f0a59f0aaf79c011f64b912a23e3eed729d4c11c0f615eee3e8b51b367242e6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- 클래스형 컴포넌트 → 클래스형 컴포넌트에서 부모 컴포넌트에서 정의한 props 값을 {this.props.props이름}으로 받아서 씀

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/dc9893f0-e9cb-4b3b-89cb-776aba00cd95/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074522Z&X-Amz-Expires=86400&X-Amz-Signature=afe67925db480ecadf89824647a762a6a60abd28a9d44326e33a44e0934ab62d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- 함수형 컴포넌트 → 함수형 컴포넌트에서 정의한 props 값은 함수의 인자값(파라미터)으로 받아옴 즉, 부모 컴포넌트에서 전달받은 props 값을 함수형 컴포넌트의 인자로 설정하여 함수 내부에 props 값을 전달해서 화면에 나타나게 하는 것

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/8deaea4e-b8ce-4cbf-a476-b653fb2b00a6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074534Z&X-Amz-Expires=86400&X-Amz-Signature=f129b2ec851be614174293ecb8ec5eaeac70e945d860214b1799d825e5ada749&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)
