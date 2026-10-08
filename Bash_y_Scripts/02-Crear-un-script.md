---
tags:
  - linux
  - bash
  - scripts
---

# Crear un script paso a paso

Vamos a crear nuestro primer script desde cero, usando comandos que ya conocemos.

## Paso 1: Crear el archivo con `touch`

Un script de Bash suele llevar la extensión **`.sh`**. Creamos el archivo vacío con `touch`:

```bash
touch mi_script.sh
```

Esto genera un archivo llamado `mi_script.sh` en el directorio actual. Puedes comprobar que existe con `ls`.

> La extensión `.sh` no es obligatoria para que funcione, pero es una convención que ayuda a identificar de un vistazo que el archivo es un script de shell.

## Paso 2: Editar el archivo con `nano`

Ahora abrimos el archivo con el editor `nano` para escribir dentro:

```bash
nano mi_script.sh
```

Se abrirá el editor dentro de la terminal. Ahí escribimos el contenido del script.

## Paso 3: Escribir un ejemplo sencillo

Dentro de `nano`, escribimos lo siguiente:

```bash
#!/bin/bash

echo "¡Hola, mundo!"
echo "Este es mi primer script en Bash."
```

Línea por línea:

- `#!/bin/bash` → el **shebang**, indica que el script se ejecuta con Bash.
- Línea en blanco → solo para que se lea mejor; no afecta la ejecución.
- `echo "¡Hola, mundo!"` → el comando `echo` imprime en pantalla el texto que le pasamos.
- `echo "Este es mi primer script en Bash."` → imprime una segunda línea de texto.

Para **guardar y salir** de `nano`:

1. Pulsa `Ctrl + O` y luego `Enter` para guardar (*write Out*).
2. Pulsa `Ctrl + X` para salir del editor.

Con esto ya tenemos el script escrito y guardado. El siguiente paso es darle permisos y ejecutarlo (ver [Permisos y ejecución](03-Permisos-y-ejecucion.md)).
