# Lerna Monorepo, Typescript, Yarn & React Storybook Base

Project with minimum configuration needed to start a Monorepo, e.g a component's library with an example of Storybook to
show examples of them.

We have also added ESLint & Prettier dependencies and configurations, you could use this as a base and complete it.

## Project setup

### Clone or copy the repo

Download the repo, cloning or copying it into your project or in a new one.

### Environment

For running the project, you need to have installed node and yarn.

### Install dependencies

To install dependencies we will use lerna tasks.

To install all dependencies and linking any cross-dependencies:

```shell
yarn install
```

To execute Storybook scripts we will use lerna as:

```shell
lerna run lint
lerna run build
lerna run storybook
```

The last one will start a Storybook in our navigator.

To see more information about Lerna, visit: <https://lerna.js.org/>
To see more information about Storybook, visit: <https://storybook.js.org/>

## Folder structure

```
<project-root>
├─ 📁 .husky
│   ├─ pre-commit
│   ├─ pre-push
├─ 📁 node_modules
├─ 📂 packages
│   ├─ 📂 components
│   │   ├─ 📁 eslint-config-node
│   │      └─ index.js
│   │      └─ package.json
│   ├─ 📂 storybook
│   │   └─ <storybook files>
├─ .eslintignore
├─ .eslintrc.json
├─ .gitignore
├─ lerna.json
├─ package.json
├─ tsconfig.json
├─ vitest.config.ts
└─ <more project root files>
```

## Architecture

### Lerna

Version 7.1.4

### Typescript

Version 5.1.6

### Storybook

Version 7.0.27

## Testing support

Installed all necessary to do tests in future components. To execute it, we have to configure
component scripts (in each package.json) and run it with lerna tasks

```shell
lerna run test
```

This command will trigger test scripts in all components where have it configure

## Husky & Lint-Staged

Husky Version 8.0.3
Lint-staged Version 13.1.0

Improved the development flow using Git Hooks that will be executed before commits and push. It will check if
the linter passes correctly and tests give OK

This ensure that the code you upload to repository has a minimum quality
