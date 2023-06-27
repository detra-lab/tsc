# TS Configs

[![NPM Version][npm_version_badge]][npm_badge_url]
[![NPM Downloads][npm_downloads_badge]][npm_badge_url]

A collection of TSConfigs to extend in your own apps, tuned to a particular runtime environment.

- [TS Configs](#ts-configs)
  - [Available Configurations](#available-configurations)
  - [License](#license)

## Available Configurations

<details>

<summary><strong>Node.js - CJS</strong></summary>

> A version of Node >= 16 is supported by the following configuration.

To install the configuration and its related dev-dependencies, use the following command:

```sh
pnpm add -D @detra-lab/tsc typescript @types/node@16
```

After the installation, add the code snippet below to your `tsconfig.json` file:

```json
{
  "extends": "@detra-lab/tsc/node/tsconfig.cjs.json",
  "compilerOptions": {
    "declarationDir": "./types",
    "typeRoots": ["./types", "./node_modules/@types"]
  }
}
```

</details>

<details>

<summary><strong>Node.js - ESM</strong></summary>

> A version of Node >= 16 is supported by the following configuration.

To install the configuration and its related dev-dependencies, use the following command:

```sh
pnpm add -D @detra-lab/tsc typescript @types/node@16
```

After the installation, add the code snippet below to your `tsconfig.json` file:

```json
{
  "extends": "@detra-lab/tsc/node/tsconfig.esm.json",
  "compilerOptions": {
    "declarationDir": "./types",
    "typeRoots": ["./types", "./node_modules/@types"]
  }
}
```

</details>

<details>

<summary><strong>Lit</strong></summary>

If you're working on projects that use [Lit](https://lit.dev/) with TypeScript, you can simplify the setup process by installing a configuration and its related dependencies using the following command:

```sh
pnpm add -D @detra-lab/tsc typescript
```

After the installation, add the code snippet below to your `tsconfig.json` file:

```json
{
  "extends": "@detra-lab/tsc/lit/tsconfig.json"
}
```

</details>

<details>

<summary><strong>React.js</strong></summary>

When working on projects that involve using React with TypeScript, such as [Create React App](https://create-react-app.dev/) or [Next.js](https://nextjs.org/), you can simplify the setup process by installing a configuration and its dependencies with a single command:

```sh
pnpm add -D @detra-lab/tsc typescript
```

After the installation, add the code snippet below to your `tsconfig.json` file:

```json
{
  "extends": "@detra-lab/tsc/react/tsconfig.json"
}
```

</details>

## License

[MIT License](./LICENSE)

<!-- Badges -->

[npm_version_badge]: https://img.shields.io/npm/v/@detra-lab/tsc?style=flat-square&colorA=6930C3&colorB=5390D9
[npm_downloads_badge]: https://img.shields.io/npm/dm/@detra-lab/tsc?style=flat-square&colorA=6930C3&colorB=5390D9

<!-- Links -->

[npm_badge_url]: https://www.npmjs.com/package/@detra-lab/tsc
