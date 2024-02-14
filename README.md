# Full Stack E-Commerce Dashboard Next.js 13 App Router, React, Tailwind, Prisma, PostgreSQL

Key Features:

- Shadcn UI for the Admin!
- Serves as both CMS, Admin and API!
- Control mulitple vendors / stores through this single CMS!
- Create, update and delete categories!
- Create, update and delete products!
- Upload multiple images for products, and change them!
- Create, update and delete filters such as "Color" and "Size", and then match them in the "Product" creation form.
- Create, update and delete "Billboards".
- Search through all categories, products, sizes, colors, billboards with included pagination!
- Control which products are "featured" so they show on the homepage!
- Orders, sales, graphs of your revenue etc in Dashboard.
- Clerk Authentication!
- Order creation
- Stripe checkout
- Stripe webhooks
- PostgreSQL + Prisma + PlanetScale

### Prerequisites

**Node version 14.x**

### Cloning the repository

```shell
git clone https://github.com/Badhon303/ecom-admin.git
```

### Install packages

```shell
npm i
```

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

DATABASE_URL=""
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=
STRIPE_WEBHOOK_SECRET=
# .\stripe listen --forward-to localhost:3000/api/webhook for local
```

### Connect to PlanetScale and Push Prisma
```shell
npx prisma generate
npx prisma db push
```


### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |
