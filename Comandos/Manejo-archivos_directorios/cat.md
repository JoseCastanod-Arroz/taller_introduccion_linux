# `cat`

*Concatenate*. Muestra el contenido completo de un archivo en la terminal. También sirve para concatenar varios archivos.

## Descripción

Imprime el contenido de uno o más archivos. Es útil para ver archivos pequeños rápidamente o para unir varios archivos en uno solo.

## Sintaxis y ejemplos

```bash
cat archivo.txt            # Muestra el contenido
cat a.txt b.txt            # Muestra el contenido de ambos seguidos
cat a.txt b.txt > c.txt    # Concatena a.txt y b.txt en c.txt
```

## Opciones

| Opción  | Descripción |
|---------|-------------|
| `-n`    | Numera todas las líneas |
| `-b`    | Numera solo las líneas no vacías |
| `-s`    | Suprime líneas en blanco repetidas (deja una sola) |
| `-E`    | Muestra un `$` al final de cada línea |
| `-T`    | Muestra las tabulaciones como `^I` |
| `-A`    | Muestra todos los caracteres no imprimibles (equivale a `-vET`) |

> **Consejo:** Usa `man cat` o `cat --help` para ver todas las opciones.
