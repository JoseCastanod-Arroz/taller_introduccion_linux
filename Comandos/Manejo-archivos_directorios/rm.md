# `rm`

*Remove*. Elimina archivos y directorios.

> **⚠️ Advertencia:** Es una operación irreversible: `rm` no envía los archivos a la papelera, los borra definitivamente.

## Descripción

Borra archivos y, con la opción `-r`, también directorios y todo su contenido.

## Sintaxis y ejemplos

```bash
rm archivo.txt       # Elimina un archivo
rm -r carpeta        # Elimina una carpeta y su contenido (recursivo)
rm -i archivo.txt    # Pide confirmación antes de borrar
```

## Opciones

| Opción  | Descripción |
|---------|-------------|
| `-r`    | Elimina de forma recursiva (carpetas y su contenido) |
| `-f`    | Fuerza el borrado sin pedir confirmación ni dar error si no existe |
| `-i`    | Pide confirmación antes de cada borrado |
| `-I`    | Pide confirmación una sola vez al borrar muchos archivos |
| `-v`    | Muestra lo que va eliminando (verbose) |
| `-d`    | Elimina directorios vacíos |

> **Consejo:** Usa `man rm` o `rm --help` para ver todas las opciones.
