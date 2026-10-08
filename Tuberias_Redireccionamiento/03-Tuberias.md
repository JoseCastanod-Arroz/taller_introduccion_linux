---
tags:
  - linux
  - terminal
  - tuberias
---

# Tuberías (pipes)

Una **tubería** (en inglés *pipe*) conecta la **salida de un comando** con la **entrada del siguiente**. Se escribe con el símbolo de barra vertical `|`.

La idea es poderosa: en lugar de guardar un resultado en un archivo y luego procesarlo, pasamos los datos **directamente de un comando a otro**, como agua fluyendo por una tubería.

```bash
comando1 | comando2
```

Aquí el `stdout` de `comando1` se convierte en el `stdin` de `comando2`.

## Un ejemplo sencillo

Supongamos que `ls` lista muchísimos archivos y solo quieres contarlos. El comando `wc -l` cuenta líneas:

```bash
ls | wc -l
```

- `ls` genera la lista de archivos.
- El `|` pasa esa lista a `wc -l`.
- `wc -l` cuenta cuántas líneas (archivos) hay y muestra el número.

Nunca creamos un archivo intermedio: los datos pasaron directo por la tubería.

## Encadenar varios comandos

Las tuberías se pueden encadenar tantas veces como necesites. Cada `|` conecta un comando con el siguiente:

```bash
cat registro.txt | grep "error" | sort | uniq
```

Paso a paso:

1. `cat registro.txt` → muestra el contenido del archivo.
2. `grep "error"` → se queda solo con las líneas que contienen la palabra "error".
3. `sort` → ordena esas líneas alfabéticamente.
4. `uniq` → elimina líneas duplicadas consecutivas.

El resultado final es una lista ordenada y sin repetidos de los errores del archivo.

## Diferencia con el redireccionamiento

Es fácil confundirlos, pero no son lo mismo:

- **Redireccionamiento (`>`, `<`)** conecta un comando con un **archivo**.
- **Tubería (`|`)** conecta un comando con **otro comando**.

```bash
ls > archivo.txt    # la salida de ls va a un ARCHIVO
ls | wc -l          # la salida de ls va a OTRO COMANDO
```

## ¿Por qué son tan importantes?

La filosofía de Linux es tener muchas herramientas pequeñas que hacen **una sola cosa bien**. Las tuberías son el "pegamento" que permite combinarlas para resolver tareas complejas, sin necesidad de un programa gigante que lo haga todo. Dominar `|` es dominar buena parte del poder de la terminal.
