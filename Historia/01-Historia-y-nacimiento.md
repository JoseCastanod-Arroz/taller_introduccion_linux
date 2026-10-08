---
tags:
  - linux
  - software-libre
  - historia
---

# Historia y nacimiento de GNU/Linux

## Línea de tiempo: de GNU a GNU/Linux

```
1969 ──► UNIX nace en los laboratorios Bell (AT&T)
         Sistema potente, pero propietario y cerrado.

1983 ──► Richard Stallman anuncia el PROYECTO GNU
         "GNU's Not Unix": crear un SO 100% libre.

1985 ──► Se funda la Free Software Foundation (FSF)
         y se formaliza la idea de "software libre".

1989 ──► Nace la licencia GPL (GNU General Public License)
         El "copyleft" que protege la libertad del código.

1991 ──► Linus Torvalds publica el KERNEL LINUX
         La pieza que le faltaba a GNU: el núcleo.

1992 ──► GNU + Linux = GNU/Linux
         Un sistema operativo completo, libre y funcional.

1993 ──► Nace Debian, una de las distros más influyentes.

2004 ──► Nace Ubuntu: Linux "para seres humanos".
```

Nota: GNU aportó todas las herramientas del sistema (compilador GCC, shell bash, utilidades...) pero le faltaba el kernel. Linux aportó justamente ese kernel. Por eso técnicamente el sistema se llama GNU/Linux, aunque popularmente se le diga solo "Linux".

---

## El Proyecto GNU (1983)

- Iniciado por **Richard Stallman** en el MIT.
- Objetivo: construir un sistema operativo **completo y libre**, compatible con UNIX pero sin su código propietario.
- GNU = acrónimo recursivo: **"GNU's Not Unix"**.
- Desarrolló las piezas esenciales:
	- `GCC` → compilador de C
	- `Bash` → intérprete de comandos (shell)
	- `Coreutils`, `Emacs`, `glibc`, etc.

> A GNU solo le faltaba una pieza crítica para funcionar: **el kernel**.

Nota: El kernel oficial de GNU (Hurd) se retrasó durante años, y ese hueco lo llenó Linux en 1991.

---

## El kernel Linux (1991)

- **Linus Torvalds**, estudiante finlandés de 21 años, crea un kernel por hobby.
- Mensaje original en Usenet:

> *"Estoy haciendo un sistema operativo (libre, solo un hobby, no será grande ni profesional como GNU)..."*

- Lo libera bajo la licencia **GPL**.
- Al unirse con las herramientas GNU, nace un sistema operativo **completo**:

<br>

### Herramientas GNU + Kernel Linux = **GNU/Linux**

Nota: La combinación fue perfecta: GNU tenía todo menos el núcleo, y Linux era exactamente ese núcleo libre que faltaba.
