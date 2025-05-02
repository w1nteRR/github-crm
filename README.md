
# GitHub CRM

This is a monorepo for a CRM system.

---

## 📦 Project Structure

```
.
├── frontend/      # React interface
├── backend/       # NestJS + Docker + Prisma
├── package.json 
├── pnpm-workspace.yaml
```

---

## 🚀 Quick Start

### 1. Clone the Repository

> ⚠️ This project uses Git submodules — clone it with the following flag:

```bash
git clone --recurse-submodules https://github.com/w1nteRR/github-crm.git
```

Navigate to the project directory:

```bash
cd github-crm
```

---

### 2. Install Dependencies

This project uses [`pnpm`](https://pnpm.io/).

#### Install `pnpm` if not already installed:

```bash
npm install -g pnpm
```

#### Install all dependencies:

```bash
pnpm install:all
```

Or separately:

```bash
pnpm install:frontend
pnpm install:backend
```

---

### 3. Run the Project

#### ✅ Start the backend (NestJS + Docker):

```bash
pnpm backend:up
```

#### ⛔ Stop the backend:

```bash
pnpm backend:down
```

#### 🔄 Reset the database (delete & apply migrations again):

```bash
pnpm backend:reset
```

> Uses `prisma migrate reset` inside the `nest-app` container.

---

#### ▶️ Start the frontend in development mode:

```bash
pnpm frontend:dev
```

---

#### 🚀 Start both frontend and backend:

```bash
pnpm dev:all
```

---

## 📋 Requirements

- Node.js `>=22`
- [pnpm](https://pnpm.io/) `>=8`
- Docker + Docker Compose
