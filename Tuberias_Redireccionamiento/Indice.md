# Índice de Tuberías y Redireccionamiento

En la terminal, los comandos no están aislados: podemos **conectar la salida de uno con la entrada de otro** y **enviar resultados a archivos** en lugar de a la pantalla. Esas dos ideas (tuberías y redireccionamiento) son la base de la potencia de la línea de comandos en Linux, porque permiten combinar herramientas pequeñas para resolver tareas complejas. En esta sección verás primero los tres flujos de datos (stdin, stdout, stderr), luego cómo redirigir esos flujos hacia archivos, y por último cómo encadenar comandos con tuberías. Cada enlace lleva a una nota con explicaciones y ejemplos.

## Temas

- [Flujos de datos: stdin, stdout y stderr](01-Flujos-de-datos.md) - Las tres "corrientes" de entrada y salida que usa todo comando.
- [Redireccionamiento](02-Redireccionamiento.md) - Enviar la salida a archivos y leer la entrada desde archivos (`>`, `>>`, `<`, `2>`).
- [Tuberías (pipes)](03-Tuberias.md) - Conectar comandos con `|` para encadenar su trabajo.
