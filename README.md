# mono-folio

This is the very begining of a new project called mono-folio, it is a Next.js based web client to unleash web development experiments for newbies and experimented developers.

It will be a project to empower other developers to have not only an starting point for their own portfolio but also as a reference for newbies to learn and practice with a simple approach to web technologies using a monorepo solution ready to deploy right to the cloud

Note: the initial version is still in progress, it has some testing mocks and texts.

# ToDo:

Update documentation with a clear step by step tutorial for deploying in vercel and render cloud services

## Getting started

### Setting up Node

Next.js v14 requires Node.js 18.17.0 or later. It's recommended to use a node version manager such as [nvm](https://github.com/nvm-sh/nvm) or an alternative.

If you're using nvm, you can run the following command to install the correct version of node:

```bash
nvm use
```

### Installing dependencies

Once your node version is setup correctly, the next step is to install the dependencies by running:

```bash
yarn
```

### Environment variables

If this is your first time running the app, you'll want to create a `.env.local` file in the root of the project by copying the `.env.development` file. Make sure to update the values in the `.env.local` file to match your local environment.

### Apps and Packages

## Apps

- `backend`: a [Node](https://strapi.io/) app running Strapi
- `docs`: a [Next.js](https://nextjs.org/) app
- `web`: a [Next.js](https://nextjs.org/) app
- `storybook`: a [Storybook](https://storybook.js.org/) implementation

## Packages

- `ui`: a stub React component library shared by all the applications
- `eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`) for code linting
- `typescript-config`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### CONTRIBUTING

Check [CONTRIBUTING.md](CONTRIBUTING.md) guidelines to get a context before contributing to this repository.

## Commands

### Running the app

To run the app locally, use the following command:

```bash
yarn dev
```

### Unit tests

To run unit tests, use the following command:

```bash
yarn test
```

### Formatting

To check the code is formatted correctly, use the following command:

```bash
yarn lint
```

To format the code, use the following command:

```bash
yarn format
```

### Storybook

To run the component library Storybook, use the following command:

```bash
yarn workspace @mono-folio/storybook storybook
```

### Build

To build all apps and packages, run the following command:

```bash
yarn build
```

### Other commands

See the [package.json](./package.json) in the root of the repo for a full list of commands you can run.

## Useful Links

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting

Learn more about the power of Turborepo:

- [Tasks](https://turbo.build/repo/docs/core-concepts/monorepos/running-tasks)
- [Caching](https://turbo.build/repo/docs/core-concepts/caching)
- [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching)
- [Filtering](https://turbo.build/repo/docs/core-concepts/monorepos/filtering)
- [Configuration Options](https://turbo.build/repo/docs/reference/configuration)
- [CLI Usage](https://turbo.build/repo/docs/reference/command-line-reference)
