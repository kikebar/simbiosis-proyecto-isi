# Guía de contribución

Normas para proponer y revisar cambios en la documentación del Proyecto Simbiosis.

## Principios

- La fuente canónica de todo documento propio es su archivo Markdown correspondiente.
- Ningún cambio se incorpora a la rama principal sin pasar por una pull request.
- Los documentos de `docs/referencias/` no se editan: son copias de material externo o recibido.
- Las exportaciones en `releases/` no se editan directamente: se generan a partir de una línea base ya aprobada.

## Flujo de trabajo

1. Crear una rama a partir de la rama principal.
2. Editar o añadir los documentos Markdown correspondientes.
3. Actualizar los metadatos del documento afectado (estado, versión, fecha, fuente, relación con otros documentos) cuando proceda.
4. Abrir una pull request describiendo el cambio y su motivación.
5. Esperar la revisión y aprobación antes de fusionar.

## Convenciones de nombres

- Nombres de archivo en minúsculas, separados por guiones (`kebab-case`).
- No incluir números de versión en el nombre del archivo.

## Líneas base

Cuando un conjunto de documentos alcanza un estado estable acordado:

1. Se registra la línea base en [`CHANGELOG.md`](CHANGELOG.md).
2. Se crea una etiqueta de Git sobre el commit correspondiente.
3. Si procede, se genera y publica la exportación estable en [`releases/`](releases/README.md).

## Plantilla de metadatos

Los documentos de captura y de requisitos deben incluir una tabla de metadatos con, al menos, estos campos:

| Campo | Valor |
| --- | --- |
| Estado | |
| Versión | |
| Fecha | |
| Fuente | |
| Documentos relacionados | |
