# Fake Review Detection - Frontend

React + TypeScript + Vite frontend for the Fake Review Detection system.

## 🚀 Features

- Modern React 18 with TypeScript
- Supabase authentication and database
- Beautiful UI with Tailwind CSS and shadcn/ui
- Data visualization with Recharts
- Form handling with React Hook Form
- Responsive design

## 📋 Prerequisites

- Node.js 18+
- npm or yarn
- Supabase account

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/hitesh-patgar/fake-review-frontend.git
cd fake-review-frontend
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file:
```bash
cp .env.example .env
```

4. Update `.env` with your Supabase credentials:
```env
VITE_SUPABASE_URL="your-supabase-url"
VITE_SUPABASE_PUBLISHABLE_KEY="your-supabase-anon-key"
```

## 🏃 Running Locally

```bash
npm run dev
```

The app will be available at `http://localhost:5173`

## 🏗️ Build

```bash
npm run build
```

## 🚢 Deployment

### Vercel

1. Install Vercel CLI:
```bash
npm i -g vercel
```

2. Deploy:
```bash
vercel
```

3. Set environment variables in Vercel Dashboard:
   - `VITE_SUPABASE_URL`
   - `VITE_SUPABASE_PUBLISHABLE_KEY`

### Manual Deployment

1. Build the project: `npm run build`
2. Upload the `dist` folder to your hosting provider

## 📁 Project Structure

```
fake-review-frontend/
├── src/
│   ├── components/      # React components
│   ├── hooks/          # Custom React hooks
│   ├── integration/    # Supabase integration
│   ├── lib/            # Utility functions
│   ├── pages/          # Page components
│   ├── App.tsx         # Main app component
│   └── main.tsx        # Entry point
├── public/             # Static assets
├── supabase/           # Supabase config and migrations
├── .env.example        # Environment variables template
└── .gitignore         # Git ignore rules
```

## 🎨 Tech Stack

- **Framework:** React 18 + TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS
- **UI Components:** shadcn/ui
- **Backend:** Supabase
- **Charts:** Recharts
- **Forms:** React Hook Form
- **Routing:** React Router

## 🔒 Security

- Never commit `.env` files to Git
- Keep Supabase keys secure
- Use environment variables for all sensitive data
- Rotate credentials if exposed

## 📝 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## 📝 License

MIT License
