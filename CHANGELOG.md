# @alikuxac/tsconfig

## 1.3.0

### Minor Changes

- Add TypeScript 7 presets in `src/v7/`:
  - `v7/base`: Target `es2025`, `lib: ["es2025", "dom", "dom.iterable"]`, and
    `moduleResolution: "bundler"`.
  - `v7/nextjs`: Extends `v7/base` with Next.js plugin and preserved JSX.
  - `v7/nestjs`: Target `es2024`, CommonJS modules, and decorator metadata.
- Export `./v7/base`, `./v7/nextjs`, and `./v7/nestjs` in `package.json`.
- Include `src/**/*.json` in `package.json` `files` to bundle version
  directories.
- Bump `typescript` devDependency to `^7.0.2`.
- Fix broken logo link in `README.md` and document TypeScript 7 in configuration
  matrix.
- Remove Changesets in favor of direct tag-triggered `npm publish` in release
  workflow.
- Update release workflow to `actions/checkout@v7` and `actions/setup-node@v7`,
  and remove `registry-url` to fix npm OIDC publishing.

## 1.2.1

### Patch Changes

- Update package configurations and dependencies.
- Optimize GitHub Action: Trigger release only on tag push.

## 1.2.0

### Minor Changes

- Support both TypeScript v5 and v6.
- Add optimized configuration for TypeScript 6.0 with `target: es2024`.
- Restructure `src/v5/` and `src/v6/` directories for better version management.
- Update `package.json` exports to support versioned mappings (e.g.,
  `@alikuxac/tsconfig/v6/base`).
- Update devDependencies (TypeScript 6.0.2, Prettier 3.8.1) and Yarn 4.13.0.

## 1.1.9

### Patch Changes

- fix: final attempt to achieve green build status after fixing github action
  permissions
- chore: remove redundant `publish` script from `package.json`

## 1.1.8

### Patch Changes

- fix: fix workflow permissions to enable successful git tagging after publish

## 1.1.7

### Patch Changes

- fix: final attempt to stabilize the release pipeline with refreshed registry
  configuration

## 1.1.6

### Patch Changes

- fix: final adjustment to oidc workflow to ensure a green status on github
  actions

## 1.1.5

### Patch Changes

- fix: switch to npm run release in workflow to avoid yarn berry interference

## 1.1.4

### Patch Changes

- fix: meticulously align workflow with proven patterns for oidc publish and
  tagging

## 1.1.3

### Patch Changes

- fix: final refinement of oidc publish workflow based on proven patterns

## 1.1.2

### Patch Changes

- fix: refine github actions workflow for stable oidc publish

## 1.1.1

### Patch Changes

- fix: retry publish with correct environment and provenance

## 1.1.0

### Minor Changes

- feat: add specialized tsconfig files for base, nextjs, and nestjs

## 1.0.3

### Patch Changes

- cff6da3: chore(deps): update actions/checkout action to v4
- 0f3b775: chore(deps): update all non-major dependencies
- 6217738: chore(deps): bump semver from 5.7.1 to 5.7.2
- 77f2ae4: chore(deps): update dependency typescript to v5
- e6f20ae: chore(deps): update dependency prettier to ^3.2.4
- 021fd9b: chore(deps): update dependency prettier to ^3.0.1
- e3dcc6d: chore(deps): update dependency prettier to v3
