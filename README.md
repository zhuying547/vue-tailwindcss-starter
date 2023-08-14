# vue-tailwindcss-starter

This template should help get you started developing with Vue 3 in Vite.Setting up Tailwind CSS in a Vite project.

## Vite

Vite主要由两部分组成：

- 一个开发服务器，它基于**原生 ES 模块**提供了丰富的功能。
- 一套构建指令，使用 **Rollup** 打包代码，携带默认配置用于生产环境的资源构建。

### 功能

#### CSS 处理

导入 `.css` 文件将会把内容插入到 `<style>` 标签中，同时也带有 HMR 支持。

#### Build-time imports

Vite 通过 `postcss-import` 支持 CSS `@import` 内联，Vite 的路径别名也遵从 CSS `@import`。

> 预配置的功能，不需要后期再手动配置了。

实现的功能就是可以使用 `@import` 时导入多个 CSS 文件（在构建时完成），不必等到浏览器加载时再去发送网络请求导入 CSS 文件。

#### Using PostCSS as your preprocessor

CSS 文件将由 PostCSS 处理。如果项目包含有效的 PostCSS 配置，它将会自动应用于所有已导入的 CSS。

#### Optimizing for Production

Vite 默认使用 `esbuild` 来最小化 CSS。

## Tailwindcss

使用 `theme()` 函数，使用点符号访问 Tailwind 配置值。
