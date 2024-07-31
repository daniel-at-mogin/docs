## Requirements

- [Yarn v4.2.2](https://yarnpkg.com/)

## Step by Step to Setup Node Express with TypeScript

1. Create new folder for the project

   ```console
   mkdir [folder-name]
   ```

1. `cd` into it

   ```console
   cd [folder-name]
   ```

1. Initialize the project

   ```console
   yarn init -y
   ```

1. Install the dependencies

   ```console
   yarn add express
   ```

   ```console
   yarn add typescript @types/express nodemon ts-node -D
   ```

1. Initialize the typescript configuration file

   ```console
   yarn tsc --init
   ```

1. Configure the `rootDir` and `outDir` in `tsconfig.json`

   ```json
   "compilerOptions" : {
     "rootDir": "./src",
     "outDir": "./dist"
   }
   ```

1. Add new script inside the `package.json` file

   ```json
   "scripts" : {
     "build": "tsc --build",
     "start" : "node ./dist/index.js",
     "start:dev" : "nodemon ./src/index.ts"
   }
   ```

1. Voilà!! You could start working on the `./src/index.ts` by running this command in terminal
   ```console
   yarn start:dev
   ```

Read this documentation in [🇮🇩 Bahasa](./README-IN.md)
