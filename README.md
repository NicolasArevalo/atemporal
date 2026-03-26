# Atemporal - Preservando el Legado Familiar

**Atemporal** es una plataforma y servicio orientado a inmortalizar las historias, recuerdos y fotografías de las familias para crear tesoros que trascienden generaciones. Este repositorio contiene el código fuente de la *Landing Page* principal del proyecto.

## 🌟 Características Principales

- **Diseño Emocional y Minimalista**: Una interfaz limpia configurada con una paleta cálida (Blanco Hueso, Gris Carbón, Terracota Mate) para evocar calma y respeto.
- **Enfoque "Mobile-First"**: Construido desde cero para ofrecer una experiencia fluida, accesible y perfectamente responsiva en dispositivos móviles.
- **Animaciones Nativas**: Implementación de `IntersectionObserver` y CSS para revelar las secciones suavemente (*fade-in*) conforme el usuario hace scroll hacia abajo.
- **Microinteracciones**: Integración de animaciones sutiles impulsadas por CSS (como una onda de sonido animada puramente con keyframes de Tailwind).
- **Integración con WhatsApp**: Los "Call to Action" están directamente enlazados a la API de WhatsApp, con mensajes preconfigurados dependientes del contexto.

## 🛠 Tecnologías Utilizadas

Este proyecto utiliza el stack moderno y ultrarrápido por excelencia:

- **[Astro](https://astro.build/)**: Framework web diseñado principalmente para la velocidad y sitios estáticos.
- **[Tailwind CSS v4](https://tailwindcss.com/)**: Framework de CSS basado en utilidades, integrado de forma nativa en Astro para configurar los tokens de diseño y estilado de componentes.
- **HTML/CSS/Vanilla JS**: Construcción nativa sin pesadas librerías de UI externas para mantener el bundle final en su mínima expresión.
- **Fuentes**: [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) (elegancia serif para encabezados) e [Inter](https://fonts.google.com/specimen/Inter) (claridad sans-serif para cuerpos).

## 🚀 Instalación y Desarrollo Local

Sigue estos pasos para correr el proyecto en tu entorno local:

1. **Clona o descarga este repositorio**
2. **Instala las dependencias**:
   ```bash
   npm install
   ```
3. **Inicia el servidor de desarrollo**:
   ```bash
   npm run dev
   ```
4. **Disfruta del proyecto**:  
   Abre tu navegador en [http://localhost:4321/](http://localhost:4321/)

## 📂 Estructura del Proyecto

Las secciones más importantes del repositorio son:

- `src/layouts/Layout.astro`: Define el cascarón HTML general y carga las fuentes.
- `src/pages/index.astro`: Ensambla la página principal combinando los distintos componentes.
- `src/styles/global.css`: Aquí se declaran nuestros tokens de Tailwind variables y la directiva `@theme`.
- `src/components/`:
  - `Hero.astro`: Encabezado asimétrico con la promesa de valor y el video inyectado.
  - `HowItWorks.astro`: Explicación del proceso (Entrevista, Magia, Legado).
  - `LegacyGrid.astro`: Cuadrícula fotográfica que interactúa en hover activando o desactivando filtros grises.
  - `AudioPreview.astro`: UI flotante minimalista que simula ser un reproductor de audio.
  - `PricingCards.astro`: Tarjetas informativas orientadas a generar la conversión mediante WhatsApp.
