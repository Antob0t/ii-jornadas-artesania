#  II Jornadas de Artesanía - Proyecto Frontend

Este proyecto es la resolución de la Práctica de Evaluación Continua (PEC 2) de Maquetación Web. Consiste en el desarrollo de un sitio web completo, responsive y accesible para un evento ficticio de artesanía en Alcalá del Júcar.

##  Características Principales y Tecnologías

El proyecto ha sido construido desde cero (Mobile First) sin utilizar plantillas prefabricadas, implementando las siguientes tecnologías y metodologías:

*   **HTML5 Semántico:** Estructura accesible y lógica de los contenidos.
*   **SCSS / Sass:** Uso de variables, anidamiento, mixins y parciales.
*   **Metodología BEM:** Arquitectura de clases (Bloque, Elemento, Modificador) para un código CSS escalable y libre de colisiones.
*   **CSS Grid Avanzado:** Creación de un póster editorial con solapamiento de elementos en un grid de 12 columnas.
*   **Flexbox Flex-Wrap:** Sistema de retículas fluidas sin dependencias de columnas de frameworks.
*   **Bootstrap 5:** Integración selectiva de componentes (`Navbar`, `Cards`, `Forms`, `Buttons`, `Breadcrumbles`), sobrescribiendo sus estilos por defecto mediante especificidad CSS.
*   **Empaquetador:** Uso de Parcel para compilar SCSS a CSS y empaquetar el proyecto.

## Requisitos de CSS Moderno Implementados

Para cumplir con los requisitos avanzados de la práctica, se han aplicado las siguientes especificaciones recientes de CSS:

*   **Container Queries (`@container` / `cqw`):** Tipografía de títulos que responde al tamaño de su propio contenedor en lugar de la ventana del navegador.
*   **Unidades de Viewport Dinámicas (`dvh`):** Asegura que la página de contacto ocupe siempre el 100% de la pantalla real en dispositivos móviles.
*   **Nuevos espacios de color (`oklch`):** Definición de colores de fondo y estados interactivos usando el espacio de color perceptualmente uniforme OKLCH.
*   **Selectores y Pseudoclases funcionales:**
    *   `:is()`: Agrupación de selectores para aplicar estilos comunes sin repetir código (Principio DRY).
    *   `:has()`: Lógica condicional parental para aplicar estilos a un contenedor de texto si este incluye un enlace en su interior (Call to Action dinámico).

## Estructura del Proyecto

El sitio web consta de las siguientes 4 páginas:

1.  **`index.html` (Home):** Presenta un diseño de póster tipo revista editorial usando CSS Grid para superponer la imagen, el título y las fechas.
2.  **`speakers.html` (Ponentes):** Galería de artesanos creada con tarjetas (Cards) de Bootstrap integradas en un sistema de rejilla puramente Flexbox (`flex-grow`, `flex-basis`).
3.  **`article.html` (Artículo):** Página de contenido editorial con efecto *Hero Banner*, blockquotes asimétricos, y listas ordenadas `<ol>` personalizadas con CSS Counters.
4.  **`contact.html` (Contacto):** Formulario de Bootstrap 5 totalmente customizado para encajar con el diseño brutalista, aplicando estados visuales para accesibilidad (`:focus`, `:valid`).

