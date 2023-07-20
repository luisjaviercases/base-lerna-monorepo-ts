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
lerna bootstrap
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
└─ <more project root files>
```

## Architecture

### Lerna

Version 6.6.2

### Typescript

Version 5.1.6

### Storybook

Version 7.0.27
