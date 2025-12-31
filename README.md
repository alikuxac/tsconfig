# @alikuxac/tsconfig

<p align="center">
  <img src="https://raw.githubusercontent.com/microsoft/fluentui-emoji/main/assets/Gear/Flat/Gear_flat.png" width="100" height="100" />
</p>

<p align="center">
  <b>A collection of opinionated, premium TypeScript configurations for modern web development.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/npm/v/@alikuxac/tsconfig?style=flat-square&color=black" alt="npm version" />
  <img src="https://img.shields.io/npm/l/@alikuxac/tsconfig?style=flat-square&color=black" alt="license" />
  <img src="https://img.shields.io/npm/dm/@alikuxac/tsconfig?style=flat-square&color=black" alt="downloads" />
</p>

---

## 🚀 Features

- **Strict by default**: Encourages best practices and type safety.
- **Specialized**: Configurations for Base, Next.js, and NestJS.
- **Modern**: Targeted for Node.js 20+ and modern ESM/CJS environments.
- **Lightweight**: Zero dependencies, just pure JSON.

## 📦 Installation

```bash
# Using npm
npm install --save-dev @alikuxac/tsconfig

# Using yarn
yarn add -D @alikuxac/tsconfig

# Using pnpm
pnpm add -D @alikuxac/tsconfig
```

## 🛠 Usage

Extend the configuration in your `tsconfig.json` file.

### 🌟 Base (General Purpose)
Perfect for standard library or Node.js projects.
```json
{
  "extends": "@alikuxac/tsconfig/base"
}
```

### ⚛️ Next.js
Optimized for Next.js applications with proper plugin support.
```json
{
  "extends": "@alikuxac/tsconfig/nextjs"
}
```

### 🦁 NestJS
Tailored for NestJS/Backend projects with decorator support.
```json
{
  "extends": "@alikuxac/tsconfig/nestjs"
}
```

## ⚙️ Configuration Matrix

| Config | Target | Module | Features |
| :--- | :--- | :--- | :--- |
| `base` | ES2022 | ESNext | Bundler-ready, Strict |
| `nextjs` | ES2022 | ESNext | + Next.js Plugin, JSX |
| `nestjs` | ES2021 | CommonJS | + Decorators, SourceMaps |

## 📜 License

MIT © [Alikuxac](https://github.com/alikuxac)
