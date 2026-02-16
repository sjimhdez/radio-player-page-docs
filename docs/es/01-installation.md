---
layout: default
title: Instalación
---

# Instalación

Esta página describe los requisitos y los pasos para instalar y activar Radio Player Page.

## Requisitos

- **WordPress** 5.0 o superior  
- **PHP** 5.6 o superior  
- Una **URL de streaming válida** (Icecast, Shoutcast, HLS, DASH o MP3)

Para una mejor experiencia, usad un navegador moderno. Los visualizadores de audio usan la Web Audio API, soportada en las versiones actuales de Chrome, Firefox, Edge y Safari (incluido Safari en iOS 10+).

## Pasos de instalación

1. **Subid el plugin** a la carpeta `wp-content/plugins/`, o instaladlo desde la pantalla **Plugins** (Añadir nuevo → Subir plugin o buscad “Radio Player Page”).

2. **Activad el plugin** desde la pantalla **Plugins** de WordPress.

3. Id a **Ajustes → Radio Player Page Settings**.

4. Para al menos una estación:
   - Introducid la **Streaming URL** (la URL completa de vuestro stream).
   - Seleccionad la **Player Page** (la página de WordPress en la que debe mostrarse el reproductor).
   - Haced clic en **Guardar cambios**.

5. **Abrid la página asignada** en el navegador. El reproductor se carga solo; no hace falta añadir contenido ni shortcode a la página.

## Nota importante

No es necesario configurar nada en la propia página de WordPress. El plugin usa el hook `template_redirect` de WordPress: cuando un visitante solicita una página asignada a una estación, el plugin sirve una página HTML independiente con el reproductor y evita que se cargue el tema. El contenido y la plantilla de la página no se usan para esa URL.

**Siguiente:** [Configuración](02-configuration.html) — Establecer nombre de estación, tema, visualizador, imágenes y parrilla opcional.
