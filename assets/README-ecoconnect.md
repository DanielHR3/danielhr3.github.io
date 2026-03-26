# 🌱 EcoConnect — Reportes de Impacto Sostenible con IA

<div align="center">

**Plataforma web que genera reportes automáticos de impacto sostenible para PYMES, potenciada por inteligencia artificial.**

[![Angular](https://img.shields.io/badge/Angular-19-DD0031?style=flat-square&logo=angular&logoColor=white)](https://angular.dev)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![NestJS](https://img.shields.io/badge/NestJS-10-E0234E?style=flat-square&logo=nestjs&logoColor=white)](https://nestjs.com)
[![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://mysql.com)
[![OpenAI](https://img.shields.io/badge/OpenAI_API-GPT--4-412991?style=flat-square&logo=openai&logoColor=white)](https://platform.openai.com)

</div>

---

## 🎯 Propósito

Muchas PYMES realizan prácticas sostenibles pero no saben cómo comunicarlas. **EcoConnect** resuelve esto generando reportes de impacto ambiental automáticos, listos para compartir con clientes, inversores o en redes sociales.

## ✨ Funcionalidades

- 📊 **Dashboard de impacto** — visualización de métricas sostenibles (CO₂ ahorrado, residuos reducidos, energía renovable)
- 🤖 **Generación con IA** — describe tus prácticas y GPT-4 genera un reporte profesional en segundos
- 📄 **Exportar reportes** — descarga en PDF o comparte el enlace directo
- 🏢 **Perfil de empresa** — datos, logo, sector y métricas históricas
- 🔐 **Autenticación** — registro e inicio de sesión seguros

## 🛠️ Stack tecnológico

### Frontend
| Tecnología | Versión | Uso |
|---|---|---|
| Angular | 19 | Framework SPA |
| Tailwind CSS | 3 | Estilos |
| TypeScript | 5 | Tipado estático |

### Backend
| Tecnología | Versión | Uso |
|---|---|---|
| NestJS | 10 | API REST |
| MySQL | 8 | Base de datos |
| OpenAI API | GPT-4 | Generación de contenido |
| JWT | — | Autenticación |

## 🚀 Instalación

### Prerrequisitos
- Node.js 20+
- MySQL 8+
- API Key de OpenAI

### Frontend

```bash
git clone https://github.com/DanielHR3/ecoconnect-frontend.git
cd ecoconnect-frontend
npm install
ng serve
# → http://localhost:4200
```

### Variables de entorno

Crea un archivo `environment.ts` en `src/environments/`:

```typescript
export const environment = {
  production: false,
  apiUrl: 'http://localhost:3000',
  openAiKey: 'TU_API_KEY_AQUI'
};
```

## 🗂️ Arquitectura

```
ecoconnect-frontend/
├── src/
│   ├── app/
│   │   ├── core/            # Guards, interceptors, servicios base
│   │   ├── features/
│   │   │   ├── dashboard/   # Panel principal de métricas
│   │   │   ├── reports/     # Generación y visualización de reportes
│   │   │   └── profile/     # Perfil de empresa
│   │   └── shared/          # Componentes y pipes reutilizables
│   └── environments/
└── ...
```

## 📄 Licencia

MIT © [Daniel Hernández Rubio](https://danielhr3.github.io)
