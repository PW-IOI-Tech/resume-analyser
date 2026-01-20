# Project Name

> An intelligent platform that leverages AI to analyze resumes against job descriptions and provides ATS-friendly resume building tools.

This project is maintained under **PW Institute of Innovation – Open Source** and follows real-world open-source development practices.

---

## Getting Started

### Prerequisites

- Git
- Node.js / Python / Javascript
- npm package manager for javascript
- uv package manager for python

### Installation

#### Frontend

1. Head over to the frontend directory: 
  ```bash
  cd frontend
  ```
2. Install dependencies
  ```bash
  npm install
  ```
3. Run development
  ```bash
  npm run dev
  ```


#### Backend

#### FastAPI:

1. Head over to the fastapi backend
  ```bash
  cd backend/fastapi-backend
  ```
1. Create env file
  ```bash
  cp .env.example .env
  ```
2. Replace `.env` with original values
3. Install dependencies:
  ```bash
  uv sync
  ```
4. Run main fast-api server 
  ```bash
  uv run src/main.py
  ```


#### Express

1. Head over to the express backend
  ```bash
  cd backend/express-backend
  ```
1. Create env file
  ```bash
  cp .env.example .env
  ```
2. Replace `.env` with original values
3. Install dependencies:
  ```bash
  npm install
  ```
4. Run main express server 
  ```bash
  npm run dev
  ```


## Project Structure

```text
.
├── backend
│   ├── express-backend
│   │   ├── prisma
│   │   │   └── migrations
│   │   │       ├── 20250619130950_init
│   │   │       └── 20250620115923_add_token_models
│   │   └── src
│   │       ├── config
│   │       ├── controllers
│   │       ├── mail-service
│   │       ├── middlewares
│   │       ├── routes
│   │       └── utils
│   └── fastapi-backend
│       ├── logs
│       └── src
│           ├── core
│           └── features
│               ├── resume
│               │   └── utils
│               └── users
└── frontend
    ├── app
    │   ├── (auth)
    │   │   ├── forgot-password
    │   │   ├── reset-password
    │   │   │   └── [token]
    │   │   ├── signin
    │   │   ├── signup
    │   │   └── verify-email
    │   └── dashboard
    │       ├── help-support
    │       ├── jd-matcher
    │       │   └── resume-analysis
    │       ├── profile
    │       ├── resume-builder
    │       │   └── edit
    │       ├── resume-manager
    │       └── skill-assessment
    ├── components
    │   ├── auth
    │   ├── dashboard
    │   │   ├── jd-matcher
    │   │   ├── resume-builder
    │   │   ├── resume-manager
    │   │   └── skill-assessment
    │   └── ui
    ├── context
    ├── lib
    ├── services
    └── types
```

---

## Git Flow

This project follows Git Flow:

| Branch     | Use case           |
| ---------- | ------------------ |
| main       | Production-ready   |
| develop    | Active development |
| feature/\* | New features       |
| bugfix/\*  | Bug fixes          |
| hotfix/\*  | Critical fixes     |

### Development Rules

- All work branches must be created from `develop`
- Pull Requests must target `develop`
- Direct commits to `main` are **not allowed**

### Hotfixes

- `hotfix/*` branches are created from `main`
- Hotfix PRs must be merged into both `main` and `develop`

### Releases

- Releases are prepared from `develop`
- Final merges go into `main`
- Releases are tagged using semantic versioning
  (`v1.0.0`, `v1.1.0`, etc.)

---

## Issues & Features

Use the provided Issue Templates:

- Bug Report
- Feature Request
- Documentation
- Chore

Blank issues are disabled.

## Label System

We use a consistent labeling system across all repositories.

| Issue Types     | Difficulty         | Status         | Priority           |
| --------------- | ------------------ | -------------- | ------------------ |
| `bug`           | `good first issue` | `help wanted`  | `priority: high`   |
| `feature`       | `easy`             | `in progress`  | `priority: medium` |
| `enhancement`   | `medium`           | `blocked`      | `priority: low`    |
| `documentation` | `hard`             | `needs review` |
| `refactor`      |                    |                |
| `chore`         |                    |                |
| `discussion`    |                    |                |

Please use:

- **One Issue Type**
- **One Difficulty**
- **One Priority (optional)**
- **One Status (maintainers only)**

This helps us triage and respond faster.

---

## Pull Requests

- Follow the PR template
- Link issues using Fixes #<issue-number>
- Ensure all checks pass before review

---

## Credits

- **Original Author(s):** [Shoyeb45](), [Mitesh](), [Aryan]() 
- **Maintainers:** See repository contributors

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details.

---

## Code of Conduct

See [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).

---

## License

Add your license information here.
