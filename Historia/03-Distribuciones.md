---
tags:
  - linux
  - software-libre
  - historia
---

# GNU/Linux y las distribuciones

## Definición de GNU/Linux

**GNU/Linux** es un sistema operativo **libre y de código abierto** formado por:

- **Kernel Linux** → el núcleo que gestiona el hardware (CPU, memoria, dispositivos, procesos).
- **Herramientas GNU** → el entorno de usuario (shell, compiladores, utilidades, librerías).

<br>

Juntos forman un sistema operativo **completo, funcional y 100% libre**, capaz de ejecutar desde un teléfono hasta un superordenador.

Nota: Decir solo "Linux" es técnicamente impreciso: Linux es únicamente el kernel. El sistema completo es GNU/Linux. En el habla común se usa "Linux" por simplicidad.

---

## ¿Qué es una distribución (distro)?

Una **distribución** es un sistema operativo **listo para usar**, armado a partir del kernel Linux + software GNU + componentes extra, empaquetados por una comunidad o empresa.

Piensa en ella como una **receta**: todos parten de ingredientes similares (kernel, GNU) pero cada distro los combina y sazona de forma distinta.

Nota: Existen cientos de distros. Cada una toma decisiones distintas sobre qué incluir y cómo configurarlo.

---

## ¿Qué hace que una distro sea una distro?

Una distribución se define por el conjunto de decisiones y componentes que empaqueta:

- **Kernel Linux** (a veces modificado).
- **Gestor de paquetes** → cómo instalas software (`apt`, `dnf`, `pacman`...).
- **Entorno de escritorio** → GNOME, KDE, XFCE...
- **Sistema de init** → arranque y servicios (systemd...).
- **Políticas y filosofía** → libre vs. incluir drivers propietarios, estabilidad vs. novedad.
- **Ciclo de versiones y soporte** → fijo (releases) o continuo (rolling release).
- **Repositorios** → el catálogo de software disponible.

Nota: La combinación de estas decisiones es lo que da identidad a cada distro: no es solo el kernel, sino TODO el conjunto y la filosofía detrás.

---

## Debian (1993)

- Una de las distribuciones **más antiguas e influyentes**; base de muchísimas otras.
- Desarrollada por una **comunidad global de voluntarios**, sin una empresa detrás.
- Pilares:
	- **Estabilidad** → preferida para servidores.
	- **Compromiso con el software libre** → "Contrato Social de Debian".
	- Gestor de paquetes **`apt`** y formato **`.deb`**.
- Es la **base de Ubuntu**, Linux Mint, Kali Linux y muchas más.

> Debian = robustez, comunidad y principios libres.

Nota: El Contrato Social de Debian es un documento público donde la comunidad se compromete con sus usuarios y con el software libre. Su reputación de estabilidad la hace muy popular en servidores.

---

## Ubuntu (2004) y su filosofía

- Creada por **Canonical** (empresa fundada por Mark Shuttleworth).
- Basada en **Debian**, pero enfocada en ser **fácil, accesible y amigable**.
- Lanzamientos regulares cada 6 meses + versiones **LTS** (soporte de 5 años).

### Filosofía: *"Linux for human beings"*

- **Ubuntu** es una palabra africana (zulú/xhosa): *"yo soy porque nosotros somos"* → **humanidad y comunidad**.
- Objetivo: acercar Linux a cualquier persona, no solo a expertos.

Nota: Ubuntu fue clave para popularizar Linux en el escritorio y bajar la barrera de entrada. La filosofía "ubuntu" refleja el espíritu comunitario y colaborativo del software libre.
