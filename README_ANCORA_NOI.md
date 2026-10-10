# Ancora Noi — landing en italiano

La página está en `ancora-noi/index.html`. Se preparó a partir del HTML proporcionado por el propietario del producto. La guía y los bonos de pago no se incluyen en esta carpeta pública.

## Estado

- La VSL usa el MP4 público de Cloudinary que ya aparece en el HTML proporcionado.
- Las imágenes de portada están integradas en el HTML como WebP.
- La compra queda deshabilitada hasta completar `CONFIG.checkoutUrl`.
- Los enlaces legales vacíos quedan ocultos, y el borrador lleva `noindex,nofollow`.

## Datos pendientes antes de publicar

En el bloque `CONFIG` al final de `ancora-noi/index.html`, completar:

1. `checkoutUrl` con la URL de pago de Ancora Noi.
2. Precio y moneda, confirmando el valor de `€15` del borrador.
3. Días y condiciones reales de la garantía.
4. `supportEmail`, `legalName`, `privacyUrl`, `termsUrl` y `cookieUrl`.
5. Fecha real de fin de oferta, solo si existe. Sin fecha no se muestra el contador.

Después de completar y verificar esos datos, quitar la etiqueta `<meta name="robots" content="noindex,nofollow">`.

## Publicación en la ruta solicitada

La landing se publicó en `https://legadosalud.com/ancora-noi/` mediante Netlify Drop en el proyecto que ya sirve `legadosalud.com`. El paquete desplegado conserva todos los archivos de la versión anterior del portal y añade `ancora-noi/index.html`.

Este repositorio guarda el código fuente de la landing, pero **no está conectado al despliegue de Netlify**. Los cambios futuros deben incorporarse al paquete completo del portal y volver a subirse al mismo proyecto, o configurar una integración Git que incluya todos los archivos del portal.

El repositorio original `ramiaguero/prompt-infoproducto-seguro-netlify` solo contenía documentación cuando se clonó. No contenía el código fuente del portal Legado Salud. Por eso la landing se preparó aquí como carpeta independiente.
