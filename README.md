# Proteínas Colombia Team — Bocetos de onboarding para embajadores

Material de propuesta para el programa de embajadores de Proteínas Colombia,
basado en los dos documentos que envió la tienda (Kit de Bienvenida y
Reglamento Oficial).

## Contenido

| Carpeta | Qué hay |
|---|---|
| `entregables/` | Los dos PDF de diapositivas verticales (540×960, formato celular/WhatsApp): Kit de Bienvenida (10 diapositivas) y Reglamento Oficial (8 diapositivas). |
| `diapositivas/` | Fuente de los PDF: HTML + CSS compartido (`slides.css`) con las fuentes Anton y Barlow en `fuentes/`. |
| `web/` | Versión web (dos archivos independientes, fuentes incrustadas): `kit-embajadores.html` con el generador de código, y `reglamento.html` con las 12 reglas desplegables y contador de lectura. |

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

- El cliente decidió el material sin fotografías; los diseños son tipográficos.
- Fecha de entrega esperada.
