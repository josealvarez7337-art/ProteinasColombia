# Proteínas Colombia Team — Bocetos de onboarding para embajadores

Material de propuesta para el programa de embajadores de Proteínas Colombia,
basado en los dos documentos que envió la tienda (Kit de Bienvenida y
Reglamento Oficial).

## Contenido

| Carpeta | Qué hay |
|---|---|
| `entregables/` | Los dos PDF de diapositivas verticales (540×960, formato celular/WhatsApp): Kit de Bienvenida (10 diapositivas) y Reglamento Oficial (8 diapositivas). |
| `diapositivas/` | Fuente de los PDF: HTML + CSS compartido (`slides.css`) con las fuentes Anton y Barlow en `fuentes/`. |
| `web/` | Versión web interactiva (un solo archivo, fuentes incrustadas): generador de código de embajador, reglamento con contador de lectura y botón de WhatsApp. |

## Cómo regenerar los PDF

Cada archivo HTML de `diapositivas/` se imprime a PDF con Chromium sin
márgenes, página de 540×960 px y fondos activados:

```python
await page.goto("file://.../kit-slides.html")
await page.pdf(path="salida.pdf", width="540px", height="960px",
               print_background=True,
               margin={"top": "0", "right": "0", "bottom": "0", "left": "0"})
```

## Pendientes con la tienda

- Fotos propias (los espacios marcados «FOTO — …» son marcadores intencionales).
- Fecha de entrega esperada.
