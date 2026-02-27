# Vercel 部署指南

## 前提条件

在部署到 Vercel 之前，您需要：

1. **Node.js 和 npm**：Vercel CLI 需要 Node.js 环境
2. **Vercel 账户**：在 [Vercel 官网](https://vercel.com/) 注册一个账户
3. **Git**：用于版本控制（可选但推荐）

## 安装步骤

### 1. 安装 Node.js 和 npm

访问 [Node.js 官网](https://nodejs.org/) 下载并安装最新版本的 Node.js，npm 会随 Node.js 一起安装。

### 2. 安装 Vercel CLI

打开命令行工具，运行以下命令安装 Vercel CLI：

```bash
npm install -g vercel
```

### 3. 登录 Vercel

```bash
vercel login
```

按照提示完成登录流程。

## 部署步骤

### 方法 1：使用 Vercel CLI 部署

1. **进入项目目录**：

```bash
cd c:\Users\angeh\Desktop\vibe\TRAE
```

2. **初始化并部署**：

```bash
vercel
```

按照提示完成部署配置：
- 项目名称：可自定义
- 部署位置：默认即可
- 其他选项：默认即可

### 方法 2：使用 Vercel 网站部署

1. **访问 Vercel 控制台**：https://vercel.com/dashboard

2. **点击 "New Project"**

3. **选择 "Import Project"**

4. **选择 "Import Git Repository"**（如果您已将项目上传到 GitHub、GitLab 或 Bitbucket）

   或者选择 "Deploy from Local Folder"，然后拖拽您的项目文件夹（`c:\Users\angeh\Desktop\vibe\TRAE`）到指定区域。

5. **配置部署设置**：
   - Framework Preset：选择 "Other"（因为这是一个静态网站）
   - Build Command：留空
   - Output Directory：留空
   - Root Directory：留空

6. **点击 "Deploy"** 开始部署

## 部署完成

部署完成后，Vercel 会为您生成一个唯一的 URL，您可以通过这个 URL 访问您的网站。

## 项目结构说明

您的项目是一个静态网站，包含以下主要文件：
- `Angehand.html`：主页
- `timeline.html`：时间线页面
- `ColorFinder.html`：颜色查找工具
- `gomoku.html`：五子棋游戏
- `计时器/`：番茄钟计时器应用

Vercel 会自动识别这些静态文件并正确部署。