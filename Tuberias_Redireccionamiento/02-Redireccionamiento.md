---
tags:
  - linux
  - terminal
  - redireccionamiento
---

# Redireccionamiento

**Redireccionar** significa cambiar el destino de la salida de un comando o el origen de su entrada. En lugar de que los resultados salgan por pantalla o que la entrada venga del teclado, los conectamos con **archivos**.

## Redirigir la salida a un archivo: `>`

El operador `>` toma lo que un comando enviaría a la pantalla (`stdout`) y lo **escribe en un archivo**:

```bash
ls > listado.txt
```

Esto guarda la lista de archivos en `listado.txt` en vez de mostrarla. Si el archivo no existe, se crea; si ya existía, **se sobrescribe** (se borra su contenido anterior).

> Cuidado: `>` borra lo que hubiera antes en el archivo.

## Añadir al final de un archivo: `>>`

Si no quieres sobrescribir sino **agregar** al final del archivo, usa `>>`:

```bash
echo "Primera línea" > notas.txt    # crea el archivo con esa línea
echo "Segunda línea" >> notas.txt   # añade sin borrar lo anterior
```

Tras esos dos comandos, `notas.txt` contendrá ambas líneas.

## Redirigir la entrada desde un archivo: `<`

El operador `<` hace que un comando lea su entrada (`stdin`) **desde un archivo** en lugar del teclado:

```bash
wc -l < notas.txt
```

Aquí `wc -l` (que cuenta líneas) recibe el contenido de `notas.txt` como si lo hubiéramos tecleado.

## Redirigir los errores: `2>`

Recuerda que los errores viajan por `stderr` (canal `2`). Podemos redirigirlos por separado usando el número del canal:

```bash
ls carpeta_inexistente 2> errores.txt
```

El mensaje de error se guarda en `errores.txt` en vez de aparecer en pantalla.

### Combinaciones útiles

```bash
# Resultados a un archivo y errores a otro
comando > salida.txt 2> errores.txt

# Mandar resultados y errores al MISMO archivo
comando > todo.txt 2>&1

# Atajo de Bash equivalente al anterior
comando &> todo.txt

# Descartar los errores por completo (enviarlos a la "papelera" del sistema)
comando 2> /dev/null
```

- `2>&1` significa "manda el canal 2 (errores) al mismo sitio que el canal 1 (salida)".
- `&>` es un atajo propio de Bash: `comando &> todo.txt` hace lo mismo que `comando > todo.txt 2>&1`, pero más corto.
- `/dev/null` es un destino especial que descarta todo lo que recibe.

## Resumen de operadores

| Operador | ¿Qué hace? |
|----------|------------|
| `>` | Redirige la salida a un archivo (sobrescribe). |
| `>>` | Redirige la salida a un archivo (añade al final). |
| `<` | Toma la entrada desde un archivo. |
| `2>` | Redirige los errores a un archivo. |
| `2>&1` | Une los errores con la salida normal. |
| `&>` | Atajo de Bash: salida y errores al mismo archivo. |
