# ๊ฐ์์ด๊ธฐ

## ๐ป 1. ํ๋ก์ ํธ ์๊ฐ
<img src='./intro/main.png'>

- ๊ฐ์์ด๊ธฐ๋ ๊ฟ์ ์ด๋ฃฌ ๊ฐ์๋ฌ๊ฐ ๊ฟ์ ์ด๋ฃจ๊ธฐ ์ํด ๋ธ๋ ฅํ๋ ๊ณผ์ ๊ณผ ํฌ๋๋ฆฌ์คํธ๋ฅผ ํผ๋๋ฅผ ํตํด **๊ณต์ **ํ๊ณ , <br>
๊ฟ์ ์ด๋ฃจ๋ ค๋ ์ฌ๋๋ค์ **๊ทธ ๋ฆฌ์คํธ๋ฅผ ๊ฐ์ ธ์** ์ค์ฒํ  ์ ์๊ฒ ๋์์ฃผ๋ ์ฑ์๋๋ค. <br>

### ๐ ํ๋ก์ ํธ ์ธ์
- ๊ธฐํ2๋ช, ๋์์ธ2๋ช, ios๊ฐ๋ฐ2๋ช, ๋ฐฑ์๋๊ฐ๋ฐ2๋ช ์ด 8๋ช์ ์ธ์์ด ์์ดํ ๋์ถ ๋ฐ ๊ธฐํ๋ถํฐ ๊ฐ๋ฐ๊น์ง ์ฌ์ด๋ํ๋ก์ ํธ ์งํ

### ๐ ํ๋ก์ ํธ ๊ธฐ๊ฐ
- 2022.08 ~ 2022.12 (12์ ์ค์ ์ถ์ ์์ )

### โญ๏ธ ํ๋ก์ ํธ Github
- [GitHub Repository](https://github.com/live-god-life)

### ๐ ์ฃผ์ ๊ธฐ๋ฅ
<details>
<summary><b>๋ฉ์ธ ํผ๋</b></summary>
<div markdown="1">
<img src='./intro/feed.png'>
</div>
</details>
<br/>

<details>
<summary><b>Todo</b></summary>
<div markdown="1">
<img src='./intro/todo.png'>
</div>
</details>
<br/>

<details>
<summary><b>Detail</b></summary>
<div markdown="1">
<img src='./intro/detail.png'>
</div>
</details>
<br/>

<details>
<summary><b>Todo ์ถ๊ฐ</b></summary>
<div markdown="1">
<img src='./intro/add.png'>
</div>
</details>
<br/>

## ๐ฃ 2. ํ์ ํ๊ฒฝ
- Git
  - [์ปค๋ฐ ์ปจ๋ฒค์](./git/%EA%B9%83%EC%BB%A8%EB%B2%A4%EC%85%98.md)
  - [๋ธ๋์น ์ ๋ต](./git/%EB%B8%8C%EB%9E%9C%EC%B9%98%EC%A0%84%EB%9E%B5.md)
  - [์ฝ๋ ๋ฆฌ๋ทฐ](./git/%EC%BD%94%EB%93%9C%EB%A6%AC%EB%B7%B0%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4.md)
- ์ปค๋ฎค๋์ผ์ด์
  - Slack, Notion, Figma ํ์ฉ

## โญ๏ธ 3. ๋ฐฑ์๋ ๊ธฐ์  ์คํ
- Java, Gradle, SpringBoot
- JPA, QueryDSL
- MySQL
- Spring Cloud
- Naver Cloud Platform
- Docker
- Jenkins

## ๐ข 4. ์ธํ๋ผ & CI/CD
<img src='./infra/infra.png'>

- MSA ์๋น์ค
  - `discovery-service`
    - spring cloud eureka server๋ฅผ ํ์ฉํ์ฌ ๊ตฌํ
    - ๊ฐ๊ฐ์ ๋น์ฆ๋์ค ์๋น์ค๋ discovery client๋ก server์ ๋ฑ๋ก๋์ด ์ฌ์ฉ๋์ด์ง
  - `config-service`
    - spring cloud config server๋ฅผ ํ์ฉํ์ฌ ๊ตฌํ
  - `apigateway-service`
    - spring cloud gateway๋ฅผ ํ์ฉํ์ฌ ๊ตฌํ
    - JWT ์๋น์คํ ํฐ์ ์ ํจ์ฑ ๊ฒ์ฌ ๋ฐ ์ธ์ฆ, ์ธ๊ฐ ์ญํ  ๋ด๋น
    - Filter๋ฅผ ํ์ฉํ์ฌ ๊ฐ ์๋น์ค๋ฅผ ํธ์ถ

  - `auth-service`
    - JWT ์๋น์คํ ํฐ์ ๋ฐํ, ๊ฐฑ์ , refresh token ๊ด๋ฆฌ ๋ฑ์ ํ ํฐ ์๋ช์ฃผ๊ธฐ ๋ด๋น
  - `user-service`
    - ์ฌ์ฉ์์ ๊ด๋ จ๋ ๊ธฐ๋ฅ์ ๋ด๋น
  - `feed-service`
    - ๊ฐ์์ด๊ธฐ ํผ๋์ ๊ด๋ จ๋ ๊ธฐ๋ฅ์ ๋ด๋น
  - `goal-service`
    - ๊ฐ์์ด๊ธฐ ํฌ๋๋ฆฌ์คํธ์ ๊ด๋ จ๋ ๊ธฐ๋ฅ์ ๋ด๋น
  - `common-service`
    - ์ด์ฉ์ฝ๊ด, ๊ณตํต ์ฝ๋ ๋ฑ์ ๊ณตํต ๊ธฐ๋ฅ์ ๋ด๋น

- ๋ฐฑ์๋ CI/CD
  - ๊ฐ๋ฐ์ -> ๊นํ๋ธ ํธ์ -> ๊นํ๋ธ ์นํ -> ์  ํจ์ค API ํธ์ถ -> ์  ํจ์ค์ ๋ฑ๋ก๋ Pipeline ์คํ -> ๋์ปค ์ปจํ์ด๋๋ก ๋ฐฐํฌ

- DB
  - MySQL

## ๐งโ๐ป 5. ๋ด๋น ์๋ฌด
### ๊ฐ๋ฐ๋ฆฌ๋ ์ญํ 
- ๊ธฐํ์, ๊ฐ๋ฐ์๊ฐ ์ปค๋ฎค๋์ผ์ด์
- ํ๋ก ํธ, ๋ฐฑ์๋ ๊ฐ๋ฐ์๊ฐ ์ปค๋ฎค๋์ผ์ด์
- ์ฌ์ฉํ  ๊ธฐ์  ์คํ ์ ๋ฆฌ
- ๊ฐ๋ฐ ์ผ์ , ๊ฐ๋ณ ์๋ฌด ๊ด๋ฆฌ
### ๋ฐฑ์๋ ๊ฐ๋ฐ์ ์ญํ 
- Naver Cloud Platform ์๋ฒ ํ๊ฒฝ ๊ตฌ์ถ
  - [Docker ์ค์น ์ ๋ฆฌ](./infra/CentOS7_Docker%20%EC%84%A4%EC%B9%98.md)
  - [MySQL ์ค์น ์ ๋ฆฌ](./infra/CentOS7_MySQL%208%EB%B2%84%EC%A0%84%20%EC%84%A4%EC%B9%98.md)
  - [MySQL ์ธํ ์ ๋ฆฌ](./infra/CentOS7_MySQL%20%EC%84%B8%ED%8C%85.md)
- MSA ํ๊ฒฝ ๊ตฌ์ถ
  - ์ด๊ธฐ discovery, apigateway, config service ๊ธฐ๋ณธ ์ธํ
  - MSA ํ๊ฒฝ ๊ตฌ์ถ์ ์ํด ์ฌ๋ฌ ์๋ฒ๋ฅผ ํ์ฉํ๋ ๊ฒ ๋์  Docker Container๋ฅผ ํ์ฉํ์ฌ ์ต๋ํ MSA ํ๊ฒฝ์ ๊ตฌ์ฑํ์ต๋๋ค
- CI/CD ํ๊ฒฝ ๊ตฌ์ถ
  - [CI/CD ๊ตฌ์ถ ์ ๋ฆฌ](./infra/CI%2CCD%EA%B5%AC%EC%B6%95.md)
- ํฌ๋ ๋ฐ์ดํฐ ๋ชจ๋ธ๋ง ๋ฐ RestfulAPI ์ค๊ณ ๋ฐ ๊ฐ๋ฐ (goal-service)
- ํผ๋ ๋ฐ์ดํฐ ๋ชจ๋ธ๋ง ๋ฐ RestfulAPI ์ค๊ณ ๋ฐ ๊ฐ๋ฐ (feed-service)