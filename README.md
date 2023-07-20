## Demo

![demo.gif](https://github.com/5hanazar/sveltekit-prisma/blob/main/demo.gif)

## Setup

Clone the repo and install dependencies with `npm install` (or `pnpm install` or `yarn`).<br/>
Create `.env` file and set the following variables:

```bash
#MySQL connection URL
DATABASE_URL="mysql://username:password@localhost:3306/database"

#JWT secret key
PRIVATE_KEY="key"
```

Generate a Prisma migration:

```bash
npx prisma migrate dev --name init
npx prisma generate
```

Seed the database:

```bash
npx prisma db seed
```

## Developing

Start a development server:

```bash
npm run dev
```

## Building

To create a production version of your app:

```bash
npm run build
```