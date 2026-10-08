# `mv`

*Move*. Mueve o renombra archivos y directorios.

## Descripción

Sirve tanto para mover archivos/carpetas a otra ubicación como para renombrarlos (cuando el destino está en el mismo directorio con otro nombre).

## Sintaxis y ejemplos

```bash
mv archivo.txt /ruta/destino/    # Mueve un archivo
mv viejo.txt nuevo.txt           # Renombra un archivo
mv carpeta/ /ruta/destino/       # Mueve una carpeta
```

## Opciones

| Opción  | Descripción |
|---------|-------------|
| `-i`    | Pide confirmación antes de sobrescribir |
| `-f`    | Fuerza el movimiento sin pedir confirmación |
| `-u`    | Mueve solo si el origen es más reciente que el destino |
| `-v`    | Muestra lo que va moviendo (verbose) |
| `-n`    | No sobrescribe archivos existentes |
| `-b`    | Crea una copia de respaldo del archivo sobrescrito |

> **Consejo:** Usa `man mv` o `mv --help` para ver todas las opciones.
