# 🍸 Elixir - Premium Cocktail Landing Page

A stunning, interactive landing page showcasing the art of cocktail mixology, powered by cutting-edge animations and modern web technologies.

## ✨ Features

### 🎬 Advanced GSAP Animations

This landing page demonstrates the incredible power of **GSAP (GreenSock Animation Platform)** with:

- **Smooth Scroll Animations**: Dynamic parallax effects triggered by scroll position
- **Text Animations**: Character-by-character and line-by-line reveals using SplitText
- **Hero Section**: Eye-catching entrance animations with staggered timing
- **Interactive Elements**: Scroll-triggered animations throughout the page
- **Parallax Leaves**: Decorative cocktail leaf elements that animate parallactically

### 🍹 Cocktail-Focused Content

The landing page features multiple sections dedicated to cocktails:

- **Hero Section**: Captivating introduction to the Elixir experience
- **Cocktails Section**: Showcase of popular and trending cocktail selections
- **Menu Section**: Detailed cocktail menu with descriptions
- **About Section**: Story behind the cocktail bar and philosophy
- **Art Section**: Visual gallery of cocktail presentations
- **Contact Section**: Easy way to get in touch

## 🛠️ Tech Stack

- **React 19** - Modern UI library with optimal performance
- **Vite 7** - Lightning-fast build tool with HMR support
- **GSAP 3** - Professional animation library with ScrollTrigger plugin
- **Tailwind CSS 4** - Utility-first CSS framework for rapid styling
- **React Responsive** - Media queries for responsive design

## 📦 Key Dependencies

```json
{
  "gsap": "^3.13.0",
  "@gsap/react": "^2.1.2",
  "react": "^19.1.1",
  "tailwindcss": "^4.1.16",
  "react-responsive": "^10.0.1",
  "vite": "^7.1.7"
}
```

## 🚀 Getting Started

### Installation

```bash
npm install
```

### Development Server

```bash
npm run dev
```

This will start the Vite development server with HMR enabled for instant updates.

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## 📁 Project Structure

```
elixir/
├── src/
│   ├── components/
│   │   ├── Navbar.jsx        - Navigation bar
│   │   ├── Hero.jsx          - Hero section with animations
│   │   ├── Cocktails.jsx     - Popular cocktails showcase
│   │   ├── Menu.jsx          - Full cocktail menu
│   │   ├── About.jsx         - About section
│   │   ├── Art.jsx           - Art/gallery section
│   │   └── Contact.jsx       - Contact information
│   ├── App.jsx               - Main app component with GSAP plugins
│   ├── main.jsx              - React entry point
│   └── index.css             - Global styles
├── constants/
│   └── index.js              - Mock data and constants
├── public/
│   ├── images/               - Image assets
│   ├── fonts/                - Font files
│   └── videos/               - Video assets
├── package.json              - Dependencies
├── vite.config.js            - Vite configuration
└── tailwind.config.js        - Tailwind CSS configuration
```

## 🎨 Animation Highlights

### GSAP Features Used

- **ScrollTrigger**: Reactive animations based on scroll position
- **SplitText**: Advanced text animations with character/line control
- **Timelines**: Coordinated multi-element animations
- **Easing Functions**: Professional animation curves (ease.out, expo, etc.)
- **Staggering**: Sequential animations for visual impact

### Example: Hero Text Animation

```jsx
const heroSplit = new SplitText(".title", { type: "chars, words" });
gsap.from(heroSplit.chars, {
  yPercent: 100,
  duration: 1.8,
  ease: "expo.out",
  stagger: 0.06,
});
```

### Example: Scroll-Triggered Parallax

```jsx
const parallaxTimeline = gsap.timeline({
  scrollTrigger: {
    trigger: "#cocktails",
    start: "top 30%",
    end: "bottom 80%",
    scrub: true,
  },
});
```

## 🎯 Why Choose Elixir?

- **Performance**: Optimized animations that don't compromise performance
- **Modern Design**: Contemporary UI with smooth, professional animations
- **Responsive**: Fully responsive design that works on all devices
- **Developer Experience**: Clean code structure and easy to customize
- **Professional**: Production-ready with best practices

## 📝 Linting

```bash
npm run lint
```

Uses ESLint with React and React Hooks plugins for code quality.

## 📄 License

This project is open source and available under the MIT License.
