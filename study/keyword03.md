# KEYWORD 03
<br>

### ๐ **[1/5์ผ STUDY KEYWORD](study/keyword03.md)**
```
npm ,webpack , package.json, ํด๋์คํ ์ปดํฌ๋ํธ, ํจ์ํ ์ปดํฌ๋ํธ
```
<br>

### * npm ์ด๋?
- #### npm์ด๋ Node Package Manager์ ์ฝ์๋ก, ๋ธ๋์ ํจํค์ง ๋งค๋์ ์ด๋ค. 
- #### ๋ค๋ฅธ ์ฌ๋๋ค์ด ๋ง๋  ์์ค ์ฝ๋๋ค์ ๋ชจ์๋ ์ ์ฅ์.
- ๋จ์ ์ฝ๋๋ฅผ ์ฌ์ฉํ์ฌ ํ๋ก๊ทธ๋๋ฐ ๊ฐ๋ฅ
- ์ด๋ฏธ ์๋ ๊ธฐ๋ฅ์ ๋ค์ ๊ตฌํํ  ํ์๊ฐ ์์ด ํจ์จ์ ์ด๋ค.
- ์คํ ์์ค ์ํ๊ณ๋ฅผ ๊ตฌ์ฑ์ค
- ํจํค์ง : npm์ ์๋ก๋๋ ๋ธ๋ ๋ชจ๋
- ๋ชจ๋์ด ๋ค๋ฅธ ๋ชจ๋์ ์ฌ์ฉํ  ์ ์๋ฏ, ํจํค์ง๋ ๋ค๋ฅธ ํจํค์ง๋ฅผ ์ฌ์ฉํ  ์ ์๋ค.
 
```
//npm์ ํตํด ์ค์นํ ๋ชจ๋(ํจํค์ง) ๋ค์ Common JS์ ๋ฌธ๋ฒ ํ์์ผ๋ก ๋ถ๋ฌ์ ์ธ ์ ์๋ค. ํ์์ ๋ค์๊ณผ ๊ฐ๋ค
//npm install์ ํตํด ๋ค์ด๋ฐ์ express๋ฅผ ์ฌ์ฉํ๊ณ  ์ถ๋ค๋ฉด

var express = require('express');
```
<br>


### * package.json ์ด๋?
- #### ํ์ฌ ํ๋ก์ ํธ์ ๋ํ ์ ๋ณด์ ์ฌ์ฉ ์ค์ธ ํจํค์ง์ ๋ํ ์ ๋ณด๋ฅผ ๋ด์ ํ์ผ.
- #### ํ๋ก์ ํธ(ํด๋น ๋๋ ํ ๋ฆฌ)๊ฐ ์์กดํ๊ณ  ์๋ ๋ชจ๋๋ค์ ๋ชฉ๋ก๊ณผ ๋ฒ์ ์ ๋ณด๋ฅผ ์ ๊ณต
- ๊ฐ์ ํจํค์ง๋ผ๋ ๋ฒ์ ๋ณ๋ก ๊ธฐ๋ฅ์ด ๋ค๋ฅผ ์ ์์ผ๋ฏ๋ก ๋ฒ์ ์ ๊ธฐ๋กํด๋์ด์ผ ํจ
- ๋์ผํ ๋ฒ์ ์ ์ค์นํ์ง ์์ผ๋ฉด ๋ฌธ์ ๊ฐ ์๊ธธ ์ ์๋ค.
- ๋ธ๋ ํ๋ก์ ํธ ์์ ์  package.json๋ถํฐ ๋ง๋ค๊ณ  ์์ํจ (package.json ์์ฑ ๋ช๋ น์ด : npm init)

<br>

### * webpack ์ด๋?
<img width="600" alt="1_F070uzOYIL8LXzAGf5zy9A" src="https://user-images.githubusercontent.com/76805997/148311774-59766a42-579e-4cb7-b70f-c2e577937133.png">

- #### ์นํฉ์ ์คํ ์์ค ์๋ฐ์คํฌ๋ฆฝํธ ๋ชจ๋ ๋ฒ๋ค๋ฌ
- ์ฌ๋ฌ๊ฐ๋ก ๋๋์ด์ ธ ์๋ ํ์ผ๋ค์ ํ๋์ ์๋ฐ์คํฌ๋ฆฝํธ ์ฝ๋๋ก ์์ถํ๊ณ  ์ต์ ํํ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ
- ์ฌ๋ฌ ํ์ผ์ ์๋ฐ์คํฌ๋ฆฝํธ ์ฝ๋๋ฅผ ์์ถํ์ฌ ์ต์ ํ ํ  ์ ์๊ธฐ ๋๋ฌธ์ ๋ก๋ฉ์ ๋ํ ๋คํธ์ํฌ ๋น์ฉ์ ์ค์ผ ์ ์์
- ๋ชจ๋ ๋จ์๋ก ๊ฐ๋ฐ์ด ๊ฐ๋ฅํ์ฌ, ๊ฐ๋์ฑ๊ณผ ์ ์ง๋ณด์๊ฐ ์ฌ์
<br>

### * Webpack์ ์ ์ฌ์ฉํด์ผ ํ ๊น ?
- ์๋ ์๋ ํ์ด์ง๋ง๋ค ์๋ก์ด html์ ์์ฒญํด์๋ฟ๋ ค ์ฃผ๋ ๋ฐฉ์์ด์๋ค๋ฉด, ์์๋ SPA ํ๋์ html ํ์ด์ง์ ์ฌ๋ฌ๊ฐ์ ์๋ฐ์คํฌ๋ฆฝํธ ํ์ผ๋ค์ด ํฌํจํ๋ค. ์ฐ๊ด ๋์ด ์๋ ์๋ฐ์คํฌ๋ฆฝํธ ์ข์์ฑ ์๋ ํ์ผ๋ค์ ํ๋์ ํ์ผ๋ก ๋ฌถ์ด์ค์ ๊ด๋ฆฌํ๊ธฐ ํธํ๋ค.
- ํ์ผ์ ์ปดํ์ผ ํ  ๋, ์ฌ๋ฌ ๋ชจ๋๋ค์ ํ์ผ์ ์ฝ์ด์ค๋๋ฐ ์๊ฐ์ด ์ค๋ ๊ฑธ๋ฆฐ๋ค. ๊ทธ ๋ถ๋ถ์ ํด๊ฒฐํ๊ธฐ ์ํด ์ฌ๋ฌ ํ์ผ์ ํ๋์ ํ์ผ๋ก ๋ฒ๋ค๋ง ํด์ค๋ค.
- ํ๋์ ์๋ฐ์คํฌ๋ฆฝํธ ํ์ผ๋ก ๋ง๋ค์ด์ ๋คํธ์ํฌ ์ ์์ ๋ถ๋ด์ ์ค์ด๊ณ  , ๋ ๋น ๋ฅธ ์๋น์ค ์ ๊ณต ๊ฐ๋ฅ
<br>

### * SPA vs MPA
- SPA(Single Page Application)๋ ํ ๊ฐ(Single)์ Page๋ก ๊ตฌ์ฑ๋ Application์ด๋ค.
- MPA(Multiple Page Application)๋ ์ฌ๋ฌ ๊ฐ(Single)์ Page๋ก ๊ตฌ์ฑ๋ Application์ด๋ค.
- MPA๋ ์๋ก์ด ํ์ด์ง๋ฅผ ์์ฒญํ  ๋๋ง๋ค ์ ์  ๋ฆฌ์์ค๊ฐ ๋ค์ด๋ก๋๋๋ค. ๋งค๋ฒ ์ ์ฒด ํ์ด์ง๊ฐ ๋ค์ ๋ ๋๋ง ๋๋ค.
- #### ๋ฐ๋ฉด SPA๋ ์น ์ํ๋ฆฌ์ผ์ด์์ ํ์ํ ๋ชจ๋  ์ ์  ๋ฆฌ์์ค๋ฅผ ์ต์ด ํ ๋ฒ์ ๋ค์ด๋ก๋ํ๋ค.
- #### ๊ทธ ์ดํ ์๋ก์ด ํ์ด์ง ์์ฒญ์ด ์์ ๋, ํ์ด์ง ๊ฐฑ์ ์ ํ์ํ ๋ฐ์ดํฐ๋ง ์ ๋ฌ ๋ฐ์์ ํ์ด์ง๋ฅผ ๊ฐฑ์ ํ๋ค.
- ๊ทธ๋์ SPA๋ฅผ CSR(Client Side Rendering) ๋ฐฉ์์ผ๋ก ๋ ๋๋งํ๋ค๊ณ  ๋งํ๋ค.
- ๊ทธ๋์ MPA๋ฅผ SSR(Server Side Rendering) ๋ฐฉ์์ผ๋ก ๋ ๋๋งํ๋ค๊ณ  ๋งํ๋ค.
<br>

### * ์ปดํฌ๋ํธ(Component)๋?
- ๋ฆฌ์กํธ๋ก ๋ง๋ค์ด์ง ์ฑ์ ์ด๋ฃจ๋ ์ต์ํ์ ๋จ์
- ์ปดํฌ๋ํธ๋ ๋ฐ์ดํฐ(props)๋ฅผ ์๋ ฅ๋ฐ์ View(state) ์ํ์ ๋ฐ๋ผ DOM Node๋ฅผ ์ถ๋ ฅํ๋ ํจ์.
- ๊ทธ๋์ ํฉ์ฑ์ ํตํด UI๋ฅผ ์ฌ์ฌ์ฉํ  ์ ์๊ณ , ๋๋ฆฝ์ ์ธ ๋จ์๋ก ์ชผ๊ฐ์ด ์๊ฐํ  ์ ์๊ฒ ํ๋ค.  
<br>


### * ํด๋์คํ ์ปดํฌ๋ํธ vs ํจ์ํ ์ปดํฌ๋ํธ?

### ๐ฉ 1) ์ฐจ์ด: ์ ์ธ๋ฐฉ์

#### (1) ํด๋์คํ ์ปดํฌ๋ํธ

![1](https://user-images.githubusercontent.com/76805997/148317012-d1921af7-5efd-4603-b77f-258034f4850f.png)

1. class ํค์๋ ํ์
2. Component๋ก ์์์ ๋ฐ์์ผํ๋ค.
3. render() ๋ฉ์๋๊ฐ ๋ฐ๋์ ํ์ํ๋ค.
4. state, lifeCycle ๊ด๋ จ ๊ธฐ๋ฅ์ฌ์ฉ์ด ๊ฐ๋ฅํ๋ค.
5. ํจ์ํ๋ณด๋ค ๋ฉ๋ชจ๋ฆฌ ์์์ ๋ ์ฌ์ฉํ๋ค.
6. ์์ ๋ฉ์๋๋ฅผ ์ ์ํ  ์ ์๋ค.


#### (2) ํจ์ํ ์ปดํฌ๋ํธ

![2](https://user-images.githubusercontent.com/76805997/148317088-e05ca3ee-30ff-4f96-a518-38f85a62d3b2.png)

1. state, lifeCycle ๊ด๋ จ ๊ธฐ๋ฅ์ฌ์ฉ ๋ถ๊ฐ๋ฅํ๋ค. [Hook์ ํตํด ํด๊ฒฐ]
2. ํด๋์คํ๋ณด๋ค ๋ฉ๋ชจ์ง ์์์ ๋ ์ฌ์ฉํ๋ค.
3. ์ปดํฌ๋ํธ ์ ์ธ์ด ํธํ๋ค.

<br>


###  ๐ฉ2) ์ฐจ์ด: State
- State ๋? ์ปดํฌ๋ํธ ๋ด๋ถ์์ ๋ฐ๋ ์ ์๋ ๊ฐ


#### (1) ํด๋์คํ ์ปดํฌ๋ํธ

![3](https://user-images.githubusercontent.com/76805997/148317716-a04e8b03-3409-4e61-ba72-d92b28cd9930.png)

1. constructor ์์์ this.state ์ด๊ธฐ ๊ฐ ์ค์  ๊ฐ๋ฅ
2. counstructor ์์ด๋ ๋ฐ๋ก state ์ด๊ธฐ๊ฐ์ ์ค์  ๊ฐ๋ฅ
3. this.setState() ๋ฅผ ํตํด state๊ฐ์ ๋ณ๊ฒฝ
4. ํด๋์คํ์ state๋ ๊ฐ์ฒดํ์

#### (2) ํจ์ํ ์ปดํฌ๋ํธ

![4](https://user-images.githubusercontent.com/76805997/148317717-f6e84398-97ca-48dc-95ae-535b2292315a.png)

1. useState ํจ์๋ก state๋ฅผ ์ฌ์ฉํ๋ค.
2. useState ํจ์๋ฅผ ํธ์ถํ๋ฉด ๋ฐฐ์ด์ด ๋ฐํ๋๋๋ฐ ์ฒซ ๋ฒ์งธ ์์๋ ํ์ฌ ์ํ, ๋๋ฒ์งธ ์์๋ ์ํ๋ฅผ ๋ฐ๊ฟ์ฃผ๋ ํจ์์ด๋ค.
<br>

### ๐ฉ 3) ์ฐจ์ด: props
- Props ๋? ์ปดํฌ๋ํธ์ ์์ฑ์ ์ค์ 


#### (1) ํด๋์คํ ์ปดํฌ๋ํธ

![5](https://user-images.githubusercontent.com/76805997/148318028-13755ecd-f092-4cf0-beff-92dbfe525c43.png)
1. this.props๋ก ํตํด ๊ฐ์ ๋ถ๋ฌ์ฌ ์ ์๋ค.

#### (2) ํจ์ํ ์ปดํฌ๋ํธ

![6](https://user-images.githubusercontent.com/76805997/148318030-458db084-758e-4085-9989-f066f6e20901.png)

1. props๋ฅผ ๋ถ๋ฌ์ฌ ํ์ ์์ด ๋ฐ๋ก ํธ์ถ ํ  ์ ์๋ค.
<br>

###  ๐ฉ4) ์ฐจ์ด: ์ด๋ฒคํธ ํธ๋ค๋ง

#### (1) ํด๋์คํ ์ปดํฌ๋ํธ

![7](https://user-images.githubusercontent.com/76805997/148318561-aa8e2f00-c78b-4d2d-94b3-a1af393748ec.png)

1. ํจ์ ์ ์ธ์ ํ์ดํ ํจ์๋ก ๋ฐ๋ก ์ ์ธ ๊ฐ๋ฅํ๋ค.
2. ์์์ ์ ์ฉํ ๋ this.๋ฅผ ๋ถ์ฌ์ค์ผํ๋ค.

#### (2) ํจ์ํ ์ปดํฌ๋ํธ

![8](https://user-images.githubusercontent.com/76805997/148318569-d487dfa3-eb91-4263-8903-3733cd90f1c6.png)

1. const + ํจ์ ํํ๋ก ์ ์ธํด์ผ ํ๋ค.
2. ์์์ ์ ์ฉํ ๋ this๊ฐ ํ์์๋ค.
<br>

###  ๐ฉ5) ์ฐจ์ด: Life Cycle
* #### Life Cycle ์ด๋?
- React์์ ์ปดํฌ๋ํธ๋ ์ฌ๋ฌ ์ข๋ฅ์ "์๋ช์ฃผ๊ธฐ ๋ฉ์๋" ๋ฅผ ๊ฐ์ง๋ฉฐ ์ด ๋ฉ์๋๋ฅผ ์ค๋ฒ๋ผ์ด๋ฉ(์์ํ์ฌ ์ฌ์ ์) ํ์ฌ ํน์  ์์ ์ ์ฝ๋๊ฐ ์คํ๋๋๋ก ์ค์  ํฉ๋๋ค.
- ํด๋์ค ์ปดํฌ๋ํธ์๋ง ํด๋น๋๋ ๋ด์ฉ์ด๋ฉฐ, ํจ์ํ ์ปดํฌ๋ํธ๋ Hook๋ฅผ ์ฌ์ฉํ์ฌ ์๋ช์ฃผ๊ธฐ์ ์ํ๋ ๋์์ ํฉ๋๋ค
<br>

### * ํจ์ํ ์ปดํฌ๋ํธ๋ฅผ ์ ํธํ๋ ์ด์ ?
- ํด๋์คํ ์ปดํฌ๋ํธ๋ ๋ก์ง๊ณผ ์ํ๋ฅผ ์ปดํฌ๋ํธ ๋ด์์ ๊ตฌํํ๊ธฐ ๋๋ฌธ์ ์๋์ ์ผ๋ก ๋ณต์กํ UI ๋ก์ง์ ๊ฐ๊ณ  ์๋ ๋ฐ๋ฉด,
- ํจ์ํ ์ปดํฌ๋ํธ๋ state๋ฅผ ์ฌ์ฉํ์ง ์๊ณ  ๋จ์ํ๊ฒ ๋ฐ์ดํฐ๋ฅผ ๋ฐ์์(props) UI์ ๋ฟ๋ ค์ค๋ค. 
- Hook๋ค์ ํ์ํ ๊ณณ์ ์ฌ์ฉํ๋ฉฐ Logic์ ์ฌ์ฌ์ฉ์ด ๊ฐ๋ฅํ๋ค๋ ์ฅ์ ์ด ์์ด ํจ์ํ ์ปดํฌ๋ํธ+Hook์ ์ฃผ๋ก ์ฌ์ฉํ๋ค๊ณ  ํ๋ค.
<br>

### * Props and state?
1. #### ๊ณตํต์ 
> ๋ ๊ฐ์ฒด ๋ชจ๋ ๋ ๋๋ง ๊ฒฐ๊ณผ๋ฌผ์ ์ํฅ์ ์ฃผ๋ ์ ๋ณด๋ฅผ ๊ฐ์ง๊ณ  ์๋ค.
2. #### ์ฐจ์ด์ 
> - props๋ (like ํจ์ ๋งค๊ฐ๋ณ์) Component์ ์ ๋ฌ๋๋ค.
> - state๋ (like ํจ์ ๋ด์ ์ ์ธ๋ ๋ณ์) Component์์์ ๊ด๋ฆฌ๋๋ค.
3. #### props
- ๋ถ๋ชจ Component-> ์์ Component๋ก ์ ๋ฌํด์ฃผ๋ ์ฝ๊ธฐ ์ ์ฉ ๋ฐ์ดํฐ.
- ์์ Component์์ props๋ ๋ณ๊ฒฝ์ด ๋ถ๊ฐ๋ฅํ๊ณ , props๋ฅผ ์ ๋ฌํด์ค ์ต์์ ๋ถ๋ชจ component๋ง ๋ณ๊ฒฝ๊ฐ๋ฅ
4. #### state
- ๋์ ์ธ ๋ฐ์ดํฐ๋ฅผ ๋ค๋ฃฐ ๋ ์ฌ์ฉ.
- ๋๋ฆฝ์ ์ด๋ผ ๋ค๋ฅธ component์ ์ ๊ทผ์ด ๋ถ๊ฐ๋ฅ
<br>

### ์ฐธ๊ณ 
- [SPA vs MPA์ SSR vs CSR ์ฅ๋จ์  ๋ป์ ๋ฆฌ](https://hanamon.kr/spa-mpa-ssr-csr-%EC%9E%A5%EB%8B%A8%EC%A0%90-%EB%9C%BB%EC%A0%95%EB%A6%AC/)
- [ํจ์ํ ์ปดํฌ๋ํธ vs ํด๋์คํ ์ปดํฌ๋ํธ](https://born-dev.tistory.com/27)
- [React๋ ๋ฌด์์ธ๊ฐ?](https://shin1303.tistory.com/entry/React-React%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C)

<br>


## npm

- Node Package Manager
- ์๋ฐ์คํฌ๋ฆฝํธ ํ๋ก๊ทธ๋๋ฐ ์ธ์ด๋ฅผ ์ํธ ํจํค์ง ๊ด๋ฆฌ์
- ํจํค์ง๋ฅผ ๊ด๋ฆฌํด์ฃผ๋ ๋๊ตฌ
- ์๋ฐ์คํฌ๋ฆฝํธ ๋ฐํ์ ํ๊ฒฝ node.js์ ๊ธฐ๋ณธ ํจํค์ง ๊ด๋ฆฌ์
- node.js ์์ ์ฌ์ฉํ๋ ๋ชจ๋๋ค์ ํจํค์ง๋ก ๋ง๋ค์ด npm์ ํตํ์ฌ ๊ด๋ฆฌํ๊ณ  ๋ฐฐํฌ
    - ๋ชจ๋ โ ์ ํ๋ฆฌ์ผ์ด์์ ๊ตฌ์ฑํ๋ ๊ฐ๋ณ์  ์์
- ๋ค๋ฅธ ์ฌ๋๋ค์ด ๋ง๋ค์ด ๋์ ๋ชจ๋๋ค npm์ผ๋ก ์ค์นํ์ฌ ์ฌ์ฉ
- ์ค์นํ ๋ชจ๋์ด ์ฌ์ฉํ๊ณ  ์๋ ๋ค๋ฅธ ๋ชจ๋์ ์์กด์ฑ ๋ํ ์๋์ผ๋ก ํด๊ฒฐํด์ค
- ๋ค๋ฅธ ์ธ์ด๋ค์ ๋น์ทํ ๊ฐ๋
    - ruby์ Gem
    - php์ Composer
    - C#์ NuGet
    - java์ Jpm
    - python์ pip

### ๋ฒ์ 

- [**LTS**(Long Term Supported) ๋ฒ์ ] - (ํ๋ก ํธ์๋ ๊ฐ๋ฐ ์ถ์ฒ)
    
    ์ง์ ๋ฒ์ ์ด LTS ๋ฒ์ (ํ์ฌ 4.X)
    
    ์์ ์ฑ๊ณผ ๋ณด์์ฑ์ ์ด์ ์ ๋์ด ๊ฐ๋ฐ
    
- [**Stable**ย ๋ฒ์ ] - (์๋ฒ)
    
    Stable ๋ฒ์ ์ ์ฆ์ ์๋ฐ์ดํธ๋ฅผ ์งํ
    
    ํ์ ๋ฒ์ (ํ์ฌ 6.X)
    

### ๋ชจ๋ํ์ CommonJs

- ์๋ฐ์คํฌ๋ฆฝํธ๋ ์นํ์ด์ง์ ์์ด์ ๋ณด์กฐ์ ์ธ ๊ธฐ๋ฅ์ ์ํํ๊ธฐ ์ํด ํ์ ์ ์ธ ์ฉ๋๋ก ๋ง๋ค์ด์ง ํ์์  ํ๊ณ๋ก ๋ค๋ฅธ ์ธ์ด์ ๋นํด ๋ถ์กฑํ(๋์) ๋ถ๋ถ์ด ์๋ ๊ฒ์ด ์ฌ์ค์ด๋ค. ๊ทธ ๋ํ์ ์ธ ๊ฒ์ด ๋ชจ๋ ๊ธฐ๋ฅ์ด ์๋ ๊ฒ์ด๋ค.
- C์ธ์ด๋ #include, Java๋ import ๋ฑ ๋๋ถ๋ถ์ ์ธ์ด๋ ๋ชจ๋ ๊ธฐ๋ฅ์ ๊ฐ์ง๊ณ  ์๋ค. ํ์ง๋ง Client-side JavaScript์ ๊ฒฝ์ฐ, script ํ๊ทธ๋ฅผ ์ฌ์ฉํ์ฌ ์ธ๋ถ์ ์คํฌ๋ฆฝํธ ํ์ผ์ ๊ฐ์ ธ์ฌ ์๋ ์์ง๋ง ํ์ผ๋ง๋ค ๋๋ฆฝ์ ์ธ ํ์ผ Scope๋ฅผ ๊ฐ์ง ์๊ณ  ํ๋์ ์ ์ญ ๊ฐ์ฒด(Global Object)์ ๋ฐ์ธ๋ฉ๋๊ธฐ ๋๋ฌธ์ ์ ์ญ๋ณ์๊ฐ ์ค๋ณต๋๋ ๋ฑ์ ๋ฌธ์ ๊ฐ ๋ฐ์ํ  ์ ์๋ค. ์ด๊ฒ์ผ๋ก๋ ๋ชจ๋ํ๋ฅผ ๊ตฌํํ  ์ ์๋ค.
- JavaScript๋ฅผ Client-side์ ๊ตญํํ์ง ์๊ณ  ๋ฒ์ฉ์ ์ผ๋ก ์ฌ์ฉํ๊ณ ์ ํ๋ ์์ง์์ด ์๊ธฐ๋ฉด์ ๋ชจ๋ ๊ธฐ๋ฅ์ ๋ฐ๋์ ํด๊ฒฐํด์ผํ๋ ํต์ฌ ๊ณผ์ ๊ฐ ๋์๊ณ  ์ด๋ฐ ์ํฉ์์ ์ ์๋ ๊ฒ์ดย [CommonJS](http://www.commonjs.org/)์ย [AMD(Asynchronous Module Definition)](https://github.com/amdjs/amdjs-api/wiki/AMD)์ด๋ค.
- CommonJS๊ณผ AMD๋ ์ฌ์(spec)์ผ๋ก CommonJS ๋๋ AMD๋ผ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๊ฐ ์กด์ฌํ๋ ๊ฒ์ ์๋๋ค.
- CommonJS ๋ฐฉ์์ AMD์ ๋นํด ๋ฌธ๋ฒ์ด ๊ฐ๋จํ๋ฉฐ ๋๊ธฐ ๋ฐฉ์(synchronous loading)์ผ๋ก ๋์ํ๋ค.
- AMD ๋ฐฉ์์ CommonJS์ ๋นํด ๋ฌธ๋ฒ์ด ๋ค์ ๊น๋ค๋ก์ฐ๋ฉฐ CommonJS์๋ ๋ฌ๋ฆฌ ๋น๋๊ธฐ ๋ฐฉ์(asynchronous loading)์ผ๋ก ๋์ํ๋ค. AMD ๋ฐฉ์์ ์ง์ํ๋ ๋ํ์ ์ธ ๋ชจ๋ ๋ก๋๋ย [RequireJS](http://requirejs.org/)์ด๋ค.
- Node.js๋ ์ฌ์ค์ ๋ชจ๋ ์์คํ์ ์ฌ์ค์ ํ์ค(de facto standard)์ธ CommonJS๋ฅผ ์ฑํํ์๊ณ  ํ์ฌ๋ ๋์์ ์ธ ์งํ๋ฅผ ๊ฑฐ์ณ CommonJS ์ฌ์๊ณผ 100% ๋์ผํ์ง๋ ์์ง๋ง ๊ธฐ๋ณธ์ ์ผ๋ก CommonJS ๋ฐฉ์์ ๋ฐ๋ฅด๊ณ  ์๋ค. Node.js์์ ๋ชจ๋์ ์ฌ์ฉ ๋ฐฉ๋ฒ์ ๋ํด์๋ย [Node.js module](https://poiemaweb.com/nodejs-module)์ ์ฐธ๊ณ ํ๊ธฐ ๋ฐ๋๋ค.
- ๋ธ๋ผ์ฐ์ ์์์ ๋ชจ๋ ์ฌ์ฉ์ ๋๋ถ๋ถ์ ๋ธ๋ผ์ฐ์ ๊ฐ ES6์ ๋ชจ๋์ ์ง์ํ์ง ์๊ณ  ์์ผ๋ฏ๋กย [Browserify](http://browserify.org/)ย ๋๋ย [webpack](https://webpack.github.io/)๊ณผ ๊ฐ์ ๋ชจ๋ ๋ฒ๋ค๋ฌ๋ฅผ ์ฌ์ฉํ์ฌ์ผ ํ๋ค.

## webpack
- **๋ฒ๋ค๋ฌ~**
- **JavaScript ๋ชจ๋ํ ๋๊ตฌ**
- JavaScript๋ ์ธ์ด ์์ฒด๊ฐ ์ง์ํ๋ ๋ชจ๋ ์์คํ์ด ์์ต๋๋ค. ์ด๋ฐ ํ๊ณ๋ฅผ ๊ทน๋ณตํ๋ ค ์ฌ๋ฌ ๊ฐ์ง ๋๊ตฌ๋ฅผ ํ์ฉํ๋๋ฐ ๊ทธ ๋๊ตฌ ๊ฐ์ด๋ฐ ํ๋๊ฐ **webpack**
- [Node.js](https://nodejs.org/)๊ฐ ์ค์น๋ ํ๊ฒฝ์์ ์คํ ๊ฐ๋ฅ

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/70d62db6-35aa-498e-a82e-25bb4daed378/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074255Z&X-Amz-Expires=86400&X-Amz-Signature=4b3943981e535ff90131f6cbd8dca1253dde54204ba4e4aa40496d863afef9cd&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- webpack์ ์ฌ์ฉํ  ๋ ๋ธ๋ผ์ฐ์ ์์ ์คํ๋๋ ์ฝ๋๋ ์ค์  ์์ฑํ ์ฝ๋๊ฐ ์๋๋ผ webpack์ผ๋ก ์ปดํ์ผ๋ ์ฝ๋

### ์ฅ์ 

- ๋ชจ๋ ์์คํ์ ๊ตฌ์ฑํ๋ ๊ธฐ๋ฅ
- ๋ก๋ ์ฌ์ฉ
- ๋น ๋ฅธ ์ปดํ์ผ ์๋

### webpack ์ฌ์ฉ๋ฐฉ๋ฒ

- **์ํธ๋ฆฌ ํ์ผ โ** ๋ค์ ๊ทธ๋ฆผ๊ณผ ๊ฐ์ด ์๋ก ์์กด ๊ด๊ณ์ ์๋ ๋ค์ํ ๋ชจ๋์ ์ฌ์ฉํ๋ ์์์ ์ด ๋๋ ํ์ผ
- **๋ฒ๋ค ํ์ผ โ** ๋ธ๋ผ์ฐ์ ์์ ์คํํ  ์ ์๊ฒ ๋ชจ๋์ ์ปดํ์ผํ ํ์ผ

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/f41490b5-cb52-419d-947f-ca947a19e92c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074404Z&X-Amz-Expires=86400&X-Amz-Signature=353c9eb7ad1325bb3c0d035c5edda5b41fd5ef13bfbeaa3a0d268d54d439183a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- webpack์์ ์ปดํ์ผ์ ์ํธ๋ฆฌ ํ์ผ์ ์์์ผ๋ก ์์กด ๊ด๊ณ์ ์๋ ๋ชจ๋์ ์ฎ์ด์ ํ๋์ ๋ฒ๋ค ํ์ผ์ ๋ง๋๋ ์์
- JavaScript๋ฅผ ์ฌ์ฉํ๋ HTML ์ฝ๋์์๋ ์ปดํ์ผ ๊ฒฐ๊ณผ๋ก ๋ง๋ค์ด์ง ๋ฒ๋ค ํ์ผ๋ง ํฌํจํ๋ฉด ๋จ

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/fe7ed023-e492-4c9f-877a-be274f04c80c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074419Z&X-Amz-Expires=86400&X-Amz-Signature=cb3afadfd139eff1c7607ed27fae655b1af13bb36c7d2a5934ccd1954525d768&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- ์ํธ๋ฆฌ ํ์ผ์ด ์ฌ๋ฌ ๊ฐ์ผ ๋๋ ์ํธ๋ฆฌ ํ์ผ๋ง๋ค ๋ฒ๋ค ํ์ผ์ด ์์ฑ

[https://d2.naver.com/helloworld/0239818](https://d2.naver.com/helloworld/0239818)

์ฌ๋ด

- ์น์ ๊ฐ๋ฐํ๋ค๋ณด๋ฉด ๋ค์ํ ํ์ฅ์์ ํ์ผ์ ๋ง๋ค๊ฒ ๋๋ค. ์ด๋ ๊ฒ ๋ค์ํ ์์ค๋ ์น ์ดํ๋ฆฌ์ผ์ด์์ ๋ฌด๊ฒ๊ฒ ๋ง๋ ๋ค. ํต์ ์ด ์์ ๋๋ง๋ค ์ด ์์ค๋ค์ ๋ก๋ฉํ๋ ์์์ ๊ณ ๋น์ฉ์ด๋ค. ๋ง์ JS ํจํค์ง๋ฅผ ์ฌ์ฉํ๋ค๋ณด๋ฉด ์์ํ์ง ๋ชปํ ์ถฉ๋๋ก ์ธํด ์ดํ๋ฆฌ์ผ์ด์์ด ๊นจ์ง๊ฒ ๋  ์๋ ์๋ค(๊ฐ์ ์ด๋ฆ์ ๋ณ์๋ฅผ ์ฌ์ฉํ๋ ๋ฑ). ์ด๋ฅผ ํด๊ฒฐํ๊ธฐ ์ํด ๋ฑ์ฅํ ๋๊ตฌ๊ฐ Bundler์ด๋ค. bundle์ ๋ฌถ๋๋ค๋ ๋ป์ด๋ค. **์ฌ๋ฌ๊ฐ์ ํ์ผ์ ๋ฌถ์ด์ฃผ๋ ์ด๋ ํ ์ ๋ฆฌ ๋ฐฉ๋ฒ**์ด๋ค. ๊ตฌ์ฒด์ ์ธ ๊ธฐ์ ๋ก๋ WebPack, Broserify, Parcel์ด ์๋ค. WebPack์ ๊ฐ์ฅ ์ธ๊ธฐ์๋ ๋๊ตฌ์ด๋ค. ํ๋์ JSํ์ผ์ .js๋ฟ๋ง ์๋๋ผ .css๋ imageํ์ผ ๋ฑ์ ๋ชจ๋์ ๋ชจ๋ ๋ชฐ์๋ฃ์ ์ ์๋ค. ๋์์ ์ฑ๋ฅ์ ํฅ์์ํค๊ธฐ ์ํด ํ์ํ๋ค๋ฉด ๋ค์ ๋ถ๋ฆฌํ  ์ ์๋ค. ํนํ, WebPack์ ๋๋ฌ์ผ ๋ฐฉ๋ํ ์ํ๊ณ ๋๋ถ์ ๋ค์ํ ํ์ฅ ๊ธฐ๋ฅ ๋ฑ์ด ์๋ค. ๋ฐ๋ผ์ ๋ง์ ์์๋ค์ ์๋ํ ์ํฌ ์ ์๋ค.

### SPA

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/52d72e86-78b8-40ec-add1-edae7209ec18/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T082626Z&X-Amz-Expires=86400&X-Amz-Signature=702a5815794c1120fd504b2bb0da2b5a5311cf8daf3a77776b3dfc458d45d4e6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- SPA(Single Page Application)๋ ํ ๊ฐ(Single)์ Page๋ก ๊ตฌ์ฑ๋ Application
- ์น ์ํ๋ฆฌ์ผ์ด์์ ํ์ํ **๋ชจ๋  ์ ์  ๋ฆฌ์์ค๋ฅผ ์ต์ด ํ ๋ฒ์ ๋ค์ด๋ก๋**
- ๊ทธ ํ์๋ ๋ฐ์ดํฐ๋ฅผ ๋ฐ์์ฌ ๋๋ง ์๋ฒ์ ํต์ 
- ๊ทธ ์ดํ ์๋ก์ด ํ์ด์ง ์์ฒญ์ด ์์ ๋, ํ์ด์ง ๊ฐฑ์ ์ **ํ์ํ ๋ฐ์ดํฐ๋ง ์ ๋ฌ ๋ฐ์์ ํ์ด์ง๋ฅผ ๊ฐฑ์ **
- ํ์ํ ๋ถ๋ถ๋ง ๊ฐฑ์ ํ๊ธฐ ๋๋ฌธ์ ๋ค์ดํฐ๋ธ ์ฑ์ ๊ฐ๊น์ด ์์ฐ์ค๋ฌ์ด ํ์ด์ง ์ด๋๊ณผ ์ฌ์ฉ์ ๊ฒฝํ(UX)์ ์ ๊ณต

โ SPA๋ฅผ **CSR(Client Side Rendering)** ๋ฐฉ์์ผ๋ก ๋ ๋๋ง์ด๋ผ ํจ

### ์ฅ์ 

- ์์ฐ์ค๋ฌ์ด ์ฌ์ฉ์ ๊ฒฝํ (UX) โ ์ ์ฒด ํ์ด์ง๋ฅผ ์๋ฐ์ดํธ ํ  ํ์๊ฐ ์๊ธฐ ๋๋ฌธ์ ๋น ๋ฅด๊ณ  โ๊น๋นกโ ๊ฑฐ๋ฆผ์ด ์์
- ํ์ํ ๋ฆฌ์์ค๋ง ๋ถ๋ถ์ ์ผ๋ก ๋ก๋ฉ (์ฑ๋ฅ) โ SPA์ Application์ ์๋ฒ์๊ฒ ์ ์ ๋ฆฌ์์ค๋ฅผ ํ ๋ฒ๋ง ์์ฒญ ๊ทธ๋ฆฌ๊ณ  ๋ฐ์ ๋ฐ์ดํฐ๋ ์ ๋ถ ์ ์ฅ**(์บ์=Cache)**
- ์๋ฒ์ ํํ๋ฆฟ ์ฐ์ฐ์ ํด๋ผ์ด์ธํธ๋ก ๋ถ์ฐ (์ฑ๋ฅ)
- ์ปดํฌ๋ํธ๋ณ ๊ฐ๋ฐ ์ฉ์ด (์์ฐ์ฑ)
- ๋ชจ๋ฐ์ผ ์ฑ ๊ฐ๋ฐ์ ์ผ๋์ ๋๋ค๋ฉด ๋์ผํ API๋ฅผ ์ฌ์ฉํ๋๋ก ์ค๊ณ ๊ฐ๋ฅ (์์ฐ์ฑ)

### ๋จ์ 

- JavaScript ํ์ผ์ ๋ฒ๋ค๋งํด์ ํ ๋ฒ์ ๋ฐ๊ธฐ ๋๋ฌธ์ ์ด๊ธฐ ๊ตฌ๋ ์๋๊ฐ ๋๋ฆผ (Webpack์ code splitting์ผ๋ก ํด๊ฒฐ ๊ฐ๋ฅ)
- ๊ฒ์์์ง์ต์ ํ(SEO)๊ฐ ์ด๋ ค์ (SSR๋ก ํด๊ฒฐ ๊ฐ๋ฅ) โ SPA ์ฑ์ ๊ฒ์๋ก๋ด ์์ฅ์์ ๋ณด๋ฉด ๋ชจ๋  ํ์ด์ง์ ์์ค๊ฐ ์๋์ ๊ฐ์ด ๋ณด์, ๊ฒ์์์ง์ด ์์ธ์ ํ  ๋งํ ์ปจํ์ธ ๊ฐ ์กด์ฌํ์ง ์๋ ๊ฒ
    
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
    

### **SPA ๋ฐฉ์์ด ๋ชจ๋ CSR์ธ ๊ฒ์ ์๋**

### MPA

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/70ca152a-8f1f-4dff-b9f8-e5ed0dab1b2e/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T082643Z&X-Amz-Expires=86400&X-Amz-Signature=ac9d74de29283ee4893004ed3134cb922bdd2ff55d12b13d0b7c036c099dc0df&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- MPA(Multiple Page Application)๋ ์ฌ๋ฌ ๊ฐ(Multiple)์ Page๋ก ๊ตฌ์ฑ๋ Application
- **์๋ก์ด ํ์ด์ง๋ฅผ ์์ฒญ**ํ  ๋๋ง๋ค **์ ์  ๋ฆฌ์์ค(HTML, CSS, JavaScript)**๊ฐ ๋ค์ด๋ก๋
- **๋งค๋ฒ ์ ์ฒด ํ์ด์ง๊ฐ ๋ค์ ๋ ๋๋ง**

โ MPA๋ฅผ **SSR(Server Side Rendering)** ๋ฐฉ์์ผ๋ก ๋ ๋๋ง์ด๋ผ ํจ

### ์ฅ์ 

- SEO ๊ด์ ์์ ์ ๋ฆฌ โ MPA๋ ์์ฑ๋ ํํ์ HTML ํ์ผ์ ์๋ฒ๋ก๋ถํฐ ์ ๋ฌ๋ฐ์ ๋ฐ๋ผ์ ๊ฒ์์์ง์ด ํ์ด์ง๋ฅผ ํฌ๋กค๋งํ๊ธฐ์ ์ ํฉ
- ์ฒซ ๋ก๋ฉ์ด ๋งค์ฐ ์งง์ โ ์๋ฒ์์ ์ด๋ฏธ ๋ ๋๋งํด ๊ฐ์ ธ์ค๊ธฐ ๋๋ฌธ, ๊ทธ๋ฌ๋ ํด๋ผ์ด์ธํธ๊ฐ JS ํ์ผ์ ๋ชจ๋ ๋ค์ด๋ก๋ํ๊ณ  ์ ์ฉํ๊ธฐ์  ๊น์ง๋ ๊ฐ๊ฐ์ ๊ธฐ๋ฅ์ ๋์ํ์ง ์์

### ๋จ์ 

- ์๋ก์ด ํ์ด์ง๋ฅผ ์ด๋ํ๋ฉด โ๊น๋นกโ์ธ๋ค (UX) โ ๋งค ํ์ด์ง ์์ฒญ๋ง๋ค ๋ฆฌ๋ก๋ฉ(์๋ก๊ณ ์นจ) ๋ฐ์, ์๋ก์ด ํ์ด์ง๋ฅผ ์์ฒญํ  ๋๋ง๋ค ์ ์ฒด ํ์ด์ง๋ฅผ ๋ค์ ๋ ๋๋งํ๊ธฐ ๋๋ฌธ
- ํ์์ง ์ด๋์ ๋ถํ์ํ ํํ๋ฆฟ๋ ์ค๋ณตํด์ ๋ก๋ฉ (์ฑ๋ฅ)
- ์๋ฒ ๋ ๋๋ง์ ๋ฐ๋ฅธ ๋ถํ
- ๋ชจ๋ฐ์ผ ์ฑ ๊ฐ๋ฐ์ ์ถ๊ฐ์ ์ธ ๋ฐฑ์๋ ์์ ํ์ (์์ฐ์ฑ) ๊ฐ๋ฐ์ด ๋ณต์กํด์ง ์ ์์

### SSR, CSR ์ฐจ์ด โ ์ด๊ธฐ๋ ๋๋ง์๋, SEO, ๋ณด์

### SSR์ด ๋ ๋๋ง ํ๋ ๋ฐฉ์

- ๋ชจ๋  ํํ๋ฆฟ์ ์๋ฒ ์ฐ์ฐ์ ํตํด์ ๋ ๋๋งํ๊ณ  ์์ฑ๋ ํ์ด์ง ํํ๋ก ์๋ต โ ์ด ๊ณผ์ ์ **์๋ฒ ์ฌ์ด๋ ๋ ๋๋ง(SSR)**์ด๋ผ๊ณ  ๋ถ๋ฆ

### CSR์ด ๋ ๋๋งํ๋ ๋ฐฉ์

- ์ต์ด์ ํ๋ฒ ์๋ฒ์์ ์ ์ฒด ํ์ด์ง๋ฅผ ๋ก๋ฉํ์ฌ ๋ณด์ฌ์ฃผ๊ณ  ์ดํ์๋ ์ฌ์ฉ์์ ์์ฒญ์ด ์ฌ ๋๋ง๋ค, ๋ฆฌ์์ค๋ฅผ ์๋ฒ์์ ์ ๊ณตํ ํ ํด๋ผ์ด์ธํธ๊ฐ ํด์ํ๊ณ  ๋ ๋๋งํ๋ ๋ฐฉ์

## package.json

- ํ๋ก์ ํธ์ ์ ๋ณด๋ฅผ ์ ์ํ๊ณ , ์์กดํ๋ย **ํจํค์ง ๋ฒ์  ์ ๋ณด**๋ฅผ ๋ช์ํ๋ ํ์ผ
- ๋ฐฐํฌํ ๋ชจ๋ ์ ๋ณด๋ฅผ ๋ด๊ณ ์ ๋ง๋ค์ด์ง
- ๋ธ๋๋ก ์์ฑํ๋ ์ ํ๋ฆฌ์ผ์ด์๋ package.json ํ์ผ์ ์ฌ์ฉํ์ฌ ๊ด๋ฆฌํ  ์ ์์
- ์ฌ์ฉํ๋ ํ์ฅ ๋ชจ๋์ ๋ํ ์์กด์ฑ ๊ด๋ฆฌ๊ฐ ๊ฐ๋ฅํ๊ธฐ ๋๋ฌธ์ ํธ๋ฆฌํด์ง

### ์์ญ

- ํ๋ก์ ํธ์ ์ ๋ณด - name, version ์์ญ
- ํจํค์ง ๋ฒ์  ์ ๋ณด -ย **dependencies ๋๋ devDependencies**ย ์์ญ

### ํจํค์ง ์ง์ 

- "dependencies":ย **ํ๋ก๋์ ํ๊ฒฝ**์์ ์์ฉ ํ๋ก๊ทธ๋จ์ ํ์ํ ํจํค์ง
- "devDependencies":ย **๋ก์ปฌ ๊ฐ๋ฐ ๋ฐ ํ์คํธ**์๋ง ํ์ํ ํจํค์ง

### ์๋ฉํฑ ๋ฒ์ ๋ ๊ท์น

**ํธ๋(~)**

```json
"devDependencies": {
  "@vue/cli-service": "~4.3.0",
},
```

- ํด๋น ํจํค์ง์ ํจ์น ๋ ๋ฒจ ๋ณ๊ฒฝ์ ํ์ฉํ๊ฒ ๋ค๋ ์๋ฏธ
- ์ฆ, 4.4.0 ๋ฏธ๋ง์ ํจ์น ๋ ๋ฒจ ๋ณ๊ฒฝ์ ํ์ฉํ๊ฒ ๋ค๋ ์๋ฏธ

**์บ๋ฟ(^)**

```json
"dependencies": {
  "vue": "^2.6.11"
}
```

- ํด๋น ํจ์บ์ง์ ๋ง์ด๋, ํจ์น ๋ณ๊ฒฝ์ ํ์ฉํ๊ฒ ๋ค๋ ์๋ฏธ
- ์ฆ, 3.0.0 ๋ฏธ๋ง์ ๋ง์ด๋, ํจ์น ๋ณ๊ฒฝ์ ํ์ฉํ๊ฒ ๋ค๋ ์๋ฏธ

## ์ปดํฌ๋ํธ

### ๊ธฐ๋ณธ๊ตฌ์กฐ

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/5c9fd55b-16b0-444b-a9e7-8bc7c264c537/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074448Z&X-Amz-Expires=86400&X-Amz-Signature=e07ea3936693d45fb53558d0aa23847354b9b947cb53cdc18b0d7a42b3463e7d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- ํด๋์คํ ์ปดํฌ๋ํธ โ render ํจ์๋ฅผ ์ฌ์ฉํด์ retrun์์ ์ฝ๋๋ฅผ ํ๋ฉด์ ๋ณด์ด๋๋ก ํจ
- ํจ์ํ ์ปดํฌ๋ํธ โ ์์ ์ด ๋ ๋ ํจ์์ด๊ธฐ ๋๋ฌธ์ render ํจ์ ์ฌ์ฉ์์ด return ๊ฐ๋ง ์ฌ์ฉ

### props ๊ฐ ์ ๋ฌ ๋ฐ๊ธฐ

- App.js ์ค์  โ App.js ์ปดํฌ๋ํธ๋ ํจ์ํ ์ปดํฌ๋ํธ๋ก ๊ตฌํ

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/130d7713-cc3c-4a8f-b94a-3281b37174bc/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074504Z&X-Amz-Expires=86400&X-Amz-Signature=2f0a59f0aaf79c011f64b912a23e3eed729d4c11c0f615eee3e8b51b367242e6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- ํด๋์คํ ์ปดํฌ๋ํธ โ ํด๋์คํ ์ปดํฌ๋ํธ์์ ๋ถ๋ชจ ์ปดํฌ๋ํธ์์ ์ ์ํ props ๊ฐ์ {this.props.props์ด๋ฆ}์ผ๋ก ๋ฐ์์ ์

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/dc9893f0-e9cb-4b3b-89cb-776aba00cd95/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074522Z&X-Amz-Expires=86400&X-Amz-Signature=afe67925db480ecadf89824647a762a6a60abd28a9d44326e33a44e0934ab62d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

- ํจ์ํ ์ปดํฌ๋ํธ โ ํจ์ํ ์ปดํฌ๋ํธ์์ ์ ์ํ props ๊ฐ์ ํจ์์ ์ธ์๊ฐ(ํ๋ผ๋ฏธํฐ)์ผ๋ก ๋ฐ์์ด ์ฆ, ๋ถ๋ชจ ์ปดํฌ๋ํธ์์ ์ ๋ฌ๋ฐ์ props ๊ฐ์ ํจ์ํ ์ปดํฌ๋ํธ์ ์ธ์๋ก ์ค์ ํ์ฌ ํจ์ ๋ด๋ถ์ props ๊ฐ์ ์ ๋ฌํด์ ํ๋ฉด์ ๋ํ๋๊ฒ ํ๋ ๊ฒ

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/8deaea4e-b8ce-4cbf-a476-b653fb2b00a6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T074534Z&X-Amz-Expires=86400&X-Amz-Signature=f129b2ec851be614174293ecb8ec5eaeac70e945d860214b1799d825e5ada749&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)
