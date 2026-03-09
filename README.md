# Banner 策略管理后台 (原型)

## 项目简介
这是一个基于 Vue 3 + Element Plus 的纯前端原型项目，用于演示 Banner 策略管理后台的功能。
项目包含一个简单的 Node.js 服务器 (`server.cjs`) 用于本地预览。

## 目录结构
- `index.html`: 主页面，包含所有前端逻辑（Vue + Element Plus）。
- `server.cjs`: 本地开发服务器（仅用于本地预览，**请勿用于生产环境**）。
- `vercel.json`: Vercel 部署配置文件（用于静态托管）。

## 本地运行
1. 确保已安装 Node.js。
2. 在终端运行：
   ```bash
   node server.cjs
   ```
3. 浏览器访问：http://localhost:8080

## 部署说明
本项目已配置 `vercel.json`，可直接部署到 Vercel。
由于 Vercel 是 Serverless 架构，它会自动托管静态文件 (`index.html`)，而忽略 `server.cjs`（因为 Serverless 环境不支持长连接服务器）。

**注意**：线上环境直接访问 `index.html` 即可。
