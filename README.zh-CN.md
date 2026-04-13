<div align="center">
  <img src="src/assets/sneezing-cat.svg" alt="Sneezing Cat" width="160" />
  <h1>喵影 · CatGallery Web</h1>
  <p>
    <strong>基于 React 19 + Ant Design 构建的现代化猫咪图片画廊</strong>
  </p>
  <p>
    <a href="./README.md">English</a>
  </p>
</div>

---

## 项目简介

CatGallery Web 是一个现代化的猫咪图片画廊 Web 应用。支持用户登录认证、角色权限管理、响应式瀑布流图片浏览和管理员后台，基于 React 19、Ant Design 6 和 Vite 7 构建。

## 主要功能

- 猫咪图片画廊，响应式瀑布流布局，懒加载
- 基于 Token 的用户认证，支持"记住我"
- 角色权限控制（管理员 / 普通用户）
- 深色 / 浅色模式一键切换
- 适配移动端的响应式设计
- Vite 热更新 + Mock 登录，无需后端即可开发

## 技术栈

| 层级 | 技术 |
|------|------|
| 框架 | React 19（Hooks） |
| UI 组件库 | Ant Design 6 |
| 路由 | React Router 7 |
| 构建工具 | Vite 7 |
| 样式 | CSS Modules |
| 测试 | Vitest + React Testing Library |

## 快速开始

```bash
npm install
npm run dev      # → http://localhost:5173
npm run build    # 生产构建
npm test         # 运行测试
```

## 开发模式 Mock 账号

| 用户名 | 密码 | 角色 |
|--------|------|------|
| admin | admin123 | 管理员 |
| user | user123 | 普通用户 |

## 项目结构

```
src/
├── views/            # 页面视图
│   ├── Index.jsx     # 首页（登录 + 画廊）
│   └── Admin.jsx     # 管理员后台
├── services/         # 服务层
│   ├── auth.service.js  # 认证 & Token 管理
│   └── api.js           # API 请求封装
├── assets/           # 静态资源
│   └── sneezing-cat.svg
├── App.jsx           # 根组件（路由配置）
└── main.jsx          # 应用入口
```

## 开源协议

MIT
