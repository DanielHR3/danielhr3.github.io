# 🌙 Luna y Sol — Diseño Web Creativo con Angular

<div align="center">

**Proyecto de diseño web minimalista con animaciones fluidas y paleta dual Luna/Sol. Showcase de CSS avanzado y Angular.**

[![Angular](https://img.shields.io/badge/Angular-19-DD0031?style=flat-square&logo=angular&logoColor=white)](https://angular.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![CSS3](https://img.shields.io/badge/CSS3-Animations-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/es/docs/Web/CSS)

</div>

---

## 🎨 Concepto

**Luna y Sol** explora la dualidad visual entre dos filosofías estéticas opuestas:

- 🌙 **Luna** — paleta fría, oscura, con movimientos suaves y transiciones etéreas
- ☀️ **Sol** — paleta cálida, luminosa, con energía y contraste vibrante

El resultado es un proyecto que demuestra el dominio de **animaciones CSS avanzadas**, **layouts creativos** y **design system** basado en tokens.

## ✨ Técnicas destacadas

- **Custom CSS animations** con `@keyframes` y `animation-timing-function` personalizados
- **CSS Grid y Flexbox** en layouts complejos y asimétricos
- **Variables CSS** (`--tokens`) para sistema de diseño dual (luz/oscuridad)
- **Intersection Observer API** para animaciones on-scroll sin librerías externas
- **Transiciones de tema** suaves con `transition: all` en el root

## 🛠️ Stack

- **Angular 19** — Componentes y enrutamiento
- **TypeScript** — Lógica de interacción
- **CSS puro** — 44% del proyecto, animaciones escritas a mano

## 🚀 Instalación y uso

### Prerrequisitos

- Node.js 20+
- Angular CLI 19

```bash
# Instalar Angular CLI (si no está instalado)
npm install -g @angular/cli

# Clonar el repositorio
git clone https://github.com/DanielHR3/luna-y-sol.git
cd luna-y-sol

# Instalar dependencias
npm install

# Iniciar servidor de desarrollo
ng serve
# → http://localhost:4200
```

### Otros comandos

```bash
ng build          # Build de producción
ng test           # Tests unitarios con Karma
ng lint           # Linting con ESLint
```

## 🗂️ Estructura

```
src/
├── app/
│   ├── components/
│   │   ├── hero/         # Sección principal con animación dual
│   │   ├── theme-toggle/ # Toggle Luna/Sol
│   │   └── sections/     # Secciones del contenido
│   └── styles/
│       ├── luna.css      # Variables y animaciones del tema Luna
│       └── sol.css       # Variables y animaciones del tema Sol
└── global_styles.css
```

## 🎯 Objetivo del proyecto

Proyecto creado como **showcase de habilidades CSS y diseño** para demostrar:
- Control avanzado de animaciones sin dependencias externas
- Buen ojo para la estética y composición visual
- Capacidad de construir design systems temáticos

## 📄 Licencia

MIT © [Daniel Hernández Rubio](https://danielhr3.github.io)
