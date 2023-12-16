
# setting Next.js 

- build project
```bash
npm run dev
```

- Open [http://localhost:3000](http://localhost:3000)


# setting prisma

```
npx prisma init
```

- Create .env contains
```
DATABASE_URL="mysql://username:password@localhost:3306/employee?schema=public"
```

Generate schema in schema.prisma
```
npx prisma db pull
```

Update database type in schema.prisma
```
datasource db {
  provider = "mysql"
  url      = env("DATABASE_URL")
}
```

Generate script in prisma script in node_modules
```
npx prisma generate
```

build and run next.js
```
npm run build
npm run start
```