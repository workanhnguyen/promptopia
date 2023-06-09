This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

PERSONAL NOTES:
1. Khởi tạo project: npx create-next-app@latest ./
2. Enter đến bước cuối cùng.
3. Cài đặt một số package sau:
    + npm install bcrypt
    + npm install mongodb
    + npm install mongoose
    + npm install next-auth
4. Xóa folder app và tạo lại.
5. Tạo folder components, models, styles, utils là con trực tiếp của project.
6. Xóa folder public và tạo lại.
7. Tạo file .env.
8. Vào file jsconfig.json, thay đổi "@/*" thành "@*".
9. Vào link này và copy code, sau đó dán vào file next.config.js: https://github.com/adrianhajdin/project_next_13_ai_prompt_sharing/blob/main/next.config.js
10. Thêm http:localhost:3000/api/auth/callback/google vào API Cloud google app ở mục API redirect.
11. Thêm .env vào gitignore

DEPLOYMENT:
1. Dùng Netlify hoặc Vercel up project lên thông qua github.
2. Thêm các biến môi trường (Environment variables) là NEXTAUTH_URL, NEXTAUTH_URL_INTERNAL, NEXTAUTH_SECRET có giá trị như trong file .env ở local.
3. Chỉnh network access ở mongoDB thành 0.0.0.0/0.
4. Vào API Cloud Google, thêm các URI của hosting web deploy vào.