# 👨‍💻 Daniel Diaz - Portfolio (React Edition)

**Versión moderna y basada en componentes de mi sitio web personal.**

Este repositorio contiene la refactorización completa de mi portafolio profesional, migrado de una arquitectura estática (HTML/jQuery) a una **Single Page Application (SPA)** construida con **React**. El proyecto demuestra habilidades avanzadas en frontend, gestión de estado y renderizado de gráficos interactivos.

![Portfolio Preview](./public/preview.png)


## 🚀 De HTML a React: La Evolución

El objetivo de este proyecto fue transformar un sitio web estático en una aplicación modular y escalable.

| Feature | Versión Legacy (HTML) | Versión Actual (React) |
| :--- | :--- | :--- |
| **Arquitectura** | Monolito HTML5 + Scripts Globales | Componentes Funcionales y Hooks |
| **Estado (Tema/Idioma)** | Manipulación directa del DOM | React Context API |
| **Animaciones** | Scripts Vanilla JS imperativos | `useEffect` y Refs para Canvas/WebGL |
| **Estilos** | Múltiples archivos CSS (`color-1.css`, etc.) | CSS Modules / Styled Components |
| **Contenido** | Hardcoded en HTML | Datos dinámicos (JSON/Arrays) |

## 📋 Características Técnicas

### 🎨 UI/UX Dinámica
* **Theming System:** Sistema de temas configurables que permite al usuario cambiar la paleta de colores en tiempo real.
* **Internacionalización (i18n):** Soporte multi-idioma (Español/Inglés) gestionado mediante contextos, cargando las traducciones desde archivos JSON estructurados.
* **Diseño Responsivo:** Layout fluido que se adapta a móviles, tablets y escritorio.

### 🧪 WebGL & Interactividad
* **Efecto "Smoke Simulation":** Implementación de una simulación de fluidos en un `HTML5 Canvas`. La lógica original en JavaScript puro se encapsuló dentro de un componente React (`<SmokeBackground />`), optimizando los *event listeners* y el ciclo de vida del renderizado para evitar fugas de memoria.

### 🧩 Estructura de Componentes
El proyecto sigue una arquitectura atómica organizada:

```bash
