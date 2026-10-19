# Reimora

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/swapniljadhav0041/reimora)
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fswapniljadhav0041%2Freimora&env=VITE_SUPABASE_URL,VITE_SUPABASE_PUBLISHABLE_KEY,VITE_SUPABASE_PROJECT_ID)

> Modern University Reimbursement & Financial Governance Platform built with TanStack Start, React 19, Tailwind CSS v4, Nitro, and Supabase.

---

## 🚀 One-Click Deployment on Vercel

### Step 1: Import Repository
1. Navigate to **[vercel.com/new](https://vercel.com/new)**.
2. Sign in with your GitHub account (`swapniljadhav0041`).
3. Click **Import** next to `swapniljadhav0041/reimora` (or use [this direct link](https://vercel.com/new/import?s=https%3A%2F%2Fgithub.com%2Fswapniljadhav0041%2Freimora)).

### Step 2: Configure Build Settings
- **Framework Preset**: `Other` or `Vite` (Nitro automatically configures the Vercel Build Output API v3).
- **Build Command**: `npm run build`
- **Output Directory**: Leave empty or `.vercel/output` (automatically detected).
- **Install Command**: `npm install`

### Step 3: Configure Environment Variables
Add the following variables under **Environment Variables**:

| Variable Name | Value |
|---|---|
| `VITE_SUPABASE_URL` | `https://gkovtgloqxpsgfrvsvug.supabase.co` |
| `VITE_SUPABASE_PUBLISHABLE_KEY` | `sb_publishable_qOd7CsMk_PvbAeZh5qwUVg_FD5zmmvP` |
| `VITE_SUPABASE_PROJECT_ID` | `gkovtgloqxpsgfrvsvug` |
| `SUPABASE_URL` | `https://gkovtgloqxpsgfrvsvug.supabase.co` |
| `SUPABASE_PUBLISHABLE_KEY` | `sb_publishable_qOd7CsMk_PvbAeZh5qwUVg_FD5zmmvP` |
| `SUPABASE_PROJECT_ID` | `gkovtgloqxpsgfrvsvug` |

### Step 4: Click Deploy
Click **Deploy**. Vercel will automatically build the site in seconds and provide a live production URL (e.g., `https://reimora-swapniljadhav0041.vercel.app`).

---

## 🟣 Deploy to Render (Web Service)

### Option A: 1-Click Blueprint (Recommended)
1. Go to **[Render New Blueprint](https://dashboard.render.com/select-repo?type=blueprint)**.
2. Select your repository: `swapniljadhav0041/reimora`.
3. Render will automatically read [`render.yaml`](./render.yaml), configure the service name, build commands, and Supabase environment variables on the free tier!
4. Click **Apply**. Your app will build and deploy live at `https://reimora-<unique-id>.onrender.com`.

### Option B: Manual Web Service
1. Go to **[Render New Web Service](https://dashboard.render.com/select-repo?type=web)** and connect `swapniljadhav0041/reimora`.
2. Configure settings:
   - **Environment**: `Node`
   - **Branch**: `main`
   - **Build Command**: `npm install && npm run build`
   - **Start Command**: `node .output/server/index.mjs` (or `npm start`)
   - **Instance Type**: `Free`
3. Add Environment Variables:
   - `NITRO_PRESET`: `render_com`
   - `NODE_VERSION`: `20`
   - `VITE_SUPABASE_URL`: `https://gkovtgloqxpsgfrvsvug.supabase.co`
   - `VITE_SUPABASE_PUBLISHABLE_KEY`: `sb_publishable_qOd7CsMk_PvbAeZh5qwUVg_FD5zmmvP`
   - `VITE_SUPABASE_PROJECT_ID`: `gkovtgloqxpsgfrvsvug`
   - `SUPABASE_URL`: `https://gkovtgloqxpsgfrvsvug.supabase.co`
   - `SUPABASE_PUBLISHABLE_KEY`: `sb_publishable_qOd7CsMk_PvbAeZh5qwUVg_FD5zmmvP`
   - `SUPABASE_PROJECT_ID`: `gkovtgloqxpsgfrvsvug`
4. Click **Create Web Service**.

---

## 💻 Local Development

Ensure you have Node.js 20+ and npm installed:

```sh
# Clone your repository
git clone https://github.com/swapniljadhav0041/reimora.git
cd reimora

# Install dependencies
npm install

# Run locally in dev mode
npm run dev

# Run automated tests
npm test

# Type-check & lint
npx tsc --noEmit
npm run lint

# Production build
npm run build
```

---

## 🛠️ Architecture
- **Framework**: TanStack Start (Full-stack SSR React 19)
- **Engine**: Nitro Server v3 + Vite 8
- **Styling**: Tailwind CSS v4 + Tw-Animate-CSS
- **Database & Auth**: Supabase (PostgreSQL, Storage, RLS)
- **Icons & Visuals**: Lucide React, Recharts, Sonner
