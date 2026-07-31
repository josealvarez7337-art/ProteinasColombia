# Proteínas Colombia Team — Onboarding web para embajadores

Sitio web del programa de embajadores de Proteínas Colombia: Kit de
Bienvenida y Reglamento Oficial. Versión final aprobada por el cliente
(sin fotografías, diseño plano, interactividad conservada).

## Contenido

| Archivo | Qué es |
|---|---|
| `web/index.html` | Kit de Bienvenida (página principal): generador de código de embajador, botones de WhatsApp e Instagram y enlace al reglamento. |
| `web/reglamento.html` | Reglamento Oficial: las 12 reglas desplegables con contador de lectura, contacto y enlace de regreso al kit. |
| `web/catalogo.pdf` | Catálogo de productos de la tienda (9 páginas). Se publica junto al sitio; el botón «Catálogo de productos» del cierre del Kit lo abre. |

Ambas páginas son estáticas y 100 % autocontenidas (fuentes incrustadas,
sin dependencias externas). Incluyen `noindex` para no aparecer en
buscadores, `viewport` para móvil y el isotipo de la marca como favicon, que alterna
entre la versión clara y la oscura según el tema del navegador (más
`apple-touch-icon` para cuando se agrega a la pantalla de inicio).

## Cómo publicar (Netlify, gratis)

1. Crear cuenta en netlify.com (con el correo del diseñador, que mantiene el sitio).
2. En "Sites", arrastrar la carpeta `web/` completa (o el ZIP con ambos archivos).
3. En "Site configuration → Change site name", poner `proteinascolombiateam`
   → queda publicado en `https://proteinascolombiateam.netlify.app`.
4. El Reglamento queda automáticamente en `/reglamento.html`.

Para actualizar (cambio de reglas, comisiones, etc.): editar el archivo
correspondiente y volver a arrastrar la carpeta — el link no cambia.

## Marca

| Archivo | Qué es |
|---|---|
| `brand/logo-original.jpg` | Logo tal como lo entregó la tienda (JPEG con fondo oscuro). |
| `brand/logo-master-2x.png` | Máster reconstruido: fondo transparente, blanco puro sin ruido de compresión, 1878×400. Es la versión incrustada en el encabezado de las páginas. |
| `brand/isotipo-original-claro.jpg` · `brand/isotipo-original-oscuro.jpg` | Isotipos tal como los entregó la tienda (JPEG). |
| `brand/isotipo-negro.svg` · `brand/isotipo-blanco.svg` | Isotipos vectorizados con fondo transparente — la versión negra para fondos claros y la blanca para fondos oscuros. Son las que van incrustadas como favicon. |
| `brand/isotipo-negro.png` · `brand/isotipo-blanco.png` | Los mismos isotipos rasterizados a 2048 px, para formatos que no admiten SVG.

## Acuerdo de mantenimiento

Actualizaciones de contenido se cobran por ronda de cambios, con entrega
en 48 horas, según lo acordado con el cliente.
