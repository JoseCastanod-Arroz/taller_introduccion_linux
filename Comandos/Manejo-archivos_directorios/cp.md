# `cp`

*Copy*. Copia archivos y directorios de un origen a un destino.

## Descripción

Crea copias de archivos o carpetas. Para copiar directorios completos se necesita la opción `-r` (recursivo).

## Sintaxis y ejemplos

```bash
cp origen.txt destino.txt        # Copia un archivo
cp archivo.txt /ruta/destino/    # Copia a otra carpeta
cp -r carpeta/ destino/          # Copia una carpeta completa (recursivo)
```

## Opciones

| Opción  | Descripción |
|---------|-------------|
| `-r` / `-R` | Copia carpetas de forma recursiva |
| `-i`    | Pide confirmación antes de sobrescribir |
| `-f`    | Fuerza la copia sobrescribiendo si es necesario |
| `-u`    | Copia solo si el origen es más reciente que el destino |
| `-v`    | Muestra los archivos copiados (verbose) |
| `-p`    | Conserva atributos (permisos, fechas, propietario) |
| `-a`    | Modo archivo: copia preservando todo (equivale a `-dR --preserve=all`) |
| `-l`    | Crea enlaces duros en lugar de copiar |
| `-s`    | Crea enlaces simbólicos en lugar de copiar |

> **Consejo:** Usa `man cp` o `cp --help` para ver todas las opciones.
