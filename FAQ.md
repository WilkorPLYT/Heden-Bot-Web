# ❓ Frequently Asked Questions (FAQ)

## 🚀 Instalacja

### Jak zainstalować projekt?

```bash
git clone https://github.com/WilkorPLYT/HedenCargoWeb-Web.git
cd HedenCargoWeb-Web
npm install
npm run dev
```

### Jakie są wymagania systemowe?

- Node.js 18+
- npm lub yarn
- Nowoczesna przeglądarka internetowa

### Jak zbudować wersję produkcyjną?

```bash
npm run build
# Pliki będą w folderze /dist
```

---

## 🛠️ Konfiguracja

### Jak zmienić kolory strony?

Edytuj `tailwind.config.js`:
```js
theme: {
  extend: {
    colors: {
      primary: '#3B82F6',  // Twój kolor
      secondary: '#10B981' // Twój kolor
    }
  }
}
```

### Jak dodać nowe podstrony?

1. Utwórz komponent w `src/pages/`
2. Dodaj routing w `src/App.jsx`
3. Zaktualizuj nawigację w `src/components/Header.jsx`

### Jak zintegrować z Discord Widget?

Dodaj w `src/components/DiscordWidget.jsx`:
```jsx
<iframe 
  src="https://discord.com/widget?id=YOUR_SERVER_ID&theme=dark"
  width="350" 
  height="500"
  allowtransparency="true" 
  frameborder="0"
/>
```

---

## 🎨 Customizacja

### Jak zmienić logo?

Zamień plik `src/assets/logo.svg` na swoje logo.

### Jak dodać nowe ikony?

Użyj Lucide Icons:
```jsx
import { Truck, Package, Users } from 'lucide-react';
```

### Jak zmienić czcionki?

W `tailwind.config.js`:
```js
theme: {
  extend: {
    fontFamily: {
      sans: ['Inter', 'sans-serif'],
    }
  }
}
```

---

## 📱 Responsywność

### Jak przetestować mobilną wersję?

```bash
# Użyj devtools w przeglądarce
# Lub uruchom na urządzeniu mobilnym
npm run dev -- --host
```

### Jak dostosować breakpointy?

W `tailwind.config.js`:
```js
theme: {
  extend: {
    screens: {
      'xs': '475px',
      '3xl': '1600px',
    }
  }
}
```

---

## 🚀 Deployment

### Jak wdrożyć na Vercel?

```bash
npm install -g vercel
vercel --prod
```

### Jak wdrożyć na Netlify?

1. Push kod na GitHub
2. Połącz Netlify z repozytorium
3. Ustaw build command: `npm run build`
4. Ustaw publish directory: `dist`

---

## 🐛 Troubleshooting

### Strona się nie ładuje

```bash
# Sprawdź Node.js
node --version  # Powinna być 18+

# Zainstaluj zależności
npm install

# Sprawdź port
npm run dev -- --port 3000
```

### Błędy TailwindCSS

```bash
# Przebuduj CSS
npm run build:css

# Sprawdź konfigurację
cat tailwind.config.js
```

### Problemy z obrazami

- Upewnij się że obrazy są w `src/assets/`
- Sprawdź ścieżki w importach
- Użyj odpowiednich formatów (WebP, AVIF)

---

## 📞 Pomoc

| Developer | Discord | GitHub |
|-----------|---------|--------|
| **𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻** | [𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻](https://discord.com/users/446740090757316608) | [@WilkorPLYT](https://github.com/WilkorPLYT) |
| **daniek.** | [daniek.](https://discord.com/users/640502766959329282) | [@daniekdan](https://github.com/daniekdan) |

---

Nie znalazłeś odpowiedzi? Otwórz issue! 💬
