# CEDETEC Tienda — iPhone, Mac y accesorios

Página de [CEDETEC](https://cedetec-ti.github.io/cedetec-sistema/) para vender iPhone, Mac, AirPods y accesorios Apple originales en Formosa, con una estética inspirada en apple.com.

A diferencia de las demás carpetas de este workspace (BAMBAM, RESTAURANTE, etc.), **esto no es una demo de un negocio ficticio**: es una página real de CEDETEC, con su WhatsApp e Instagram reales.

CEDETEC revende productos Apple originales como revendedor independiente. **No es Apple Inc. ni un Apple Store oficial** — esa aclaración está en el pie de página del sitio.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build ni backend), con estética inspirada en apple.com:

- Portada con el iPhone 18 Pro como protagonista, nav flotante traslúcida y tipografía del sistema (-apple-system).
- Catálogo de **iPhone** con los **97 modelos, colores y condiciones** que figuran en el catálogo completo del proveedor (esté o no marcado "Agotado" ahí: como el visitante de la página no tiene acceso a la web del proveedor, ve el catálogo completo de lo que CEDETEC puede conseguir, no solo el stock exacto de este instante), desde iPhone 13 hasta iPhone 18 Pro Max. Cada tarjeta muestra el color real, el almacenamiento y una etiqueta de condición ("Nuevo", "Usado", "Reacondicionado (CPO)" o "Semi nuevo"), más un **buscador** arriba de la grilla para filtrar por modelo, color o condición (ej. "17 Pro", "14", "cpo", "usado"). Para que la grilla no abrume con 97 tarjetas de una, por defecto se muestran solo 8 y un botón "Ver 8 modelos más" va revelando el resto de a 8; al buscar algo, se muestran todos los resultados que coincidan sin el límite. Los datos de los 97 iPhones viven en un array de JS (`IPHONES`) dentro de `index.html`, generado a partir del catálogo del proveedor y fácil de volver a generar cuando cambien los precios. Sección de **Mac** (MacBook Air y MacBook Pro, en beats a pantalla completa como los de apple.com) y grilla de **AirPods y accesorios** (AirPods Pro 3, cargador MagSafe, adaptador 20W, cable USB-C y funda transparente con MagSafe), estos últimos sin precio fijo.
- Todas las fotos son reales, tomadas de las páginas e imágenes oficiales de apple.com (CDN `store.storeimages.cdn-apple.com`), recortadas para que el producto llene el cuadro y verificadas una por una antes de publicar. Los colores de cada variante son los reales del proveedor; cuando varias variantes del mismo modelo comparten la misma foto base de Apple (por ejemplo, los 4 colores del iPhone 13 usado), es porque Apple no publica una foto "compare" distinta por color para ese modelo. Los modelos Pro Max (13 a 18) reutilizan la foto de su versión Pro, porque Apple tampoco publica una foto "compare" separada para el Max (mismo diseño, distinto tamaño). No se encontró una foto oficial verificable del iPhone 11 Pro CPO porque Apple ya no lo lista en ningún lado de su sitio (ni nuevo ni refurbished), así que ese modelo no se incluyó.
- **Precios de iPhone**: se calculan tomando el precio en USD de cada variante (modelo + color + condición) del catálogo completo del proveedor real de CEDETEC ([vencellalberdi.com](https://vencellalberdi.com)), más 10%. El precio que se muestra en cada tarjeta es el final, lo que paga el cliente — no hay que consultar nada aparte. **Mac y accesorios no muestran precio** ("Consultar precio" / botón "Consultar"): el proveedor de iPhones no los tiene en su catálogo, así que no hay un costo real verificado para calcular el 10%.
- Franja de confianza (productos originales nuevos o usados, equipos revisados y aclarados antes de comprar, entrega en Formosa, asesoramiento) y sección de contacto con WhatsApp, Instagram y TikTok reales de CEDETEC.

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages apuntando a la raíz del repo. Publicado en https://cedetec-ti.github.io/cedetec-tienda/
