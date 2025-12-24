# Mythos Website

A modern, responsive single-page website for **Mythos**. Built with vanilla JavaScript, modern CSS, and best practices for accessibility and performance.

## 🌐 Live Preview

**[View Live Site](https://ammar-taha.github.io/mythos-website/)**

## 📋 Table of Contents

- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Development](#development)
- [Build](#build)
- [Architecture](#architecture)
- [Key Features](#key-features)
- [Accessibility](#accessibility)
- [Browser Support](#browser-support)
- [Acknowledgments](#acknowledgments)

## 🛠 Tech Stack

- **HTML5**: Semantic markup with accessibility in mind
- **CSS3**:
  - CSS Custom Properties (CSS Variables)
  - CSS Layers for organized styling
  - Modern CSS Reset
  - Responsive design with clamp() and media queries
- **JavaScript (ES6+)**:
  - Vanilla JavaScript (no frameworks)
  - ES6 Modules
  - Event-driven architecture
- **Build Tools**:
  - [Vite](https://vitejs.dev/) - Fast build tool and dev server
  - [Normalize.css](https://necolas.github.io/normalize.css/) - CSS normalization

## 📁 Project Structure

```
mythos-website/
├── index.html              # Main HTML file
├── package.json            # Dependencies and scripts
├── vite.config.js          # Vite configuration
├── public/                 # Static assets (favicons, manifests)
│   ├── favicon.ico
│   ├── favicon.svg
│   └── ...
├── src/
│   ├── index.css           # Main CSS entry point
│   ├── style.css           # Application styles
│   ├── modern-css-reset.css # CSS reset
│   ├── main.js             # JavaScript functionality
│   └── assets/             # Images, fonts, icons
│       ├── fonts/          # Custom web fonts (Source Sans 3)
│       ├── blog/           # Blog post images
│       ├── social/         # Social media icons
│       └── ...             # Other assets
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:

```bash
git clone https://github.com/ammar-taha/mythos-website.git
cd mythos-website
```

2. Install dependencies:

```bash
npm install
```

## 💻 Development

Start the development server:

```bash
npm run dev
```

The site will be available at `http://localhost:5173` (or the next available port).

### Development Features

- Hot Module Replacement (HMR) for instant updates
- Fast refresh for CSS and JavaScript changes
- Source maps for debugging

## 🏗 Build

Build for production:

```bash
npm run build
```

The production-ready files will be output to the `dist/` directory.

Preview the production build:

```bash
npm run preview
```

## 🏛 Architecture

### CSS Architecture

The project uses **CSS Layers** for organized styling:

1. **Normalize Layer**: Browser normalization via normalize.css
2. **Reset Layer**: Modern CSS reset for consistent base styles
3. **App Layer**: Application-specific styles

#### CSS Custom Properties

The project uses CSS variables for theming and maintainability:

- **Color System**: Centralized color definitions (purple, teal, gray, etc.)
- **Typography**: Responsive font sizes using `clamp()` and CSS variables
- **Spacing**: Consistent spacing system
- **Breakpoints**: Media query breakpoints defined as custom properties

### JavaScript Architecture

- **Modular**: ES6 modules for code organization
- **Event-Driven**: Event listeners for user interactions
- **Responsive**: Breakpoint detection for mobile menu behavior
- **Accessible**: ARIA attributes and keyboard navigation support

### Responsive Design

- **Mobile-First**: Base styles target mobile devices
- **Breakpoints**:
  - Mobile: `< 600px` (37.5rem)
  - Tablet/Desktop: `≥ 600px`
- **Fluid Typography**: Uses `clamp()` for responsive text sizing
- **Flexible Layouts**: CSS Grid and Flexbox for responsive layouts

## 🎯 Key Features

### Mobile Navigation

- Hamburger menu for mobile devices
- Smooth slide-in animation
- Body scroll lock when menu is open
- Keyboard accessible (ESC to close, focus management)
- ARIA attributes for screen readers

### Performance Optimizations

- Optimized images with multiple resolutions (2x, 3x)
- Web font optimization with `font-display: swap`
- Minimal JavaScript footprint
- CSS layer organization for efficient rendering

### Accessibility

- Semantic HTML5 elements
- ARIA labels and roles
- Skip to main content link
- Keyboard navigation support
- Focus management
- Alt text for all images
- Proper heading hierarchy

## ♿ Accessibility

This project follows WCAG guidelines and best practices:

- ✅ Semantic HTML structure
- ✅ ARIA labels and roles
- ✅ Keyboard navigation
- ✅ Focus indicators
- ✅ Screen reader support
- ✅ Skip navigation link
- ✅ Proper color contrast
- ✅ Alt text for images

## 🙏 Acknowledgments

This project was developed as part of the **Build a Responsive Website** course by [Jess Chan](https://coder-coder.com/responsive/). The course provides comprehensive guidance on building responsive websites from design files using HTML, CSS, and JavaScript. [Find out more about the course here](https://coder-coder.com/responsive/).
