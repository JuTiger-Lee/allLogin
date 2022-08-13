# All Login

## 시작

1. npm ci

### Product Mode Start

- npm run start

### Dev Mode Start

- npm run dev

## 설명

- Passport를 이용해서 로컬 로그인, 소셜 로그인 기능을 구현해놓았습니다.

### 적용 소셜 로그인

- Kakao
- Facebook(로그아웃 기능 안됨::SDK로만 되는걸로 추측)
- Google
- Naver(로그아웃 기능 안됨::네이버에서 로그아웃 API를 제공하지 않는거 같음)

## Prisma 사용법

### 시작

- npx prisma init

### npx prisma introspect

- migrate는 export 이다, 하지만 import를 하려면 introspect 명령어를 통해서 이미 생성된 스키마를 불러올수있다.

### npx prisma generate

- Prisma 스키마를 읽고 내붕에 생성된 Prisma Client 라이브러리를 업데이트 한다.
- 즉 우리가 scheam를 업데이트하고 이 스키마를 통해 CRUD를 하려면 generate 명령어를 실행해야한다.
- 이 명령어를 실행할시 node_moudles/.prisma/client 에 생성이되고 우리는 이 파일을 통해 CRUD를 하는거다.

### 주의

_Prisma schema 가 변경될 때 마다 npx prisma generate 로 업데이트를 해야한다._
