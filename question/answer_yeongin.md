## ๐ ๊ธฐ์  ์ธ ๊ณตํต ๋ฉด์  ์ง๋ฌธ

### [ ์๊ธฐ์๊ฐ ๋ฐ ์ง์๋๊ธฐ ]

### [ ์ฃผ์ ๊ธฐ์ ์คํ ๋ฐ ์ญํ  ] โ
 - Node.js
 - React
 - Mongo DB
 
### [ ์๊ธฐ์๊ฐ์ ๊ธฐ๋ฐ์ ํ๋ก์ ํธ ์ง๋ฌธ ]
- ์ด๋ค ์ญํ ์ ๋ด๋นํ์๋๊ฐ? โ
``` 
API๋ฅผ ์ด์ฉํด์ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ ธ์ค๊ณ , react chart๋ฅผ ์ด์ฉํ์ฌ ์๊ฐํ
```
- ์๋ฒ๋ ์ด๋ป๊ฒ ๊ตฌ์ฑํ์๋๊ฐ?โ
``` 
nginx๋ฅผ reverse-proxy๋ก ๋๊ณ , pm2๋ก nodejs ๋ฌด์ค๋จ ์๋น์ค๊ฐ ๊ฐ๋ฅํ๋๋ก ๊ตฌ์ฑ
aws๋ก instance์์ฑํ์ฌ ๋ฐฐํฌ ์งํ

why reverse proxy? 
- ๋ก๋ ๋ฐธ๋ฐ์ฑ์ ์ฌ์ฉํ์ฌ ๋ ๋น ๋ฅธ ์๋ฒ๋ฅผ ๋ง๋ค ์ ์์ต๋๋ค.
- ์ฌ์ด log ์์ฑ๊ณผ ๊ด๋ฆฌ : nginx ์ค์ ์์ access_log ๊ฐ์ ์ธ์๋ฅผ ํ๋ ์ถ๊ฐํ๋ ๊ฒ๋ง์ผ๋ก๋ ์ฝ๊ฒ ๋ก๊ทธ๋ฅผ ์์ฑํ  ์ ์์ต๋๋ค.
- ๋ณด์ : ํด๋ผ์ด์ธํธ์์ ์๋ฒ์ ์ ์ ํ ๋, 3000์ ๊ฐ์ ํฌํธ๊ฐ ์๋๋ผ, nginx์ 80๋ฒ ํฌํธ๋ก ์ ์ํ  ์ ์์ด ์ง์ ์ ์ธ ์ ๊ทผ์ด ๋ถ๊ฐ๋ฅํฉ๋๋ค.
- ์บ์ฌ ์ฌ์ฉ : css๋ js์ ์ ์ ์ธ ํ์ผ์ ํธ์คํ ํ  ๋, ์บ์ฌ๋ฅผ ์ฌ์ฉํด ๋ ๋์ ์ฑ๋ฅ์ ๋ณด์ฌ์ค ์๋ ์์ต๋๋ค.

```
- ์ด๋ค ์ธ์ด์ ํ๋ ์์ํฌ, ๋ผ์ด๋ธ๋ฌ๋ฆฌ?โ
```
- ์๋ฐ์คํฌ๋ฆฝํธ
- React
- Node.js
```
- ๋ช๋ช์ ์ฌ์ฉ์, ์ด๋ ์ ๋์ ํธ๋ํฝ
- ํด๋น ๊ธฐ์  ์คํ์ ์ฌ์ฉํ ์ด์ โ
```
- mongoDB: ์์ ๋ก์ด ๋ฐ์ดํฐ ๊ตฌ์กฐ, RDB์ ๋นํด ์ฑ๋ฅ์ด ์ข์ ๋น ๋ฅธ ๋ฐ์ดํฐ ์กฐํ ๊ฐ๋ฅ
- node.js: ์๋ฐ์คํฌ๋ฆฝํธ ๋ฐํ์ ํ๊ฒฝ, jsx๋ฌธ๋ฒ ์ฌ์ฉ๊ฐ๋ฅ
- React: Component ๋จ์ ์์ฑ์ผ๋ก ์์ฐ์ฑ, ์ ์ง๋ณด์ ํธ๋ฆฌ, virtual dom์ ์ด์ฉํ ๋น ๋ฅธ ๋ ๋๋ง
```
- ๊ตฌ์กฐ์ ๋ํ ์ค๋ช ๋ฐ ์ค๊ณ ๊ด๋ จ ๋ด์ฉ
- ์ด๋ ํ ์๊ณ ๋ฆฌ์ฆ, ์๋ฃ๊ตฌ์กฐ ํน์ ๋์์ธํจํด์ ์ฌ์ฉํ์๋๊ฐ?
- ๊ฐ์ ์ ์ ๋ฌด์์ด์๋?
- ์ด๋ป๊ฒ ํ๋ก์ ํธ๋ฅผ ๊ด๋ฆฌํ๊ณ (์ค์ผ์ค, ์ํต ๋ฑ) ์ด๋ป๊ฒ ๊ธฐ์ฌํ๋๊ฐ?(๋ฌธ์ํ, ๊ตฌ์กฐ ์ค๊ณ, ๊ฐ๋ฐ ๋ฑ)
- ์์ ์ ํ๋ก์ ํธ์์ ๋ค์ํ ์ํฉ์ ๊ฐ์ ํด๋ณด์. (์ด๋ฐ ๊ฒฝ์ฐ ํน์ ์ ๋ฐ ๊ฒฝ์ฐ์ ์ด๋ป๊ฒ ํ์ค ๊ฑด๊ฐ์? ๊ฐ์ ์ง๋ฌธ์ ์์ฃผ ํจ)
