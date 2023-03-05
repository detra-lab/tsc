# TS Configs

A collection of TSConfigs to extend in your own apps, tuned to a particular runtime environment.

- [TS Configs](#ts-configs)
  - [Install](#install)
  - [Available Configurations](#available-configurations)
  - [License](#license)

## Install

```sh
# NPM
npm add --save-dev @detra-lab/tsc typescript

# PNPM
pnpm add --save-dev @detra-lab/tsc typescript

# Yarn
yarn add --dev @detra-lab/tsc typescript
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
