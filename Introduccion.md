# Introducción al Taller de GNU/Linux

¡Bienvenido/a! Este repositorio reúne todos los apuntes del taller de introducción a GNU/Linux. El material está pensado para repasar lo visto en las sesiones y para consultarlo por tu cuenta, tema por tema, a tu propio ritmo.

Esta nota es tu punto de partida: te explica **cómo están organizados los apuntes** y **cómo encontrar lo que buscas**.

## Cómo están organizados los apuntes

El contenido se divide en cuatro secciones, cada una en su propia carpeta. Dentro de cada carpeta hay un archivo `Indice.md` que resume la sección y enlaza, en orden, a cada una de sus notas.

- **[Historia](Historia/Indice.md)** — De GNU a GNU/Linux: el nacimiento del software libre, su filosofía, las distribuciones (Debian, Ubuntu) y por qué Linux es relevante hoy.
- **[Comandos](Comandos/Indice.md)** — Referencia de comandos básicos de la terminal, divididos en *Navegación* (`pwd`, `cd`, `ls`) y *Manejo de archivos y directorios* (`cat`, `cp`, `mkdir`, `mv`, `nano`, `rm`, `touch`, `less`, `more`).
- **[Tuberías y Redireccionamiento](Tuberias_Redireccionamiento/Indice.md)** — Los flujos de datos (stdin, stdout, stderr), cómo redirigir salida a archivos (`>`, `>>`, `<`, `2>`) y cómo encadenar comandos con tuberías (`|`).
- **[Bash y Scripts](Bash_y_Scripts/Indice.md)** — El salto de comandos sueltos a scripts: el shebang `#!/bin/bash`, cómo crear tu primer script y cómo darle permisos para ejecutarlo.

## Cómo buscar un apunte

Tienes tres formas de llegar a lo que necesitas:

1. **Empieza por el índice de la sección.** Abre la carpeta del tema que te interese y lee su `Indice.md`. Ahí encontrarás una breve descripción de cada nota y un enlace directo para abrirla. Es la ruta recomendada si quieres seguir el material en orden.

2. **Ve directo al archivo.** Si ya sabes qué buscas, los nombres son descriptivos. Por ejemplo, el comando `ls` está en `Comandos/Navegacion/ls.md`, y el tema de tuberías en `Tuberias_Redireccionamiento/03-Tuberias.md`. Las notas numeradas (`01-`, `02-`, ...) están pensadas para leerse en ese orden.

3. **Busca por palabra clave.** Si no recuerdas dónde está algo, usa el buscador de tu editor o la terminal:

   ```bash
   # Buscar en qué archivos aparece una palabra (por ejemplo, "chmod")
   grep -ri "chmod" .

   # Buscar un archivo por su nombre (por ejemplo, todo lo relacionado con "redireccion")
   find . -iname "*redireccion*"
   ```

## Ruta sugerida para el taller

Si es tu primera vez, te recomendamos recorrer las secciones en este orden:

1. **Historia** — para entender qué es GNU/Linux y de dónde viene.
2. **Comandos** — para aprender a moverte y trabajar en la terminal.
3. **Tuberías y Redireccionamiento** — para combinar comandos y sacarles más provecho.
4. **Bash y Scripts** — para automatizar tareas escribiendo tus propios scripts.

> Consejo: todas las notas están en formato Markdown (`.md`), así que puedes leerlas directamente en GitHub, en un editor como VS Code, o en cualquier visor de Markdown. Los enlaces entre notas son relativos, por lo que funcionan sin conexión.

¡A explorar! 🐧
