# Campus Lost and Found - Frontend

Modern web frontend for the **Campus Lost and Found** platform, built with React 19, Vite, Tailwind CSS v4, and React Router 7.

---

## 🚀 Tech Stack

- **Framework**: [React 19](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Routing**: [React Router v7](https://reactrouter.com/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/) + [Radix UI](https://www.radix-ui.com/) / [shadcn/ui](https://ui.shadcn.com/)
- **State & Data Fetching**: [TanStack Query v5](https://tanstack.com/query/latest)
- **Forms & Validation**: [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Notifications**: [Sonner](https://sonner.emilkowal.ski/)
- **3D / Visuals**: [Three.js](https://threejs.org/)

---

## 🛠️ Getting Started

### 1. Prerequisites
- [Node.js](https://nodejs.org/) (version 18+ or 20+ recommended)
- npm, yarn, or pnpm

### 2. Installation
```bash
npm install
```

### 3. Environment Variables
Copy `.env.example` to `.env`:
```bash
cp .env.example .env
```

Configure your backend API base URL (must include trailing slash):
```env
VITE_API_URL=http://localhost:3001/
```

### 4. Run Development Server
```bash
npm run dev
```
The app will be available at `http://localhost:5173`.

---

## 📦 Production Build

```bash
npm run build
```
The optimized production bundle will be created in the `dist` directory.

To preview the production build locally:
```bash
npm run preview
```

---

## 🌐 Deployment

### Deploying to Vercel
1. Import this repository into Vercel.
2. Set Framework Preset: **Vite**.
3. Build Command: `npm run build`.
4. Output Directory: `dist`.
5. Under **Environment Variables**, add:
   - `VITE_API_URL`: `https://<your-backend-api-url>/` (e.g. `https://campus-lost-found-api.onrender.com/`)
6. Deploy! (`vercel.json` is included for SPA route rewrites).

### Deploying to Netlify
1. Connect this repository to Netlify.
2. Build Command: `npm run build`.
3. Publish Directory: `dist`.
4. Under **Site Configuration > Environment Variables**, add:
   - `VITE_API_URL`: `https://<your-backend-api-url>/`
5. Deploy! (`public/_redirects` is included for SPA client-side routing).
