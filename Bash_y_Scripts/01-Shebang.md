---
tags:
  - linux
  - bash
  - scripts
---

# ¿Qué es "#!/bin/bash"?

Cuando abres un script casi siempre verás esta línea justo al principio:

```bash
#!/bin/bash
```

A esa línea se le llama **shebang** (o *hashbang*), porque empieza con los símbolos `#!`.

## ¿Para qué sirve?

El shebang le dice al sistema **qué programa debe usar para interpretar y ejecutar el archivo**. Un script es solo un archivo de texto; por sí solo el sistema no sabe en qué "idioma" está escrito. El shebang resuelve esa duda:

- `#!` → marca especial que indica "aquí viene la ruta del intérprete".
- `/bin/bash` → la ruta al programa que ejecutará el script. En este caso, el intérprete **Bash**.

Es decir: *"ejecuta este archivo usando el programa que está en `/bin/bash`"*.

## ¿Por qué es importante?

- Si **omites** el shebang, al ejecutar el script el sistema usará el intérprete por defecto de tu terminal, que no siempre es Bash. Esto puede hacer que un script falle en otra máquina.
- Poner `#!/bin/bash` garantiza que tu script se interprete siempre con Bash, sin importar qué shell esté usando el usuario.

## Detalles útiles

- Debe ir **en la primera línea** del archivo, sin nada antes (ni espacios ni líneas en blanco).
- Aunque empieza con `#` (que en Bash es un comentario), el sistema le da un trato especial **solo** cuando está en la primera línea y va acompañado del `!`.
- Verás variantes como `#!/usr/bin/env bash`, que busca Bash en el entorno del usuario y es más portable entre sistemas.

> En resumen: el shebang es la "etiqueta" que indica con qué intérprete se debe leer el script. Para nuestros scripts de Bash, siempre empezaremos con `#!/bin/bash`.
