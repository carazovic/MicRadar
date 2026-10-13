# MicoRadar — GitHub Pages

Aplicación web estática de MicoRadar. No requiere Node, compilación ni servidor backend.

## Publicarla

1. Crea un repositorio en GitHub, por ejemplo `micoradar`.
2. Sube `index.html` y este `README.md` a la raíz del repositorio.
3. En **Settings → Pages**, selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`, y guarda.
4. Espera a que termine la publicación y abre la URL que GitHub Pages muestra en Settings → Pages.

## Notas importantes

- La app intenta cargar Google Maps y conserva un mapa de respaldo basado en Leaflet/IGN-Iberpix. Si Google Maps falla (por ejemplo, por restricciones de la clave/API), el encabezado debe indicar el modo de respaldo en lugar de quedarse en «Inicializando».
- GitHub Pages sirve el HTML públicamente por HTTPS. Las claves que estén escritas dentro del HTML pueden ser vistas por cualquier visitante; restringe la clave de Google Maps por HTTP referrer y API, o retírala antes de publicar.
- La cartografía y los datos meteorológicos dependen de servicios externos; publicar en GitHub Pages no garantiza que esos servicios respondan siempre.
- Esta entrega corrige el estado visible de arranque/respaldo y prepara la estructura de publicación. No se ha podido verificar desde este entorno la carga real de los servicios cartográficos en un navegador con conexión.
