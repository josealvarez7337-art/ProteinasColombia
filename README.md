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

### Opción A — arrastrar el ZIP (lo más rápido, desde un computador)

1. Entrar a **app.netlify.com/drop** y crear la cuenta (con el correo del
   diseñador, que es quien mantiene el sitio).
2. Arrastrar el ZIP del sitio al recuadro punteado. Netlify lo descomprime
   solo; los tres archivos deben quedar en la raíz del ZIP, sin carpeta
   que los envuelva.
3. Queda publicado en una dirección aleatoria del tipo
   `brave-panda-4821.netlify.app`. Para cambiarla:
   **Site configuration → General → Change site name** → escribir
   `proteinascolombiateam` → queda
   `https://proteinascolombiateam.netlify.app`.
4. El Reglamento queda en `/reglamento.html` y el catálogo en
   `/catalogo.pdf`. El certificado HTTPS lo pone Netlify solo.

Para actualizar: **Deploys → Drag and drop your site folder** y soltar el
ZIP nuevo. La dirección no cambia, así que los embajadores que ya tienen
el enlace ven la versión nueva sin que haya que reenviarles nada.

### Opción B — conectar el repositorio (se actualiza solo)

Sirve también desde el celular y evita volver a arrastrar archivos: en
**Add new site → Import an existing project → GitHub**, elegir este
repositorio y configurar

- Branch: la rama de trabajo
- Build command: *(vacío)*
- Publish directory: `web`

Con eso, cada cambio que se suba al repositorio se publica solo.

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
