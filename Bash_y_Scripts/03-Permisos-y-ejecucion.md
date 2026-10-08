---
tags:
  - linux
  - bash
  - scripts
---

# Permisos y ejecución

Ya tenemos el script creado y escrito. Pero si intentamos ejecutarlo directamente, el sistema no nos dejará todavía: falta darle **permiso de ejecución**.

## ¿Por qué hacen falta permisos?

En Linux, cada archivo tiene permisos que definen quién puede **leerlo** (`r`), **escribirlo** (`w`) y **ejecutarlo** (`x`). Un archivo creado con `touch` nace como texto normal, **sin** permiso de ejecución. Para poder correrlo como programa, hay que activárselo.

## Paso 1: Dar permisos de ejecución con `chmod`

Usamos el comando `chmod` (del inglés *change mode*) para añadir el permiso de ejecución:

```bash
chmod +x mi_script.sh
```

- `chmod` → cambia los permisos de un archivo.
- `+x` → añade (`+`) el permiso de ejecución (`x`).
- `mi_script.sh` → el archivo al que se le aplican los permisos.

Puedes verificar el cambio con `ls -l`: ahora deberían aparecer unas `x` en los permisos del archivo.

```bash
ls -l mi_script.sh
# -rwxr-xr-x  1 usuario usuario  60 oct  7 10:00 mi_script.sh
```

Las `x` en `-rwxr-xr-x` indican que el archivo ya es ejecutable.

## Paso 2: Ejecutar el script

Para ejecutarlo, lo llamamos indicando que está en el directorio actual con `./`:

```bash
./mi_script.sh
```

- `./` → significa "en esta carpeta". Le dice al sistema que busque el script en el directorio actual y no entre los comandos del sistema.
- `mi_script.sh` → el nombre del archivo a ejecutar.

La salida será:

```
¡Hola, mundo!
Este es mi primer script en Bash.
```

> Si olvidas el `./` y escribes solo `mi_script.sh`, el sistema buscará el comando en las rutas del sistema y no lo encontrará. Por eso usamos `./` para los scripts del directorio actual.

## Alternativa: ejecutar sin permisos

También puedes correr el script pasándoselo directamente a Bash, sin necesidad de `chmod`:

```bash
bash mi_script.sh
```

Aquí es **Bash** quien lee y ejecuta el archivo, por lo que no hace falta el permiso de ejecución. Es una opción práctica para pruebas rápidas, pero lo habitual es dar permisos con `chmod +x` y ejecutarlo con `./`.
