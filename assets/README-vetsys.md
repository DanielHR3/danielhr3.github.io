# 🐾 VetSys — Sistema de Gestión Veterinaria

<div align="center">

**Aplicación de escritorio completa para la gestión eficiente de clínicas veterinarias.**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![SQLite](https://img.shields.io/badge/SQLite-3-003B57?style=flat-square&logo=sqlite&logoColor=white)](https://sqlite.org)
[![Tkinter](https://img.shields.io/badge/Tkinter-GUI-FF6B35?style=flat-square&logo=python&logoColor=white)](https://docs.python.org/3/library/tkinter.html)
[![FPDF](https://img.shields.io/badge/FPDF2-PDF-red?style=flat-square)](https://py-pdf.github.io/fpdf2)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

</div>

---

## 🎯 Descripción

**VetSys** es una solución integral para clínicas veterinarias que centraliza la gestión de pacientes, citas, historial médico, inventario y más — todo desde una interfaz de escritorio intuitiva sin necesidad de conexión a internet.

## ✨ Funcionalidades

| Módulo | Descripción |
|---|---|
| 🐶 **Pacientes** | Registro de mascotas con especie, raza, propietario e historial |
| 📅 **Citas** | Agenda de citas con vista diaria y semanal |
| 🏥 **Historial médico** | Consultas, diagnósticos y tratamientos por paciente |
| 💊 **Recetas** | Generación de recetas médicas con firma y datos del veterinario |
| 📦 **Inventario** | Control de medicamentos, alimentos y stock con alertas de mínimos |
| 👥 **Usuarios y roles** | Acceso diferenciado: admin, veterinario, recepcionista |
| 📄 **Reportes PDF** | Exportación de historial, recetas e inventario a PDF |
| 💾 **Backups** | Copias de seguridad automáticas de la base de datos |

## 🛠️ Stack tecnológico

- **Python 3.10+** — Lógica de negocio y controladores
- **SQLite 3** — Base de datos local embebida
- **Tkinter** — Interfaz gráfica de usuario (GUI)
- **FPDF2** — Generación de documentos PDF
- **Pillow** — Manejo de imágenes (logos, fotos de mascotas)

## 🚀 Instalación

### Prerrequisitos

- Python 3.10 o superior
- pip (gestor de paquetes de Python)

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/DanielHR3/vetsys.git
cd vetsys

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Ejecutar la aplicación
python main.py
```

### Acceso inicial por defecto

```
Usuario:    admin
Contraseña: admin
```

> ⚠️ **Recomendación**: cambia la contraseña del administrador al iniciar sesión por primera vez en Configuración > Usuarios.

## 🗂️ Arquitectura

El proyecto sigue el patrón **MVC (Modelo-Vista-Controlador)**:

```
vetsys/
├── main.py              # Punto de entrada
├── models/              # Modelos de datos y operaciones con SQLite
│   ├── paciente.py
│   ├── cita.py
│   ├── inventario.py
│   └── usuario.py
├── views/               # Ventanas y formularios Tkinter
│   ├── dashboard.py
│   ├── pacientes_view.py
│   └── ...
├── controllers/         # Lógica entre modelos y vistas
├── utils/               # Generación de PDF, backups, helpers
└── data/                # Base de datos SQLite (generada automáticamente)
```

## 💡 Casos de uso

- Clínicas veterinarias pequeñas y medianas sin sistema de gestión
- Entornos sin conexión a internet estable
- Consultorios independientes con un solo veterinario

## 📄 Licencia

MIT © [Daniel Hernández Rubio](https://danielhr3.github.io)
