# Proteínas Colombia Team — Onboarding web para embajadores

Material para el programa de embajadores de Proteínas Colombia, basado en
los dos documentos que envió la tienda (Kit de Bienvenida y Reglamento
Oficial). El entregable acordado es la versión web; sin fotografías, por
decisión del cliente.

## Contenido

| Archivo | Qué es |
|---|---|
| `web/kit-embajadores.html` | Kit de Bienvenida: página autocontenida (fuentes incrustadas) con el generador de código de embajador y botones de WhatsApp e Instagram. |
| `web/reglamento.html` | Reglamento Oficial: página independiente con las 12 reglas desplegables, contador de lectura y contacto propio. |

Ambas páginas son estáticas y autocontenidas — se publican copiando los
archivos a cualquier hosting (Netlify, Vercel, Cloudflare Pages) sin
dependencias externas.

## Antes de publicar la versión final

- Agregar `<meta name="robots" content="noindex">` para que el link no
  aparezca en buscadores (solo lo conoce quien lo recibe).
- Quitar el pie «Boceto de diseño — versión interactiva».
- Opcional: botón «Lee el reglamento» al final del Kit apuntando a
  `reglamento.html` (enlace relativo, funciona una vez alojadas juntas).

## Pendiente con la tienda

- Fecha de entrega esperada.

Las versiones anteriores en PDF de diapositivas (y su fuente HTML/CSS)
están disponibles en el historial de git si se llegaran a necesitar.
