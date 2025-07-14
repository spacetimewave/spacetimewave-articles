# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Installation

1. Install Volta.

2. Install Node and npm with Volta

3. Install pnpm globally

```bash
npm install -g pnpm
```

4. Create docusaurus project

```bash
npx create-docusaurus@latest spacetimewave-articles classic --typescript        # pnpm create docusaurus
```

5. Add developer dependencies

```bash
pnpm add --save-dev typescript @docusaurus/module-type-aliases @docusaurus/tsconfig @docusaurus/types
```

5. Run docusaurus server

```bash
pnpm run start
```


6. Open http://localhost:3000/

7. Build docusaurus

```bash
pnpm run build
```

## Local Development

```bash
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build

```bash
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Using SSH:

```bash
USE_SSH=true yarn deploy
```

Not using SSH:

```bash
GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
