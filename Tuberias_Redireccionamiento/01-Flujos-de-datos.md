---
tags:
  - linux
  - terminal
  - redireccionamiento
---

# Flujos de datos: stdin, stdout y stderr

Antes de hablar de tuberías y redireccionamiento, hay que entender que casi todos los comandos de Linux trabajan con **tres flujos (o canales) de datos**. Imagina cada comando como una pequeña máquina con una entrada y dos salidas.

| Flujo | Nombre | Número | ¿Para qué sirve? |
|-------|--------|:------:|------------------|
| **stdin** | Entrada estándar | `0` | Por donde el comando **recibe** datos (normalmente, lo que escribes en el teclado). |
| **stdout** | Salida estándar | `1` | Por donde el comando **envía sus resultados** normales (normalmente, la pantalla). |
| **stderr** | Salida de error | `2` | Por donde el comando **envía los mensajes de error**, separados de los resultados. |

## ¿Por qué separar la salida normal de los errores?

A primera vista, en la terminal tanto `stdout` como `stderr` aparecen mezclados en la pantalla. Pero son canales distintos, y eso es muy útil: podemos **guardar los resultados en un archivo** y, al mismo tiempo, **ver los errores aparte** (o guardarlos en otro archivo).

Por ejemplo, el comando `ls` imprime la lista de archivos por `stdout`, pero si le pides un archivo que no existe, el mensaje de error sale por `stderr`.

```bash
ls archivo_que_no_existe
# ls: cannot access 'archivo_que_no_existe': No such file or directory  (esto es stderr)
```

## La idea clave

Todo lo que veremos a continuación consiste en **redirigir estos flujos**:

- Mandar `stdout` a un archivo en vez de a la pantalla → **redireccionamiento**.
- Tomar `stdin` desde un archivo en vez del teclado → **redireccionamiento**.
- Conectar el `stdout` de un comando con el `stdin` de otro → **tubería (pipe)**.

Entender estos tres canales es la base para dominar las siguientes dos notas.
