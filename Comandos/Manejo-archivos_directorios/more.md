# `more`

Visor de contenido página por página, más simple que `less`. Solo permite avanzar (en su versión clásica).

## Descripción

Muestra el contenido de un archivo una pantalla a la vez. Es más básico que `less`: tradicionalmente solo avanza hacia adelante. Se sale con `q`.

## Sintaxis y ejemplos

```bash
more archivo.txt
```

### Navegación dentro de `more`

- `Espacio`: avanzar una página
- `Enter`: avanzar una línea
- `/texto`: buscar "texto"
- `q`: salir

## Opciones

| Opción      | Descripción |
|-------------|-------------|
| `-d`        | Muestra instrucciones de uso en pantalla |
| `-f`        | Cuenta líneas lógicas en vez de líneas de pantalla |
| `-p`        | Limpia la pantalla antes de mostrar cada página |
| `-s`        | Comprime múltiples líneas en blanco en una sola |
| `+N`        | Comienza a mostrar desde la línea número N |
| `+/texto`   | Comienza a mostrar desde la primera línea con "texto" |

> **Consejo:** Usa `man more` para ver todas las opciones.
