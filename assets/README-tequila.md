# 🥃 Tequilera — Sitio Web Empresarial

<div align="center">

**Sitio web corporativo para una empresa tequilera con catálogo de productos, galería y formulario de contacto con backend PHP.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/es/docs/Web/CSS)
[![PHP](https://img.shields.io/badge/PHP-8-777BB4?style=flat-square&logo=php&logoColor=white)](https://php.net)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)](https://mysql.com)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)

</div>

---

## 🎯 Descripción

**Tequilera** es un sitio web de tipo corporativo desarrollado para una empresa ficticia del sector de bebidas artesanales. El proyecto simula un entorno real de negocio con páginas de inicio, catálogo de productos y sistema de contacto funcional con almacenamiento en base de datos.

## 📄 Páginas

| Página | Descripción |
|---|---|
| `index.html` | Home — Hero, historia de la marca, diferenciales |
| `productos.html` | Catálogo de productos con galería de imágenes |
| `contacto.html` | Formulario de contacto con validación |
| `contacto.php` | Backend PHP — procesa y guarda el formulario en MySQL |

## ✨ Características técnicas

- 🎨 **Diseño responsive** — adaptado a móvil, tablet y escritorio
- 📧 **Formulario funcional** — PHP guarda los mensajes en base de datos MySQL
- 🖼️ **Galería de productos** — presentación visual de la cartera de tequilas
- 🎯 **Banner y secciones diferenciales** — diseño por secciones con assets propios
- ✅ **Validación del lado del cliente** con JavaScript puro
- 🔁 **Reset CSS propio** para consistencia cross-browser

## 🛠️ Stack tecnológico

- **HTML5** — Estructura semántica de cada página
- **CSS3** — Diseño custom: `style.css`, `style-home.css`, `reset.css`
- **JavaScript** — Validación de formulario y comportamiento dinámico
- **PHP 8** — Procesamiento del formulario de contacto
- **MySQL** — Almacenamiento de mensajes (schema en `tequila_contacto.sql`)

## 🚀 Instalación y uso local

### Prerrequisitos

- Servidor local con PHP: [XAMPP](https://apachefriends.org), [Laragon](https://laragon.org) o [WAMP](https://wampserver.com)
- MySQL para la base de datos del formulario

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/DanielHR3/Tequila.git

# 2. Copiar la carpeta a la raíz de tu servidor local
# XAMPP: C:/xampp/htdocs/tequilera/
# Laragon: C:/laragon/www/tequilera/

# 3. Importar la base de datos
# Abre phpMyAdmin → Importar → selecciona tequila_contacto.sql

# 4. Abrir en el navegador
# → http://localhost/tequilera/
```

### Configurar conexión a la base de datos

Edita la conexión en `contacto.php`:

```php
$conn = new mysqli('localhost', 'root', '', 'tequila_contacto');
```

## 🗂️ Estructura del proyecto

```
tequilera/
├── index.html          # Página de inicio
├── productos.html      # Catálogo de productos
├── contacto.html       # Formulario de contacto
├── contacto.php        # Backend del formulario
├── reset.css           # Reset de estilos
├── style.css           # Estilos globales
├── style-home.css      # Estilos específicos del home
├── tequila_contacto.sql # Schema de la base de datos
├── back.jpg            # Imagen de fondo
├── banner/             # Imágenes del banner
├── diferenciales/      # Imágenes de sección diferenciales
└── imagenes/           # Galería de productos
```

## 📄 Licencia

MIT © [Daniel Hernández Rubio](https://danielhr3.github.io)
