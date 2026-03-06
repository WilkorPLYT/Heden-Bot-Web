<div align="center">

# 🌐 HEDEN Cargo Web - Platforma Informacyjna

[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18+-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-5+-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3+-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)](https://hedencargo.com)
[![License](https://img.shields.io/badge/License-Closed%20Source-red?style=for-the-badge)](#-licencja)

<br>

### 🚐 Oficjalna strona internetowa firmy HEDEN Cargo Sp. z o.o.

<br>

[🌐 Demo](#-demo-strony) •
[📸 Screenshots](#-screenshots) •
[🛠️ Technologie](#️-technologie) •
[📞 Kontakt](#-kontakt)

<br>

---

</div>

<br>

## 🌐 Demo Strony

### 🏢 Strona Główna

<img src="screenshots/strona-glowna.png" alt="Strona główna HEDEN Cargo" width="800">

<br><br>

### 🚐 Nasza Flota

<img src="screenshots/flota.png" alt="Flota pojazdów HEDEN Cargo" width="800">

<br><br>

### 📋 Panel Zleceń

<img src="screenshots/panel-zlecen.png" alt="Panel zleceń online" width="800">

<br>

---

## 📸 Screenshots

### 🎨 Design Interfejsu

<table>
<tr>
<td>

#### 🏠 Strona Główna
- ✅ Nowoczesny design responsywny
- ✅ Animacje i przejścia CSS
- ✅ Integracja z Discord Widget
- ✅ Sekcja aktualności firmy

</td>
<td>

#### 🚐 Flota Pojazdów
- ✅ Galeria naszej floty
- ✅ Specyfikacje techniczne
- ✅ System śledzenia pojazdów
- ✅ Historia przejazdów

</td>
</tr>
<tr>
<td>

#### 📋 Panel Klienta
- ✅ Składanie zleceń online
- ✅ Tracking przesyłek
- ✅ Historia zleceń
- ✅ System płatności

</td>
<td>

#### 👞 Zespół
- ✅ Prezentacja pracowników
- ✅ Role i uprawnienia
- ✅ System kontaktowy
- ✅ Struktura firmy

</td>
</tr>
</table>

<br>

---

## 🎨 Przykładowe Elementy UI

```html
<!-- Hero Section -->
<section class="hero bg-gradient-to-r from-blue-600 to-blue-800">
  <div class="container mx-auto px-6 py-24">
    <h1 class="text-5xl font-bold text-white mb-6">
      HEDEN Cargo Sp. z o.o.
    </h1>
    <p class="text-xl text-blue-100 mb-8">
      Profesjonalne usługi spedycyjne i transportowe
    </p>
    <button class="bg-white text-blue-600 px-8 py-3 rounded-lg font-semibold hover:bg-blue-50 transition">
      Złóż zlecenie
    </button>
  </div>
</section>

<!-- Fleet Grid -->
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
  <div class="fleet-card bg-white rounded-lg shadow-lg overflow-hidden">
    <img src="/vehicles/volvo-fh16.jpg" alt="Volvo FH16">
    <div class="p-6">
      <h3 class="text-xl font-bold mb-2">Volvo FH16</h3>
      <p class="text-gray-600">Ciężarówka 40t • 2024</p>
    </div>
  </div>
</div>
```

<br>

---

## 🛠️ Technologie

<div align="center">

[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer%20Motion-0085FF?style=for-the-badge&logo=framer&logoColor=white)](https://www.framer.com/motion/)
[![Lucide](https://img.shields.io/badge/Lucide-000000?style=for-the-badge&logo=lucide&logoColor=white)](https://lucide.dev/)

</div>

### Stack Techniczny:

- **Frontend:** React 18 z Vite 5
- **Styling:** TailwindCSS 3 z custom components
- **Animations:** Framer Motion dla płynnych przejść
- **Icons:** Lucide React Icons
- **Deployment:** Vercel/Netlify ready
- **SEO:** Meta tags + Open Graph + Structured Data

<br>

---

## 🚀 Szybki Start

### Wymagania
- Node.js 18+
- npm lub yarn
- Git

<br>

### Instalacja

```bash
# Klonuj repozytorium
git clone https://github.com/WilkorPLYT/HedenCargoWeb-Web.git
cd HedenCargoWeb-Web

# Zainstaluj zależności
npm install

# Uruchom serwer deweloperski
npm run dev

# Zbuduj wersję produkcyjną
npm run build
```

<br>

---

## 📁 Struktura Projektu

```
HedenCargoWeb-Web/
├── 📄 index.html                 # Główny plik HTML
├── 📄 package.json              # Zależności
├── 📄 vite.config.js            # Konfiguracja Vite
├── 📄 tailwind.config.js        # Konfiguracja Tailwind
├── 📄 README.md                 # Ta dokumentacja
├── 📄 .gitignore                # Git ignore
├── 📁 src/
│   ├── main.jsx                # Główny komponent React
│   ├── App.jsx                 # Aplikacja główna
│   ├── components/             # Komponenty UI
│   │   ├── Header.jsx          # Nagłówek
│   │   ├── Footer.jsx          # Stopka
│   │   ├── Hero.jsx            # Sekcja hero
│   │   ├── Fleet.jsx           # Flota pojazdów
│   │   └── Contact.jsx         # Formularz kontaktowy
│   ├── pages/                  # Podstrony
│   │   ├── Home.jsx            # Strona główna
│   │   ├── About.jsx           # O nas
│   │   ├── Services.jsx        # Usługi
│   │   └── Contact.jsx         # Kontakt
│   ├── assets/                 # Zasoby statyczne
│   │   ├── images/             # Zdjęcia
│   │   ├── icons/              # Ikony
│   │   └── css/                # Style CSS
│   └── utils/                  # Funkcje pomocnicze
├── 📁 public/                  # Pliki publiczne
│   ├── favicon.ico             # Favicon
│   ├── manifest.json           # PWA manifest
│   └── robots.txt              # SEO robots
└── 📁 screenshots/             # Screenshots aplikacji
```

<br>

---

## 💼 Dostępne na zamówienie

<div align="center">

### 🌐 Chcesz taką stronę dla swojej firmy?

<br>

| Pakiet | Opis |
|--------|------|
| 🎫 **Basic** | Strona wizytówka + sekcja usług |
| 🚗 **Professional** | Pełna strona + panel klienta + zlecenia |
| 🏢 **Enterprise** | Wsparcie + hosting + utrzymanie |

<br>

---

## 📞 Kontakt

<div align="center">

### Zainteresowany? Napisz do nas!

<br>

| Developer | Discord | GitHub |
|-----------|---------|--------|
| **𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻** | [Wilkor#446740090757316608](https://discord.com/users/446740090757316608) | [@WilkorPLYT](https://github.com/WilkorPLYT) |
| **daniek.** | [daniek.#640502766959329282](https://discord.com/users/640502766959329282) | [@daniekdan](https://github.com/daniekdan) |

<br>

### 📧 Kontakt Biznesowy
- 📧 **Email:** biuro@hedencargo.pl
- 📱 **Telefon:** +48 123 456 789
- 🏢 **Adres:** ul. Transportowa 1, 00-001 Warszawa

</div>

<br>

---

## 📄 Licencja

<div align="center">

🔒 **Closed Source - Wszelkie prawa zastrzeżone**

Ten projekt jest własnością autora. Kod źródłowy nie jest publicznie dostępny.

Nieautoryzowane kopiowanie, modyfikowanie lub dystrybucja jest zabroniona.

Autor: WilkorPLYT & Daniel [Daniek.]
Copyright © 2024-2026 HEDEN Cargo Sp. z o.o.

</div>

<br>

---

<br>

## 👨‍💻 Autorzy

<div align="center">

[![Stworzony przez](https://img.shields.io/badge/Stworzony%20przez-WilkorPLYT%20%26%20daniekdan-blueviolet?style=for-the-badge)](https://github.com/WilkorPLYT)

<br>

Stworzony z ❤️ przez **𝓓𝓻𝓦𝓲𝓵𝓪𝓭𝓸𝓻** & **daniek.** dla **HEDEN Cargo Sp. z o.o.**

<br>

| Developer | Discord | GitHub |
|-----------|---------|--------|
| 𝓓𝓻𝓦𝓲𝓵𝓴𝓸𝓻 | [![Discord](https://img.shields.io/badge/Discord-Wilkor%23446740090757316608-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.com/users/446740090757316608) | [![GitHub](https://img.shields.io/badge/GitHub-WilkorPLYT-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/WilkorPLYT) |
| daniek. | [![Discord](https://img.shields.io/badge/Discord-daniek.%23640502766959329282-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.com/users/640502766959329282) | [![GitHub](https://img.shields.io/badge/GitHub-daniekdan-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/daniekdan) |

<br>

---

<br>

**⭐ Jeśli podoba Ci się ten projekt, zostaw gwiazdkę! ⭐**

</div>

<br>

---

<div align="center">

Made with ❤️ | HEDEN Cargo © 2024-2026

</div>
