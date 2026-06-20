# APEX Mockup

Mockup frontend de APEX para pruebas de flujo operativo. La aplicacion usa React + Vite y se publica como sitio estatico.

## Desarrollo local

```bash
npm ci
npm run dev
```

## Validacion

```bash
npm run lint
npm run build
```

## Publicacion en GitHub Pages

Este proyecto esta preparado para publicarse desde GitHub Actions hacia GitHub Pages.

1. Crear un repositorio dedicado, por ejemplo `apex-mockup-demo`.
2. Subir solo el contenido de esta carpeta `apex-mockup` como raiz del repositorio.
3. En GitHub, abrir `Settings > Pages`.
4. En `Build and deployment`, seleccionar `GitHub Actions`.
5. En GoDaddy, crear el DNS:
   - Tipo: `CNAME`
   - Host: `demo`
   - Valor: `<usuario-u-organizacion>.github.io`
6. En GitHub Pages, configurar el dominio personalizado:
   - `demo.naraconsultores.com`
7. Esperar la propagacion DNS y activar `Enforce HTTPS` cuando GitHub lo permita.

## Alcance de la demo

- No tiene backend ni persistencia real.
- Los datos son mock/locales.
- Al recargar la pagina se reinicia el estado del mockup.
