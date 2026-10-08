# `nano`

Editor de texto sencillo que funciona dentro de la terminal.

## Descripción

`nano` es un editor de texto fácil de usar, ideal para principiantes. Permite crear y editar archivos directamente en la terminal mostrando en la parte inferior los atajos de teclado disponibles. Si el archivo indicado no existe, lo crea al guardar.

## Sintaxis y ejemplos

```bash
nano archivo.txt          # Abre (o crea) un archivo para editarlo
nano +10 archivo.txt      # Abre el archivo en la línea 10
nano -l archivo.txt       # Muestra números de línea
```

## Atajos de teclado (dentro de nano)

El símbolo `^` representa la tecla **Ctrl**.

| Atajo        | Acción |
|--------------|--------|
| `Ctrl + O`   | Guardar (Write Out) |
| `Ctrl + X`   | Salir |
| `Ctrl + K`   | Cortar la línea actual |
| `Ctrl + U`   | Pegar |
| `Ctrl + W`   | Buscar texto |
| `Ctrl + \`   | Buscar y reemplazar |
| `Ctrl + G`   | Mostrar la ayuda |

## Opciones

| Opción  | Descripción |
|---------|-------------|
| `-l`    | Muestra los números de línea |
| `-m`    | Habilita el uso del ratón |
| `-i`    | Sangría automática (autoindent) |
| `-v`    | Abre el archivo en modo solo lectura |
| `-B`    | Crea una copia de respaldo al guardar |
| `+N`    | Abre el archivo situando el cursor en la línea N |

> **Consejo:** Usa `man nano` o `nano --help` para ver todas las opciones.
