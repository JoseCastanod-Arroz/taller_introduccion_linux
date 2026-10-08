# `touch`

Crea archivos vacíos. Si el archivo ya existe, actualiza su fecha de modificación/acceso.

## Descripción

Su uso más común es crear archivos vacíos rápidamente. También sirve para actualizar las marcas de tiempo (acceso y modificación) de archivos existentes.

## Sintaxis y ejemplos

```bash
touch archivo.txt          # Crea un archivo vacío
touch a.txt b.txt c.txt    # Crea varios archivos a la vez
```

## Opciones

| Opción       | Descripción |
|--------------|-------------|
| `-a`         | Cambia solo la fecha de acceso |
| `-m`         | Cambia solo la fecha de modificación |
| `-c`         | No crea el archivo si no existe |
| `-t STAMP`   | Usa una fecha/hora específica (`[[CC]YY]MMDDhhmm[.ss]`) |
| `-r ARCHIVO` | Usa las fechas de otro archivo de referencia |
| `-d CADENA`  | Usa una fecha indicada como texto (ej. `-d "2024-01-01"`) |

> **Consejo:** Usa `man touch` o `touch --help` para ver todas las opciones.
