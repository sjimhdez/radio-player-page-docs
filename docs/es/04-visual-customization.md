# Personalización visual

Podéis adaptar el aspecto del reproductor con temas de color, visualizadores de audio e imágenes. Todas las opciones son por estación y se configuran en **Ajustes → Radio Player Page Settings**.

**Anterior:** [Parrilla de programación](03-program-schedule.md) · **Siguiente:** [Múltiples estaciones](05-multiple-stations.md)

## Tema de color

Hay ocho temas de color. Todos usan fondo oscuro; solo cambia el color de acento.

| Tema    | Descripción          |
|---------|----------------------|
| Neutral | Acento gris por defecto |
| Blue    | Acento azul          |
| Green   | Acento verde         |
| Red     | Acento rojo          |
| Orange  | Acento naranja       |
| Yellow  | Acento amarillo      |
| Purple  | Acento morado        |
| Pink    | Acento rosa          |

Seleccionad el tema en el desplegable **Theme Color** de cada estación. Por defecto: **Neutral**.

## Visualizadores

Hay cuatro visualizaciones de audio en tiempo real. Se cargan solo cuando hace falta (lazy-loaded) y se ejecutan solo mientras hay audio.

| Visualizador          | Tipo               | Descripción                |
|-----------------------|--------------------|----------------------------|
| Oscilloscope          | Forma de onda (por defecto) | Forma de onda clásica en dominio temporal |
| Bars Spectrum         | Frecuencia         | Barras de frecuencias      |
| Amplitude Waterfall   | Amplitud           | Cascada de amplitud        |
| Spectral Particles    | Frecuencia         | Vista de partículas        |

Seleccionad el **Visualizer** en los ajustes de la estación. Por defecto: **Oscilloscope**. La visualización requiere que el navegador soporte la Web Audio API (todos los navegadores modernos de escritorio y móviles la soportan).

## Imágenes

### Logo de estación

El **Logo Image** de la estación se muestra en el reproductor y en los controles de medios del sistema (pantalla de bloqueo, notificación, controles de escritorio). Tamaño recomendado: **512×512 píxeles** o más. Configuradlo en el bloque de la estación en **Logo Image (Optional)**.

### Imagen de fondo

La **Background Image** se muestra a tamaño completo detrás del reproductor. No hay un tamaño fijo; usad una imagen que se vea bien en distintas resoluciones. Configuradla en **Background Image (Optional)**.

### Logo de programa

Cuando definís programas en la [Parrilla de programación](03-program-schedule.md), podéis adjuntar una imagen opcional a cada programa. Tamaño recomendado: **256×256 píxeles**. Los logotipos de programa aparecen en el modal de parrilla y en el modal de todos los programas.

## Notas

- **Diseño responsive** — El reproductor se adapta a escritorio, tablet y móvil.
- **iOS** — El control de volumen se oculta en iOS porque el sistema controla el volumen de reproducción. Los streams HLS usan el reproductor nativo de Safari cuando está disponible.
- **Rendimiento** — Los visualizadores y las librerías de streaming (p. ej. para HLS/DASH) se cargan bajo demanda para mantener la carga inicial ligera.

**Anterior:** [Parrilla de programación](03-program-schedule.md) · **Siguiente:** [Múltiples estaciones](05-multiple-stations.md)
