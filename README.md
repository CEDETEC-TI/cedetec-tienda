# NOVA (demo)

Sitio de una sola página para "NOVA", tienda de tecnología ficticia en Formosa Capital, Argentina, que vende iPhone, Mac, AirPods y accesorios Apple originales. Pieza de demo/portfolio de [CEDETEC Digital](https://cedetec-ti.github.io/cedetec-sistema/), pensada como caso representativo para prospección en el rubro de venta de tecnología, con una estética inspirada en apple.com.

No representa un negocio real: nombre, dirección, teléfono y contenido son de ejemplo. Repo y sitio completamente independientes de otros proyectos de demo del portfolio: no comparten código, carpeta ni historial.

**NOVA no es Apple Inc. ni un Apple Store oficial.** Es una tienda ficticia que vendería productos Apple genuinos como revendedor independiente (un modelo real y común, equivalente a un "Apple Premium Reseller"). El sitio no usa el logo ni la marca de Apple como identidad propia; la marca del sitio es "NOVA". El pie de página incluye el disclaimer correspondiente.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build ni backend), con estética inspirada en apple.com:

- Portada con el iPhone 18 Pro como protagonista, nav flotante traslúcida y tipografía del sistema (-apple-system).
- Catálogo de **iPhone** (18 Pro, Air, 17 y 16), sección de **Mac** (MacBook Air y MacBook Pro, en beats a pantalla completa como los de apple.com) y grilla de **AirPods y accesorios** (AirPods Pro 3, cargador MagSafe, adaptador 20W, cable USB-C y funda transparente con MagSafe).
- Todas las fotos son reales, tomadas de las páginas e imágenes oficiales de apple.com (CDN `store.storeimages.cdn-apple.com`) y del newsroom de Apple, verificadas una por una antes de publicar.
- Precios: se muestra el precio de lista oficial en USD de Apple EE.UU. como referencia, y se invita a consultar el precio final en pesos por WhatsApp (varía por importación y tipo de cambio). No se inventaron precios en pesos.
- Franja de confianza (productos originales, garantía oficial, entrega en Formosa, asesoramiento) y sección de contacto con WhatsApp.

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages, Netlify o Vercel apuntando a la raíz del repo.
