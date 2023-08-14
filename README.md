# vue-tailwindcss-starter

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
pnpm install
```

### Compile and Hot-Reload for Development

```sh
pnpm dev
```

### Compile and Minify for Production

```sh
pnpm build
```

### Lint with [ESLint](https://eslint.org/)

```sh
pnpm lint
```

## Vite官方中文文档

Vite主要由两部分组成：一个开发服务器，它基于 原生 ES 模块 提供了 丰富的内建功能；一套构建指令输出用于生产环境的静态资源。

### CSS

导入 `.css` 文件将会把内容插入到 `<style>` 标签中，同时也带有 HMR 支持。

#### Build-time imports

预处理器提供的最有用的功能之一就是将 CSS 整理成多个文件，并在构建时通过提前处理 @import 语句（而不是在浏览器中）将它们组合起来。
Vite 通过 `postcss-import` 预配置支持了 CSS `@import` 内联，Vite 的路径别名也遵从 CSS `@import`。

#### Using PostCSS as your preprocessor

CSS 文件将由 PostCSS 处理。如果项目包含有效的 PostCSS 配置，它将会自动应用于所有已导入的 CSS。
