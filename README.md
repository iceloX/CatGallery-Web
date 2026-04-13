<div align="center">
  <img src="src/assets/sneezing-cat.svg" alt="Sneezing Cat" width="160" />
  <h1>CatGallery Web · 喵影</h1>
  <p>
    <strong>A modern cat photo gallery built with React 19 + Ant Design</strong>
  </p>
  <p>
    <a href="./README.zh-CN.md">简体中文</a>
  </p>
</div>

---

## Overview

CatGallery Web is a modern web application for browsing and managing cat photos. It features user authentication, role-based access control, a responsive waterfall-layout photo gallery, and an admin dashboard — all built with React 19, Ant Design 6, and Vite 7.

## Key Features

- Cat photo gallery with responsive waterfall layout and lazy loading
- Token-based authentication with "Remember Me" support
- Role-based access control (Admin / User)
- Dark / Light mode toggle
- Mobile-friendly responsive design
- Fast dev experience with Vite HMR and mock login (no backend needed)

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | React 19 (Hooks) |
| UI Library | Ant Design 6 |
| Routing | React Router 7 |
| Build Tool | Vite 7 |
| Styling | CSS Modules |
| Testing | Vitest + React Testing Library |

## Quick Start

```bash
npm install
npm run dev      # → http://localhost:5173
npm run build    # production build
npm test         # run tests
```

## Mock Accounts (Dev Mode)

| Email | Password | Role |
|-------|----------|------|
| admin | admin123 | Admin |
| user | user123 | User |

## Project Structure

```
src/
├── views/            # Page views
│   ├── Index.jsx     # Homepage (login + gallery)
│   └── Admin.jsx     # Admin dashboard
├── services/         # Service layer
│   ├── auth.service.js  # Auth & token management
│   └── api.js           # API request wrapper
├── assets/           # Static assets
│   └── sneezing-cat.svg
├── App.jsx           # Root component (routes)
└── main.jsx          # App entry
```

## License

MIT
