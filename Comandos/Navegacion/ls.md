# `ls`

Lista el contenido (archivos y directorios) de una carpeta.

## Descripción

Muestra los archivos y subdirectorios que contiene un directorio. Sin argumentos, lista el directorio actual.

## Sintaxis y ejemplos

```bash
ls                 # Lista el directorio actual
ls /ruta/carpeta   # Lista una carpeta específica
ls -l              # Lista con formato detallado (permisos, tamaño, fecha)
ls -la             # Incluye archivos ocultos en formato detallado
```

## Opciones

| Opción | Descripción |
|--------|-------------|
| `-l`   | Formato largo: permisos, propietario, tamaño y fecha |
| `-a`   | Muestra todos los archivos, incluidos los ocultos (los que empiezan con `.`) |
| `-A`   | Como `-a` pero sin mostrar `.` y `..` |
| `-h`   | Tamaños legibles para humanos (KB, MB, GB). Se usa con `-l` |
| `-R`   | Lista subdirectorios de forma recursiva |
| `-t`   | Ordena por fecha de modificación (más reciente primero) |
| `-r`   | Invierte el orden de la lista |
| `-S`   | Ordena por tamaño de archivo |
| `-F`   | Añade un indicador al final del nombre (`/` carpeta, `*` ejecutable) |
| `-d`   | Muestra el directorio en sí, no su contenido |
| `-1`   | Un archivo por línea |

> **Consejo:** Usa `man ls` o `ls --help` para ver todas las opciones.
