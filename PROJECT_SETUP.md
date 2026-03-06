# 🚀 Project Setup Guide

## 📋 Wymagania

### System Requirements
- **Node.js:** 18.0.0 lub nowszy
- **npm:** 8.0.0 lub nowszy (lub yarn 1.22.0+)
- **Git:** Latest version
- **Przeglądarka:** Chrome 90+, Firefox 88+, Safari 14+

### Development Tools (zalecane)
- **VS Code** + extensions:
  - ES7+ React/Redux/React-Native snippets
  - Tailwind CSS IntelliSense
  - Auto Rename Tag
  - Prettier - Code formatter
  - ESLint

---

## 🛠️ Instalacja

### 1. Klonowanie repozytorium

```bash
git clone https://github.com/WilkorPLYT/HedenCargoWeb-Web.git
cd HedenCargoWeb-Web
```

### 2. Instalacja zależności

```bash
# Używając npm
npm install

# Lub używając yarn
yarn install
```

### 3. Sprawdzenie instalacji

```bash
# Sprawdź wersję Node.js
node --version

# Sprawdź wersję npm
npm --version

# Sprawdź czy Vite działa
npm run dev --version
```

---

## ⚙️ Konfiguracja

### 1. Zmienne środowiskowe

Utwórz plik `.env.local`:

```env
# API URLs
VITE_API_URL=http://localhost:3001/api
VITE_DISCORD_WEBHOOK_URL=https://discord.com/api/webhooks/...

# Google Analytics
VITE_GA_ID=G-XXXXXXXXXX

# Mapy API
VITE_MAPS_API_KEY=your_google_maps_api_key

# Inne
VITE_APP_NAME=HEDEN Cargo Web
VITE_APP_VERSION=1.0.0
```

### 2. Konfiguracja TailwindCSS

Edytuj `tailwind.config.js`:

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {
      colors: {
        primary: {
          50: '#eff6ff',
          500: '#3b82f6',
          600: '#2563eb',
          700: '#1d4ed8',
        },
        secondary: {
          50: '#f0fdf4',
          500: '#22c55e',
          600: '#16a34a',
          700: '#15803d',
        }
      },
      fontFamily: {
        sans: ['Inter', 'system-ui', 'sans-serif'],
      },
    },
  },
  plugins: [],
}
```

---

## 🚀 Uruchomienie

### Development Mode

```bash
# Start serwera deweloperskiego
npm run dev

# Otwórz w przeglądarce
# Domyślnie: http://localhost:5173
```

### Production Build

```bash
# Zbuduj wersję produkcyjną
npm run build

# Podgląd buildu lokalnie
npm run preview

# Analiza rozmiaru bundle
npm run build -- --analyze
```

---

## 📁 Struktura Projektu

```
HedenCargoWeb-Web/
├── 📄 public/                  # Pliki statyczne
│   ├── favicon.ico            # Favicon
│   ├── logo.svg               # Logo
│   └── manifest.json          # PWA manifest
├── 📄 src/
│   ├── main.jsx                # Entry point
│   ├── App.jsx                 # Root component
│   ├── components/             # Reusable components
│   │   ├── ui/                # UI components
│   │   ├── layout/            # Layout components
│   │   └── sections/          # Page sections
│   ├── pages/                  # Page components
│   ├── assets/                 # Static assets
│   │   ├── images/            # Images
│   │   ├── icons/             # Icons
│   │   └── styles/            # CSS files
│   ├── hooks/                  # Custom hooks
│   ├── utils/                  # Utility functions
│   └── data/                   # Static data
├── 📄 index.html               # HTML template
├── 📄 package.json            # Dependencies
├── 📄 vite.config.js           # Vite config
├── 📄 tailwind.config.js       # Tailwind config
└── 📄 .env.local               # Environment variables
```

---

## 🎨 Praca z Components

### Tworzenie nowego komponentu

```jsx
// src/components/sections/HeroSection.jsx
import React from 'react';
import { Button } from '../ui/Button';

export const HeroSection = () => {
  return (
    <section className="relative bg-gradient-to-r from-blue-600 to-blue-800">
      <div className="container mx-auto px-6 py-24">
        <h1 className="text-5xl font-bold text-white mb-6">
          HEDEN Cargo Sp. z o.o.
        </h1>
        <Button variant="primary" size="lg">
          Złóż zlecenie
        </Button>
      </div>
    </section>
  );
};
```

### Używanie komponentu

```jsx
// src/pages/Home.jsx
import { HeroSection } from '../components/sections/HeroSection';

export const Home = () => {
  return (
    <main>
      <HeroSection />
      {/* inne sekcje */}
    </main>
  );
};
```

---

## 🎯 Best Practices

### 1. Nazewnictwo plików
- Używaj PascalCase dla komponentów: `HeroSection.jsx`
- Używaj camelCase dla utilities: `formatDate.js`
- Używaj kebab-case dla assets: `hero-bg.jpg`

### 2. Struktura komponentów
```jsx
// Importy na górze
import React from 'react';
import { Button } from '../ui/Button';

// Props interface (TypeScript)
// lub komentarz (JavaScript)
/**
 * @param {Object} props
 * @param {string} props.title
 * @param {Function} props.onClick
 */

// Komponent
export const MyComponent = ({ title, onClick }) => {
  return (
    <div className="component-wrapper">
      <h2>{title}</h2>
      <Button onClick={onClick}>Click me</Button>
    </div>
  );
};

// Export na dole
export default MyComponent;
```

### 3. TailwindCSS Tips
```jsx
// ✅ Dobre - używanie klas
<div className="flex items-center justify-between p-4 bg-white rounded-lg shadow-md">

// ❌ Złe - inline styles
<div style={{ display: 'flex', padding: '16px' }}>

// ✅ Dobre - custom colors w config
<div className="bg-primary-500 text-white">

// ❌ Złe - arbitrary values
<div className="bg-[#3b82f6]">
```

---

## 🔧 Troubleshooting

### Common Issues

#### 1. Vite dev server nie startuje
```bash
# Sprawdź port
netstat -ano | findstr :5173

# Zmień port
npm run dev -- --port 3000
```

#### 2. TailwindCSS nie działa
```bash
# Przebuduj CSS
npm run build:css

# Sprawdź konfigurację
npx tailwindcss --help
```

#### 3. Import error
```bash
# Sprawdź ścieżki
# Używaj relative imports
import Button from '../components/ui/Button'; // ✅
import Button from '@/components/ui/Button';  // ❌ (bez path alias)
```

---

## 🚀 Deployment

### Vercel (zalecane)

```bash
# Zainstaluj Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

### Netlify

```bash
# Build
npm run build

# Upload folder /dist do Netlify
```

### Docker

```dockerfile
FROM node:18-alpine

WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production

COPY . .
RUN npm run build

FROM nginx:alpine
COPY --from=0 /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

---

## 📞 Pomoc

### Resources
- [Vite Documentation](https://vitejs.dev/)
- [TailwindCSS Documentation](https://tailwindcss.com/)
- [React Documentation](https://reactjs.org/)

### Support
- 🐙 [GitHub Issues](https://github.com/WilkorPLYT/HedenCargoWeb-Web/issues)
- 💬 [Discord](https://discord.gg/hedencargo)
- 📧 [biuro@hedencargo.pl](mailto:biuro@hedencargo.pl)

---

*Ostatnia aktualizacja: 6 marca 2026*
