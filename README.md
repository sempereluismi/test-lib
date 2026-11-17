# test-lib

## Documentacion

El contenido de [`docs/`](docs/) es la fuente de verdad de la wiki de GitHub.
El workflow [Sync docs to GitHub Wiki](.github/workflows/sync-wiki.yml) publica
los cambios de `docs/` en la wiki al hacer push a `main`. La sincronizacion es
un espejo: las paginas eliminadas de `docs/` tambien se eliminan de la wiki.

### Configuracion de GitHub

1. Habilita la wiki del repositorio y crea su primera pagina en GitHub.
2. Crea un token con permiso de escritura en la wiki.
3. Guarda el token en **Settings > Secrets and variables > Actions** con el
   nombre `WIKI_TOKEN`.

El workflow tambien se puede ejecutar manualmente desde la pestana **Actions**.