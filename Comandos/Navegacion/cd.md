# `cd`

*Change Directory*. Cambia el directorio de trabajo actual.

## Descripción

Permite moverte entre directorios del sistema de archivos usando rutas absolutas o relativas.

## Sintaxis y ejemplos

```bash
cd /ruta/absoluta  # Ir a una ruta absoluta
cd carpeta         # Entrar a una subcarpeta (ruta relativa)
cd ..              # Subir un nivel (directorio padre)
cd ~               # Ir al directorio HOME del usuario
cd -               # Volver al directorio anterior
cd                 # Sin argumentos, va al HOME
```

## Opciones y argumentos

`cd` es un comando interno (builtin) del shell; no usa flags al estilo tradicional, pero acepta argumentos especiales.

| Argumento | Descripción |
|-----------|-------------|
| `..`      | Sube al directorio padre |
| `~`       | Va al directorio HOME del usuario |
| `-`       | Vuelve al directorio anterior |
| (vacío)   | Va al directorio HOME |
| `-P`      | Resuelve enlaces simbólicos al cambiar de directorio |
| `-L`      | Sigue enlaces simbólicos (comportamiento por defecto) |

> **Consejo:** Usa `help cd` para ver la ayuda del builtin del shell.
