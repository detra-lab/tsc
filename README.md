# TS Configs

[![NPM Version][npm_version_badge]][npm_badge_url]
[![NPM Downloads][npm_downloads_badge]][npm_badge_url]

A collection of TSConfigs to extend in your own apps, tuned to a particular runtime environment.

- [TS Configs](#ts-configs)
  - [Install](#install)
  - [Available Configurations](#available-configurations)
  - [License](#license)

## Install

```sh
pnpm add -D @detra-lab/tsc typescript
```

## Available Configurations

<details>

<summary><strong>Node.js - CJS</strong></summary>

> ⚠️ The following configuration supports a version of Node >= 16.

Add to your `tsconfig.json`:

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

> ⚠️ The following configuration supports a version of Node >= 16.

Add to your `tsconfig.json`:

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

<summary><strong>React.js</strong></summary>

> ⚠️ The following configuration is helpful in projects based on Create React App and Next.js.

Add to your `tsconfig.json`:

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
