---
layout: default
title: Parrilla de programación
---

# Parrilla de programación

La parrilla de programación permite que el reproductor muestre **qué suena ahora** y **qué viene después**. Definid programas (nombre, logo y descripciones opcionales) y asignadlos a franjas horarias para cada día de la semana. El reproductor usa la zona horaria de WordPress y se actualiza al inicio de cada minuto.

**Anterior:** [Configuración](02-configuration.html) · **Siguiente:** [Personalización visual](04-visual-customization.html)

## Qué muestra el reproductor

- **Programa actual** — Bajo el título de la estación: nombre del programa y franja horaria (p. ej. “Programa matinal – 08:00–10:00”).
- **Próximo programa** — Cuando el siguiente programa empieza en 10 minutos o menos, aparece un anuncio (p. ej. “Próximamente: Noticias del mediodía en 5 min”).
- **Modal de parrilla** — Vista semanal con el día actual primero y scroll automático al programa activo; “Volver a hoy” y botón de cerrar.
- **Modal de todos los programas** — Lista alfabética de todos los programas con sus franjas semanales. Las descripciones y descripciones extendidas se muestran en estos modales.

Todas las horas se basan en la **zona horaria de WordPress** (Ajustes → General). La “hora actual” en el reproductor es la hora de la emisora, no necesariamente la hora local del visitante. Cuando la zona horaria de la emisora difiere de la del visitante, el reloj de zona horaria en el reproductor muestra la hora de la emisora y la diferencia.

## En el admin: Programas

Expandid **Show Program Schedule** para la estación. En la sección **Programs**:

1. Haced clic en **Add Program** por cada programa que queráis definir.
2. Para cada programa:
   - **Program name** (obligatorio si lo usáis en la parrilla) — Nombre corto mostrado en el reproductor y en la parrilla.
   - **Add Program Image** / **Change Image** — Logo opcional; tamaño recomendado 256×256 px. Se usa en el reproductor y en la parrilla/modales.
   - **Description** y **extended description** opcionales (si usáis el área “Show more fields”) — Se muestran en la parrilla y en el modal de todos los programas.
3. Usad **Remove Program** para eliminar un programa. Si está en alguna franja, quitad o cambiad primero esas franjas.

Validación: si un programa se usa en la parrilla, debe tener nombre. El formulario mostrará un error y hará scroll al primer problema si intentáis guardar con nombre faltante o franjas no válidas.

*[Figura: Panel de parrilla en el admin con Programs y Schedule por día. Añadir captura como `../../assets/images/admin-schedule-panel.jpg` cuando se disponga.]*

## En el admin: Schedule

En la sección **Schedule** asignáis programas a franjas horarias para cada día (de lunes a domingo).

1. Para el día deseado, haced clic en **Add Time Slot**.
2. En cada franja:
   - **Select Program** — Elegid uno de los programas definidos.
   - **Start** y **End** — Formato 24 horas (HH:MM). Por ejemplo, las 14:00 son las 2 de la tarde.
3. Podéis añadir varias franjas por día. Usad **Remove Time Slot** para eliminar una franja.

### Reglas

- **Sin solapamientos** el mismo día. Si dos franjas se solapan, ambas mostrarán un error (p. ej. “This time slot overlaps with: Programa matinal”). Corregid las horas para que no se solapen.
- **Programas que cruzan medianoche** están permitidos. Por ejemplo, una franja de 23:00 a 01:00 es válida; el plugin la trata como que cruza medianoche.
- Las horas se guardan y muestran en formato 24 horas. El reproductor usa la zona horaria de WordPress para decidir qué programa es “ahora” y cuál es “siguiente”.

La descripción bajo la parrilla en el admin lo resume: asignad programas a franjas por día; el reproductor muestra el programa actual y el siguiente y puede anunciar el próximo cuando empiece en 10 minutos o menos; la visualización usa la zona horaria del sitio y se actualiza al inicio de cada minuto.

*[Figura: Reproductor con programa actual y anuncio “Próximamente” opcional. Añadir captura como `../../assets/images/player-now-playing.jpg` cuando se disponga.]*

*[Figura: Modal de parrilla o de todos los programas en el reproductor. Añadir captura como `../../assets/images/program-modal.jpg` cuando se disponga.]*

## Zona horaria

El “ahora” usado para el programa actual y el anuncio del “siguiente” es la **hora del sitio WordPress** (Ajustes → General → Zona horaria). Si vuestra emisora emite en otra zona horaria, configurad la zona horaria de WordPress a la de la emisora. El reloj de zona horaria en el reproductor (cuando se muestra) indica la hora de la emisora y la diferencia con la del visitante.

**Anterior:** [Configuración](02-configuration.html) · **Siguiente:** [Personalización visual](04-visual-customization.html)
