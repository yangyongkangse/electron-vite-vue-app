# electron-vite-vue-app

An Electron application with Vue and TypeScript

## Recommended IDE Setup

- [VSCode](https://code.visualstudio.com/) + [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) + [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)

## Project Setup

### Install

```bash
$ npm install
```

### Development

```bash
$ npm run dev
```

### Build

```bash
# For windows
$ npm run build:win

# For macOS
$ npm run build:mac

# For Linux
$ npm run build:linux
```

```text
├─ /.vscode
├─ /build                      <-- build编译过程性输出目录
├─ /dist                       <-- 最终build的输出目录
├─ /node_modules
├─ /out                        <-- dev和build编译过程性输出目录
├─ /resources                  <-- 主进程和preload的公共资源目录
├─ /src
|  ├─ /main                    <-- 主进程开发目录
|  ├─ /preload                 <-- preload开发目录
|  ├─ /renderer                <-- 渲染进程开发目录
|  |  ├─ /api                  <-- api目录
|  |  |  └─ index.js           <-- api库
|  |  ├─ /common               <-- 全局公用目录
|  |  |  ├─ /fonts             <-- 字体文件目录
|  |  |  ├─ /images            <-- 图片文件目录
|  |  |  ├─ /js                <-- 公用js文件目录
|  |  |  └─ /styles            <-- 公用样式文件目录
|  |  |  |  ├─ frame.styl      <-- 全部公用样式（import本目录其他全部styl）
|  |  |  |  ├─ reset.styl      <-- 清零样式
|  |  |  |  └─ global.styl     <-- 全局公用样式
|  |  ├─ /components           <-- 公共模块组件目录
|  |  |  ├─ /header            <-- 头部导航模块（示例）
|  |  |  |  └─ header.vue      <-- header主文件
|  |  |  └─ ...                <-- 其他模块
|  |  ├─ /views                <-- 页面组件目录
|  |  |  ├─ /home              <-- home页目录
|  |  |  |  └─ home.vue        <-- home主文件
|  |  |  ├─ /login             <-- login页目录
|  |  |  |  └─ login.vue       <-- login主文件
|  |  |  └─ ...                <-- 其他页面
|  |  ├─ /router               <-- 路由配置目录
|  |  |  └─ index.js           <-- 路由配置文件
|  |  ├─ App.vue               <-- 项目页面入口文件
|  |  ├─ main.js               <-- 渲染进程入口文件
|  |  └─ index.html            <-- 渲染进程HTML模板
├─ .editorconfig               <-- IDE配置文件
├─ .eslintignore               <-- 忽略eslint检查的配置文件
├─ .eslintrc.cjs               <-- eslint配置文件
├─ .gitignore
├─ .npmrc                      <-- npm镜像源配置文件
├─ .prettierignore             <-- 忽略prettier代码格式化的配置文件
├─ .prettierrc.yaml            <-- prettier代码格式化配置文件
├─ dev-app-update.yml
├─ electron-builder.yml        <-- build配置文件
├─ electron.vite.config.js     <-- electron-vite配置文件
├─ package.json
├─ README.md
└─ yarn.lock
```
