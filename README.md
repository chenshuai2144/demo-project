## 一步步搭建一个复杂的项目

## 初始化项目

```shell
npm i pnpm -g

mkdir simple

cd simple

pnpm dlx create-umi@latest

# 这里我们选择 simple 模板
✔ Install the following package: create-umi? (Y/n) · true
✔ Pick Npm Client › pnpm
✔ Pick Npm Registry › taobao
```

### 1. 项目结构

```bash
.
├── config
│   └── config.ts
├── dist
├── mock
│   └── app.ts｜tsx
├── src
│   ├── .umi
│   ├── .umi-production
│   ├── layouts
│   │   ├── BasicLayout.tsx
│   │   ├── index.less
│   ├── models
│   │   ├── global.ts
│   │   └── index.ts
│   ├── pages
│   │   ├── index.less
│   │   └── index.tsx
│   ├── utils // 推荐目录
│   │   └── index.ts
│   ├── services // 推荐目录
│   │   └── api.ts
│   ├── app.(ts|tsx)
│   ├── global.ts
│   ├── global.(css|less|sass|scss)
│   ├── overrides.(css|less|sass|scss)
│   ├── favicon.(ico|gif|png|jpg|jpeg|svg|avif|webp)
│   └── loading.(tsx|jsx)
├── node_modules
│   └── .cache
│       ├── bundler-webpack
│       ├── mfsu
│       └── mfsu-deps
├── .env
├── plugin.ts
├── .umirc.ts // 与 config/config 文件 2 选一
├── package.json
├── tsconfig.json
└── typings.d.ts
```

### 启动项目

```shell
pnpm i

pnpm run start
```

我们会看到

![启动](./B182905C-FFC0-449a-83D3-8DD2582C68C7.png)

## 增加 layout 功能
