# Express TypeScript Starter 

![node typescript express docker logos](https://user-images.githubusercontent.com/2646053/191009021-82d404d7-3d51-4dd3-ad0a-51009f89e048.png)

[📷](https://github.com/ljlm0402/typescript-express-starter)

## Definitions

| Library | Description |
| ------- | ----------- |
| Express | Minimal and flexible Node.js web application framework for creating [APIs](https://en.wikipedia.org/wiki/API). |
| TypeScript | A [strongly typed](https://en.wikipedia.org/wiki/Strong_and_weak_typing) programming language that builds on JavaScript, giving you better tooling at any scale. |
| ESLint  | [Statically analyzes](https://en.wikipedia.org/wiki/Static_program_analysis) your code to quickly find problems. |
| Jest    | A delightful JavaScript testing framework with a focus on simplicity. |
[ Docker  | Package software into standardized units for development, shipment and deployment |

## About

This is a template repo for building a [Node.js](https://nodejs.org/en/) [API](https://en.wikipedia.org/wiki/API) with [Express](https://expressjs.com/) using [TypeScript](https://www.typescriptlang.org/). This repo contains a minimal [ESLint](https://eslint.org/) configuration to enforce coding styles, and comes equipped with [Jest](https://jestjs.io/) for unit and integration testing. Additionally, this repo demonstrates organizing controllers similarly to how components are organized in an [Angular](https://angular.io/guide/file-structure) project. Controllers are grouped by the API resource they serve, and the associated unit (spec.ts) and integration (e2e.ts) files live in the same directory. Finally, this template leverages [Docker](https://www.docker.com/) and [Remote Containers](https://code.visualstudio.com/docs/remote/containers) to ensure consistency in development and production environments.

## Getting Started

The recommended development method for this repo is via a Remote Container and VS Code. As your development environment grows in complexity you can leverage Docker to manage said complexity. Docker will automatically manage development environments so that you don't waste time manually configuring systems for every user that wants to help you develop your app.

### Development Container

Install [Docker Desktop](https://www.docker.com/products/docker-desktop/), [VS Code](https://code.visualstudio.com/download) and [Git](https://git-scm.com/downloads). Open VS Code and install the [Docker extension](https://code.visualstudio.com/docs/containers/overview#_installation) and the [Remote Containers extension](https://code.visualstudio.com/docs/remote/containers-tutorial#_install-the-extension).

Click the green [Use this template](https://github.com/bobbyg603/express-typescript-starter/generate) button to copy this repo to your GitHub account. Once you've copied the repo, clone it to your workspace (be sure to replace my URL with the URL to the repo you generated by clicking `Use this template`):

```sh
git clone https://github.com/bobbyg603/node-typescript-express-docker-starter
```

Open the downloaded repo in VS Code and ensure Docker Desktop is running. If you've installed the Docker and Remote Containers extensions correctly you should be prompted to open the project in a Remote Container.

<img width="769" alt="open in remote container" src="https://user-images.githubusercontent.com/2646053/191012971-e087ef57-2f2d-4d54-a79b-bed577669a3c.png">

If you're not prompted to open the workspace in a Remote Container, you can also open the repo in a Remote Container via the [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette)

<img width="881" alt="vs code command palette" src="https://user-images.githubusercontent.com/2646053/191013677-bb8bd90d-66cc-4577-9ad0-854de75f1b27.png">

This will leverage [Dockerfile.dev](todo bg) to build a container and install project's dependencies with npm. Once the workspace has loaded you can run the unit and integration tests to ensure everything installed correctly:

```sh
npm test && npm run e2e
```

Start the development server:

```sh
npm start
```

The development server should begin listening for web requests. If you navigate to https://localhost:3000 in your browser you should see something that resembles the following:

<img width="1728" alt="image" src="https://user-images.githubusercontent.com/2646053/188285900-dd9af5d3-95fc-43a0-ab65-3dc1305d1da2.png">
