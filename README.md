# CEDETEC Tienda — iPhone, Mac y accesorios

Página de [CEDETEC](https://cedetec-ti.github.io/cedetec-sistema/) para vender iPhone, Mac, AirPods y accesorios Apple originales en Formosa, con una estética inspirada en apple.com.

A diferencia de las demás carpetas de este workspace (BAMBAM, RESTAURANTE, etc.), **esto no es una demo de un negocio ficticio**: es una página real de CEDETEC, con su WhatsApp e Instagram reales.

CEDETEC revende productos Apple originales como revendedor independiente. **No es Apple Inc. ni un Apple Store oficial** — esa aclaración está en el pie de página del sitio.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build ni backend), con estética inspirada en apple.com:

- Portada con el iPhone 18 Pro como protagonista, nav flotante traslúcida y tipografía del sistema (-apple-system).
- Catálogo de **iPhone** con los 9 modelos que el proveedor tiene en stock, nuevos y usados (18 Pro, 18 Pro Max, 17 Pro, 17 Pro Max, 16, 15, 14 nuevo, 14 usado y 13 usado), cada uno con una etiqueta "Nuevo" o "Usado · SWAP". Sección de **Mac** (MacBook Air y MacBook Pro, en beats a pantalla completa como los de apple.com) y grilla de **AirPods y accesorios** (AirPods Pro 3, cargador MagSafe, adaptador 20W, cable USB-C y funda transparente con MagSafe), estos últimos sin precio fijo.
- Todas las fotos son reales, tomadas de las páginas e imágenes oficiales de apple.com (CDN `store.storeimages.cdn-apple.com`) y del newsroom de Apple, recortadas para que el producto llene el cuadro y verificadas una por una antes de publicar. El iPhone 18 Pro Max y el 17 Pro Max reutilizan la foto del 18 Pro y el 17 Pro (mismo diseño); no se encontró una foto oficial verificable del iPhone 11 Pro CPO porque Apple ya no lo lista en ningún lado de su sitio (ni nuevo ni refurbished), así que ese modelo no se incluyó.
- **Precios de iPhone**: se calculan tomando el precio en USD del proveedor real de CEDETEC ([vencellalberdi.com](https://vencellalberdi.com)) para cada modelo que tiene en stock (nuevo o usado/SWAP), más 10%. El precio que se muestra en cada tarjeta es el final, lo que paga el cliente — no hay que consultar nada aparte. Cuando un modelo tenía varios colores en stock a precios ligeramente distintos, se tomó el más bajo. **Mac y accesorios no muestran precio** ("Consultar precio" / botón "Consultar"): el proveedor de iPhones no los tiene en su catálogo, así que no hay un costo real verificado para calcular el 10%.
- Franja de confianza (productos originales nuevos o usados, equipos revisados y aclarados antes de comprar, entrega en Formosa, asesoramiento) y sección de contacto con WhatsApp e Instagram reales de CEDETEC.

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages, Netlify o Vercel apuntando a la raíz del repo. Publicado en https://cedetec-ti.github.io/cedetec-tienda/
