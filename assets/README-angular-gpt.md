# 🤖 Angular GPT — Chat con Inteligencia Artificial

<div align="center">

**Aplicación web en Angular integrada con la API de OpenAI. Interfaz de chat conversacional con soporte de Markdown.**

[![Angular](https://img.shields.io/badge/Angular-17-DD0031?style=flat-square&logo=angular&logoColor=white)](https://angular.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![OpenAI](https://img.shields.io/badge/OpenAI_API-GPT--4-412991?style=flat-square&logo=openai&logoColor=white)](https://platform.openai.com)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

</div>

---

## 🎯 Descripción

**Angular GPT** es una interfaz de chat conversacional que conecta Angular directamente con la API de OpenAI. Permite enviar prompts, recibir respuestas de GPT y visualizarlas con renderizado de Markdown — ideal para experimentar con IA desde el frontend.

## ✨ Funcionalidades

- 💬 **Chat en tiempo real** con modelos GPT de OpenAI
- 📝 **Renderizado de Markdown** — código, listas, negritas y más en las respuestas
- 📜 **Historial de conversación** — contexto acumulativo en cada sesión
- 🎛️ **Configuración** — selector de modelo (GPT-3.5 / GPT-4) y temperatura
- 📋 **Copiar respuesta** al portapapeles con un clic
- 🌙 **Tema claro/oscuro**

## 🛠️ Stack tecnológico

| Tecnología | Versión | Uso |
|---|---|---|
| Angular | 17 | Framework principal |
| TypeScript | 5 | Tipado estático |
| ngx-markdown | 17 | Renderizado de Markdown |
| OpenAI SDK | — | Integración con API |
| CSS | — | Estilos propios |

## 🚀 Instalación

### Prerrequisitos

- Node.js 20+
- Angular CLI 17+
- API Key de [OpenAI](https://platform.openai.com/api-keys)

```bash
# 1. Clonar el repositorio
git clone https://github.com/DanielHR3/angular-gpt.git
cd angular-gpt

# 2. Instalar dependencias (incluye ngx-markdown)
npm install
npm install ngx-markdown@17.2.1 --save

# 3. Configurar la API Key
# Edita src/environments/environment.ts:
# openAiKey: 'TU_API_KEY_AQUI'

# 4. Iniciar servidor de desarrollo
ng serve
# → http://localhost:4200
```

### Variables de entorno

```typescript
// src/environments/environment.ts
export const environment = {
  production: false,
  openAiKey: 'sk-...'   // Tu API Key de OpenAI
};
```

> ⚠️ **Nunca subas tu API Key a GitHub.** Agrega `environment.ts` al `.gitignore` o usa variables de entorno del sistema en producción.

## 🗂️ Estructura

```
src/app/
├── components/
│   ├── chat/            # Interfaz principal del chat
│   │   ├── chat.component.ts
│   │   └── chat.component.html
│   ├── message/         # Burbuja de mensaje individual
│   └── settings/        # Panel de configuración
├── services/
│   └── openai.service.ts  # Llamadas a la API de OpenAI
└── models/
    └── message.model.ts   # Tipado de mensajes
```

## 🔐 Seguridad

- ⚠️ Este proyecto consume la API de OpenAI directamente desde el frontend (solo para fines de desarrollo/demo)
- Para producción, se recomienda un backend intermediario (NestJS/Express) que proteja la API Key

## 📄 Licencia

MIT © [Daniel Hernández Rubio](https://danielhr3.github.io)
