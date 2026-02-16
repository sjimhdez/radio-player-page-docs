---
layout: default
title: Preguntas frecuentes
---

# Preguntas frecuentes

**Anterior:** [Múltiples estaciones](05-multiple-stations.html) · **Volver a:** [Índice de documentación](index.html)

## ¿Hay que configurar algo en la página de WordPress?

No. Una vez asignéis una página a una estación en **Ajustes → Radio Player Page Settings**, no hace falta nada más en la página. El plugin intercepta las peticiones a esa página y sirve una página HTML independiente con el reproductor. El contenido, la plantilla y los ajustes de la página no se usan para esa URL.

## ¿Dónde puedo obtener soporte o reportar problemas?

Usad el [foro de soporte de WordPress.org para Radio Player Page](https://wordpress.org/support/plugin/radio-player-page/) para preguntas, peticiones de funciones y reporte de errores.

## ¿Puedo usarlo para emisoras comerciales?

Sí. El plugin es gratuito y de código abierto (GPLv2 o posterior) y puede usarse tanto en emisoras comerciales como no comerciales.

## ¿Dónde está el código fuente?

El código fuente está en [GitHub](https://github.com/sjimhdez/radio-player-page).

## ¿Qué formatos de stream soporta?

El plugin soporta:

- **Icecast** y **Shoutcast** — Protocolos tradicionales de streaming de radio.
- **HLS** (`.m3u8`) — Streaming adaptativo; Safari en iOS usa soporte HLS nativo.
- **DASH** (`.mpd`) — Streaming adaptativo moderno.
- **MP3** — Streaming de audio estándar.

El plugin detecta el tipo de stream automáticamente y carga el reproductor adecuado (incluidas las librerías opcionales para HLS/DASH cuando hace falta).

## ¿En qué idiomas está el reproductor?

La interfaz del reproductor está disponible en: inglés (EE. UU.), español, español (México), ruso, neerlandés, rumano, sueco, gallego y danés. El idioma se elige según el navegador (atributo `lang` del HTML, luego preferencia guardada, luego idioma del navegador), con fallback a inglés.

## ¿Cómo funciona el temporizador de apagado (sleep timer)?

Podéis hacer que el reproductor deje de reproducir tras **30**, **60** o **120** minutos. Se muestra una cuenta atrás mientras el temporizador está activo. Si pausáis la reproducción manualmente, el sleep timer se cancela. El temporizador solo sirve para detener la reproducción automáticamente; no afecta al stream ni a la estación.

## ¿Qué pasa si desinstalo el plugin?

Cuando el plugin se **desinstala** (se elimina del sitio, no solo se desactiva), el script `uninstall.php` se ejecuta y elimina la opción `radplapag_settings` de la base de datos. En multisitio se elimina de cada sitio. La opción **no** se elimina si solo desactiváis el plugin.

## ¿Por qué no carga el stream?

Si el reproductor no arranca o el stream no suena:

1. **Comprobad la URL** — En **Ajustes → Radio Player Page Settings**, aseguraos de que la **Streaming URL** es correcta y accesible (probad a abrirla en otra pestaña o en otro reproductor).
2. **CORS** — Si el stream está en otro dominio, el servidor debe permitir peticiones desde vuestro sitio (cabeceras CORS). Muchos servidores de streaming lo permiten por defecto; si no, puede que tengáis que configurar el servidor del stream.
3. **Consola del navegador** — Abrid las herramientas de desarrollo (F12) y revisad la pestaña Consola en busca de errores. Errores de red o peticiones bloqueadas pueden indicar URL incorrecta o problema de CORS.
4. **Formato** — El plugin soporta Icecast, Shoutcast, HLS, DASH y MP3. Streams poco habituales o protegidos pueden no funcionar.

Si el problema continúa, describid vuestra configuración (tipo de stream, formato de URL y mensajes de error) en el [foro de soporte](https://wordpress.org/support/plugin/radio-player-page/).

**Anterior:** [Múltiples estaciones](05-multiple-stations.html) · **Volver a:** [Índice de documentación](index.html)
