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

这里主要是解释在 Vite 是如何处理 CSS 文件的：
导入 `.css` 文件将会把内容插入到 `<style>` 标签中，同时也带有 HMR 支持。

#### Build-time imports

Vite 通过 `postcss-import` 预配置支持了 CSS `@import` 内联，Vite 的路径别名也遵从 CSS `@import`。**就是说不需要在postcss-load-config里配置它**。
实现的功能就是可以使用 `@import` 时导入多个 CSS 文件（在构建时完成），不必等到浏览器加载时再去发送网络请求导入 CSS 文件。

#### Using PostCSS as your preprocessor

CSS 文件将由 PostCSS 处理。如果项目包含有效的 PostCSS 配置，它将会自动应用于所有已导入的 CSS。

#### Optimizing for Production

Vite 默认使用 `esbuild` 来最小化 CSS。

## Tailwindcss

使用 `theme()` 函数，使用点符号访问 Tailwind 配置值。
