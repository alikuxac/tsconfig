# @alikuxac/tsconfig

<p align="center">
  <img src="https://raw.githubusercontent.com/microsoft/fluentui-emoji/main/assets/Gear/3D/gear_3d.png" width="100" height="100" alt="@alikuxac/tsconfig logo" />
</p>

<p align="center">
  <b>Opinionated TypeScript configurations for Node.js, Next.js, and NestJS.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/npm/v/@alikuxac/tsconfig?style=flat-square&color=black" alt="npm version" />
  <img src="https://img.shields.io/npm/l/@alikuxac/tsconfig?style=flat-square&color=black" alt="license" />
  <img src="https://img.shields.io/npm/dm/@alikuxac/tsconfig?style=flat-square&color=black" alt="downloads" />
</p>

---

## Features

- **Strict type checking**: Catches type errors early across all presets.
- **TypeScript 5, 6, and 7 support**: Version-pinned configurations in `src/v5`,
  `src/v6`, and `src/v7`.
- **Project presets**: Presets for base Node/ESM libraries, Next.js with
  compiler plugins, and NestJS with decorators.
- **Zero dependencies**: Pure JSON configuration files.

## Installation

```bash
# npm
npm install --save-dev @alikuxac/tsconfig

# yarn
yarn add -D @alikuxac/tsconfig

# pnpm
pnpm add -D @alikuxac/tsconfig
```

## Usage

Extend a configuration in your `tsconfig.json`.

### Base (Libraries and Node.js)

Default:

```json
{
  "extends": "@alikuxac/tsconfig/base"
}
```

TypeScript 7 target:

```json
{
  "extends": "@alikuxac/tsconfig/v7/base"
}
```

### Next.js

Default:

```json
{
  "extends": "@alikuxac/tsconfig/nextjs"
}
```

TypeScript 7 target:

```json
{
  "extends": "@alikuxac/tsconfig/v7/nextjs"
}
```

### NestJS

Default:

```json
{
  "extends": "@alikuxac/tsconfig/nestjs"
}
```

TypeScript 7 target:

```json
{
  "extends": "@alikuxac/tsconfig/v7/nestjs"
}
```

## Configuration Matrix

| Config      | Target | Module   | Features                |
| :---------- | :----- | :------- | :---------------------- |
| `base` (v5) | ES2022 | ESNext   | Bundler-ready, strict   |
| `nextjs`    | ES2022 | ESNext   | Next.js plugin, JSX     |
| `nestjs`    | ES2021 | CommonJS | Decorators, source maps |
| `v6/base`   | ES2024 | ESNext   | Bundler-ready, strict   |
| `v6/nextjs` | ES2024 | ESNext   | Next.js plugin, JSX     |
| `v6/nestjs` | ES2021 | CommonJS | Decorators, source maps |
| `v7/base`   | ES2025 | ESNext   | Bundler-ready, strict   |
| `v7/nextjs` | ES2025 | ESNext   | Next.js plugin, JSX     |
| `v7/nestjs` | ES2024 | CommonJS | Decorators, source maps |

## License

MIT © [Alikuxac](https://github.com/alikuxac)
