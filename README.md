# Evolve — Fitness & Gym Landing

<p align="center">
  <img src="https://img.shields.io/badge/React-18.2-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-5.0-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Vite-4.3-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Tailwind%20CSS-3.3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
</p>

A modern, responsive single-page fitness and gym landing site. Built with **React 18**, **TypeScript**, **Vite**, and **Tailwind CSS**, with smooth scrolling, scroll-triggered animations, and an accessible contact form.

---

## ✨ Features

| Section | Description |
|--------|-------------|
| **Home** | Hero section with headline, CTA buttons, and sponsor strip (desktop). |
| **Benefits** | Highlights: state-of-the-art facility, community, and certified trainers. |
| **Our Classes** | Horizontal scroll gallery (Weight Training, Yoga, Ab Core, Adventure, Fitness, Training). |
| **Contact** | Validated contact form (name, email, message) with [FormSubmit.co](https://formsubmit.co) integration. |
| **Navigation** | Sticky navbar with active section highlighting and mobile hamburger menu. |
| **UX** | Smooth anchor scrolling, Framer Motion animations, responsive layout. |

---

## 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| UI | React 18 |
| Language | TypeScript 5 |
| Build | Vite 4 |
| Styling | Tailwind CSS 3 |
| Animations | Framer Motion |
| Forms | React Hook Form |
| Icons | Heroicons |
| Smooth scroll | react-anchor-link-smooth-scroll |

---

## 📋 Prerequisites

- **Node.js** 18+ (recommended: [nvm](https://github.com/nvm-sh/nvm) or [fnm](https://github.com/Schniz/fnm))
- **npm** 9+ (or yarn / pnpm)

---

## 🚀 Getting Started

### Clone & install

```bash
git clone <your-repo-url>
cd fitness-application
npm install
```

### Development

```bash
npm run dev
```

Open **http://localhost:5173** in your browser.

### Production build

```bash
npm run build
npm run preview   # optional: serve dist/ locally
```

---

## 📜 Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start Vite dev server with HMR |
| `npm run build` | Type-check and build for production |
| `npm run preview` | Serve the production build locally |
| `npm run lint` | Run ESLint on `src` |

---

## 📁 Project Structure

```
fitness-application/
├── public/
├── src/
│   ├── assets/           # Images and graphics
│   ├── hooks/            # Custom hooks (e.g. useMediaQuery)
│   ├── scenes/           # Page sections
│   │   ├── navbar/
│   │   ├── home/
│   │   ├── benefits/
│   │   ├── ourClasses/
│   │   └── contactUs/
│   ├── shared/           # Shared components and types
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── index.html
├── package.json
├── tailwind.config.js
├── tsconfig.json
└── vite.config.ts
```

Path alias **`@`** maps to **`src/`** (see `vite.config.ts` and `tsconfig.json`).

---

## 🎨 Styling & Best Practices

- **Tailwind**: Custom palette (`primary-*`, `secondary-*`, `gray-*`) and breakpoints (`xs`, `sm`, `md` at 1060px).
- **Typography**: DM Sans (body), Montserrat (headings).
- **Accessibility**: Semantic HTML, focus states, and form labels.
- **State**: Scroll-based active section and optional mobile menu state.

---

## 📬 Contact Form

The contact form posts to **FormSubmit.co**. To use your own endpoint:

1. Open `src/scenes/contactUs/index.tsx`.
2. Update the form `action` URL to your FormSubmit email or API endpoint.

Validation is handled by **React Hook Form** (required fields, email pattern, max lengths).

---

## 📄 License

This project is private. Use and distribution follow the repository license terms.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`.
3. Commit changes: `git commit -m 'Add your feature'`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a Pull Request.
