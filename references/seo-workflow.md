# Referencias operativas de Indexa

Origen del flujo: [reel de Luis Álvarez Web](https://www.facebook.com/reel/2098623907436804), descripción completa consultada el 29 de octubre de 2026. Sus cuatro acciones son verificar Search Console, enviar sitemap, solicitar indexación de páginas importantes e importar en Bing. La implementación usa documentación oficial vigente; el reel no garantiza indexación ni un plazo.

## Search Console y propiedad

- [Añadir una propiedad](https://support.google.com/webmasters/answer/34592?hl=es): una propiedad de dominio cubre protocolos/subdominios; una de prefijo de URL se limita al prefijo. No tramites automáticamente hosts administrativos sólo porque existe una propiedad de dominio.
- [Verificar la propiedad](https://support.google.com/webmasters/answer/9008080?hl=es): métodos, condiciones y conservación de la prueba. Un archivo/etiqueta puede requerir que la página sea accesible públicamente; DNS permite verificar sin abrir una demo. Preserva tokens previos y usa el valor exacto mostrado por Search Console.
- [Search Console](https://search.google.com/search-console): selecciona cuenta y propiedad antes de enviar algo. Registra el resultado del proveedor, no sólo que existe un TXT o archivo.

## Sitemap y exclusiones

- [Crear y enviar sitemap](https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap?hl=es): lista URLs preferidas, absolutas y canónicas. Un índice de sitemaps válido también sirve. El envío ayuda al descubrimiento, pero no obliga a Google a rastrear ni indexar.
- [Bloquear la indexación con noindex](https://developers.google.com/search/docs/crawling-indexing/block-indexing?hl=es): Google necesita rastrear para ver `noindex`; bloquear en robots puede impedirlo. Mantén autenticación para contenido privado. No publiques contenido sensible con la expectativa de que robots lo proteja.
- [Introducción a robots.txt](https://developers.google.com/search/docs/crawling-indexing/robots/intro?hl=es): comprueba el archivo del host concreto. No asumas que reglas del dominio raíz protegen subdominios.

## Solicitud de indexación

- [Inspección de URL](https://support.google.com/webmasters/answer/9012289?hl=es): el informe del índice y la prueba en vivo responden preguntas diferentes. Registra estado y URL exacta. Una solicitud tiene cuotas y no prueba inclusión en resultados.
- No uses la Indexing API como sustituto general de la inspección/sitemap de un sitio ordinario.

## Bing

- [Añadir y verificar un sitio](https://www.bing.com/webmasters/help/add-and-verify-site-12184f8b?action=learn&source=helpdocvnext&type=verificationtrouble): importación desde Search Console o verificación manual por archivo XML, etiqueta o DNS.
- [Bing Webmaster Tools](https://www.bing.com/webmasters/): revisa la cuenta actual y selecciona sólo el sitio solicitado. La conexión puede revalidar propiedad e importar nuevos sitemaps periódicamente. Los permisos exactos los establece el consentimiento real; elegir un sitio no garantiza que OAuth esté limitado a ese sitio.

## Registro mínimo sugerido

| Paso | Estado | Evidencia | Siguiente acción |
|---|---|---|---|
| Propiedad Google | Hecho / pendiente / bloqueado | Tipo y prefijo, resultado de verificación | Acción exacta |
| Sitemap | Hecho / pendiente / bloqueado | URL, HTTP y estado del proveedor | Acción exacta |
| Inspección/indexación | Hecho / pendiente / bloqueado | URLs públicas y estado observado | Acción exacta |
| Bing | Hecho / pendiente / bloqueado | Propiedad y sitemap confirmados | Acción exacta |

En un bloqueo de publicación, conserva pendientes los pasos dependientes y ofrece la corrección concreta más pequeña. En un bloqueo de cuenta, conserva preparados dominio, sitemap y URLs sin registrar secretos ni ampliar el alcance.
