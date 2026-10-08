# `mkdir`

*Make Directory*. Crea uno o varios directorios.

## Descripción

Crea carpetas nuevas. Con la opción `-p` puede crear toda una jerarquía de carpetas anidadas de una sola vez.

## Sintaxis y ejemplos

```bash
mkdir carpeta              # Crea una carpeta
mkdir -p padre/hijo/nieto  # Crea toda la jerarquía de carpetas
```

## Opciones

| Opción      | Descripción |
|-------------|-------------|
| `-p`        | Crea las carpetas padre necesarias; no da error si ya existen |
| `-v`        | Muestra un mensaje por cada carpeta creada (verbose) |
| `-m MODO`   | Asigna permisos al crear (ej. `-m 755`) |

> **Consejo:** Usa `man mkdir` o `mkdir --help` para ver todas las opciones.
