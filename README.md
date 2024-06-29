
# KidCorp Admin & Backend

KidCorp is a project intended to be used as a kid-friendly tool to generate stores, teach e-commerce, and be managed hands-off. This part of the project is the Admin site, API used to communicate with both the standalone database as well as the Shopify headless CMS.


## Tech Stack

**Primary:** TypeScript, Next.js, Mantine UI, Prisma ORM, Mongo DB

**Secondary:** Shopify Admin/Storefront APIs, bcrypt, jwt
## Developer Thoughts

This part of the project contains a WIP Admin page and and works as the API for the standlone database and Shopify CMS.

**Important**: This entire repo can be scrapped and done in any way you please. Feel free to use it as a reference or just to connect the other repo to Shopify for the time being.

This project is using Shopify to get products from various drop shipping services as base collections, then copy the desired collection as a standalone to handle the products for each generated store. It is also using it's own database with *User* and *Store* tables with their IDs being added as tags on Shopify to related orders, collections, etc. within Shopify to manage handling data related to each specific store, all managed under the single Shopify account, effectively using it as a multi-vendor marketplace.

Again, you can do this however you want. I doubt a ton of developers would go this route unless they have specifically spent a ton of time with Shopify and know the ins and outs of the data queries and mutations available via their GraphQL endpoints. 
## Author

- C.J. Fritz | [GitHub](https://www.github.com/cjfritz9) | [Email](mailto:contact@cjfritz.dev)

# Mantine Next.js template

This is a template for [Next.js](https://nextjs.org/) app router + [Mantine](https://mantine.dev/).
If you want to use pages router instead, see [next-pages-template](https://github.com/mantinedev/next-pages-template).

## Features

This template comes with the following features:

- [PostCSS](https://postcss.org/) with [mantine-postcss-preset](https://mantine.dev/styles/postcss-preset)
- [TypeScript](https://www.typescriptlang.org/)
- [Storybook](https://storybook.js.org/)
- [Jest](https://jestjs.io/) setup with [React Testing Library](https://testing-library.com/docs/react-testing-library/intro)
- ESLint setup with [eslint-config-mantine](https://github.com/mantinedev/eslint-config-mantine)

## npm scripts

### Build and dev scripts

- `dev` – start dev server
- `build` – bundle application for production
- `analyze` – analyzes application bundle with [@next/bundle-analyzer](https://www.npmjs.com/package/@next/bundle-analyzer)

### Testing scripts

- `typecheck` – checks TypeScript types
- `lint` – runs ESLint
- `prettier:check` – checks files with Prettier
- `jest` – runs jest tests
- `jest:watch` – starts jest watch
- `test` – runs `jest`, `prettier:check`, `lint` and `typecheck` scripts

### Other scripts

- `storybook` – starts storybook dev server
- `storybook:build` – build production storybook bundle to `storybook-static`
- `prettier:write` – formats all files with Prettier
