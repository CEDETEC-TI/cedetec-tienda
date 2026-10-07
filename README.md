# CEDETEC Tienda — iPhone, Mac y accesorios

Página de [CEDETEC](https://cedetec-ti.github.io/cedetec-sistema/) para vender iPhone, Mac, AirPods y accesorios Apple originales en Formosa, con una estética inspirada en apple.com.

A diferencia de las demás carpetas de este workspace (BAMBAM, RESTAURANTE, etc.), **esto no es una demo de un negocio ficticio**: es una página real de CEDETEC, con su WhatsApp e Instagram reales.

CEDETEC revende productos Apple originales como revendedor independiente. **No es Apple Inc. ni un Apple Store oficial** — esa aclaración está en el pie de página del sitio.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build ni backend), con estética inspirada en apple.com:

- Portada con el iPhone 18 Pro como protagonista, nav flotante traslúcida y tipografía del sistema (-apple-system).
- Catálogo de **iPhone** con los **19 modelos y colores** que el proveedor tiene en stock ahora mismo, nuevos y usados (desde iPhone 13 usado hasta iPhone 18 Pro Max), cada uno con su color real, su etiqueta "Nuevo" o "Usado · SWAP" y un **buscador** arriba de la grilla para filtrar por modelo, color o condición (ej. "17 Pro", "14", "usado"). Los datos de los 19 iPhones viven en un array de JS (`IPHONES`) dentro de `index.html`, fácil de editar a mano cuando cambie el stock. Sección de **Mac** (MacBook Air y MacBook Pro, en beats a pantalla completa como los de apple.com) y grilla de **AirPods y accesorios** (AirPods Pro 3, cargador MagSafe, adaptador 20W, cable USB-C y funda transparente con MagSafe), estos últimos sin precio fijo.
- Todas las fotos son reales, tomadas de las páginas e imágenes oficiales de apple.com (CDN `store.storeimages.cdn-apple.com`) y del newsroom de Apple, recortadas para que el producto llene el cuadro y verificadas una por una antes de publicar. Los colores de cada variante son los reales del proveedor; cuando varias variantes del mismo modelo comparten la misma foto base de Apple (por ejemplo, los 4 colores del iPhone 13 usado), es porque Apple no publica una foto "compare" distinta por color para ese modelo. El iPhone 18 Pro Max y el 17 Pro Max reutilizan la foto del 18 Pro y el 17 Pro (mismo diseño). No se encontró una foto oficial verificable del iPhone 11 Pro CPO porque Apple ya no lo lista en ningún lado de su sitio (ni nuevo ni refurbished), así que ese modelo no se incluyó.
- **Precios de iPhone**: se calculan tomando el precio en USD del proveedor real de CEDETEC ([vencellalberdi.com](https://vencellalberdi.com)) para cada variante (modelo + color + condición) que tiene en stock, más 10%. El precio que se muestra en cada tarjeta es el final, lo que paga el cliente — no hay que consultar nada aparte. **Mac y accesorios no muestran precio** ("Consultar precio" / botón "Consultar"): el proveedor de iPhones no los tiene en su catálogo, así que no hay un costo real verificado para calcular el 10%.
- Franja de confianza (productos originales nuevos o usados, equipos revisados y aclarados antes de comprar, entrega en Formosa, asesoramiento) y sección de contacto con WhatsApp e Instagram reales de CEDETEC.

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages, Netlify o Vercel apuntando a la raíz del repo. Publicado en https://cedetec-ti.github.io/cedetec-tienda/
