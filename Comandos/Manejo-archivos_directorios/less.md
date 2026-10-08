# `less`

Visor de contenido página por página. Permite desplazarse hacia arriba y abajo. Ideal para archivos grandes.

## Descripción

Abre un archivo en un visor interactivo que no carga todo el contenido en memoria de golpe, por lo que es muy eficiente con archivos grandes. Se sale con la tecla `q`.

## Sintaxis y ejemplos

```bash
less archivo.txt
```

### Navegación dentro de `less`

- `Espacio` o `f`: avanzar una página
- `b`: retroceder una página
- `/texto`: buscar "texto"
- `n`: siguiente coincidencia de búsqueda
- `g`: ir al inicio del archivo
- `G`: ir al final del archivo
- `q`: salir

## Opciones

| Opción  | Descripción |
|---------|-------------|
| `-N`    | Muestra números de línea |
| `-S`    | No divide líneas largas (se desplazan horizontalmente) |
| `-i`    | Búsqueda sin distinguir mayúsculas/minúsculas |
| `-g`    | Resalta solo la última coincidencia de búsqueda |
| `-F`    | Sale automáticamente si el contenido cabe en una pantalla |
| `+F`    | Modo seguimiento, como `tail -f` |
| `-X`    | No limpia la pantalla al salir |

> **Consejo:** Usa `man less` para ver todas las opciones.
