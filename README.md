# React Monorepo Template Project
This is a base React project using monorepo architecture. It uses Typescript and yarn 2 as package manager, included eslint, commitlint, husky,...
## How to use
Step 1: Place your React app at /src/apps and your packages at /src/packages.
Step 2: Config your app/package name in package.json file
Step 3: In root package.json script, you can run children package command using Yarn workspace
```json
"scripts": {
  "<command here>": "yarn workspace <Your app name in package.json> <command>"
}
```
For example:
```json
"scripts": {
  "dev:test-app": "yarn workspace test-app dev",
  "build:test-app": "yarn workspace test-app build"
}
```
