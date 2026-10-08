# `pwd`

*Print Working Directory*. Muestra la ruta absoluta del directorio en el que te encuentras actualmente.

## Descripción

Imprime en la terminal la ruta completa del directorio de trabajo actual. Es útil para saber en qué ubicación del sistema de archivos estás.

## Sintaxis y ejemplos

```bash
pwd                # /home/usuario/Documentos
```

## Opciones

| Opción | Descripción |
|--------|-------------|
| `-L`   | Muestra la ruta lógica (respeta enlaces simbólicos). Es el valor por defecto |
| `-P`   | Muestra la ruta física real (resuelve enlaces simbólicos) |

> **Consejo:** Usa `man pwd` o `pwd --help` para ver todas las opciones.
