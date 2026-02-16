---
layout: default
title: Configuración
---

# Configuración

Todas las opciones de las estaciones se gestionan en **Ajustes → Radio Player Page Settings**. Cada estación tiene su propio bloque de opciones; esta página describe cada campo.

**Anterior:** [Instalación](01-installation.html) · **Siguiente:** [Parrilla de programación](03-program-schedule.html)

## Dónde configurar

Abrid **Ajustes → Radio Player Page Settings** en el escritorio de WordPress. Veréis uno o más bloques de estación. Para cada estación que uséis, rellenad al menos **Player Page** y **Streaming URL** y haced clic en **Guardar cambios** al final de la página.

*[Figura: Página de ajustes con las opciones generales de la estación. Añadir captura como `../../assets/images/settings-general.jpg` cuando se disponga.]*

## Campos por estación

### Player Page (obligatorio)

La página de WordPress en la que aparecerá el reproductor. Seleccionadla en el desplegable. Cuando alguien visite la URL de esa página, el plugin sirve el reproductor independiente en lugar del tema. Cada estación debe tener una página distinta.

### Streaming URL (obligatorio)

La URL completa de vuestro stream de audio (p. ej. `https://ejemplo.com:8000/stream` o una URL HLS/DASH). Formatos soportados:

- Icecast y Shoutcast  
- HLS (`.m3u8`)  
- DASH (`.mpd`)  
- Streams MP3  

El plugin valida la URL al guardar y detecta el tipo de stream automáticamente para la reproducción.

### Station Name (opcional)

Un título de la estación (p. ej. “Mi radio”). Máximo 64 caracteres. Si se deja vacío, se usa el título del sitio de **Ajustes → General** en el reproductor y en los controles de medios del sistema.

### Theme Color

Desplegable con ocho opciones: **Neutral**, **Blue**, **Green**, **Red**, **Orange**, **Yellow**, **Purple**, **Pink**. Todos los temas usan fondo oscuro. Por defecto: **Neutral**.

### Visualizer

Elegid la visualización de audio en tiempo real: **Oscilloscope** (por defecto, forma de onda), **Bars Spectrum**, **Amplitude Waterfall** o **Spectral Particles**. Los visualizadores se cargan solo cuando hace falta y se ejecutan solo mientras hay audio.

### Logo Image (opcional)

El logo de la estación, mostrado en el reproductor y en la pantalla de bloqueo y controles de medios del sistema. Tamaño recomendado: 512×512 píxeles o más. Usad **Select Image** para elegir de la biblioteca de medios y **Remove** para quitarlo.

### Background Image (opcional)

Una imagen a tamaño completo mostrada detrás del reproductor. Usad **Select Image** para establecerla y **Remove** para quitarla.

### Program Schedule (opcional)

Sección colapsable para definir **programas** (nombre, logo opcional, descripciones opcionales) y la **parrilla semanal** de franjas horarias por día. El reproductor mostrará entonces el programa actual y el siguiente y puede anunciar el próximo cuando falten 10 minutos o menos. Para todos los detalles, ved [Parrilla de programación](03-program-schedule.html).

## Guardar cambios

Siempre haced clic en **Guardar cambios** al final del formulario después de editar. Hasta que guardéis, los cambios no se almacenan y el reproductor no los reflejará.

**Anterior:** [Instalación](01-installation.html) · **Siguiente:** [Parrilla de programación](03-program-schedule.html)
