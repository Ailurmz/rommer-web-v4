# Rommer: prototipo navegable (etapa 1)

Prototipo en HTML/CSS/JS de la **Home**, la **Ficha de producto** y el **Changuito (drawer)**, para aprobar el diseño antes de pasarlo a WordPress.

## Cómo verlo
Todo funciona sin internet: las librerías y las fuentes están dentro de la carpeta.

Lo más fácil es abrirlo con un servidor local desde esta carpeta:

```bash
python3 -m http.server 8000
```

Después entrá a http://localhost:8000. También funciona con doble clic en `index.html`.

## Qué incluye
- `index.html`: Home con las 18 secciones del brief.
- `producto.html?id=shampoo-keratin`: Ficha de producto. Cambiando el `id` se ven los otros productos.
- `assets/css/rommer.css`: tokens de marca (colores, tipografías, radios) y todos los estilos.
- `assets/js/rommer.js`: catálogo de ejemplo, carrito, carruseles y animaciones.
- `vendor/`: GSAP 3.12.5, ScrollTrigger, Lenis 1.1.13 y Swiper 11.1.14.

## Qué funciona en el prototipo
- Preloader con el logo real letra por letra (una vez por sesión).
- Hero con el wordmark gigante que se "derrite" con el scroll y stickers con parallax.
- Marquees y cintas cruzadas.
- Carruseles arrastrables con barra de progreso con la "r".
- Mega-menú, menú mobile y buscador predictivo.
- Método Rommer fijo con el scroll en desktop.
- Pestañas que recolorean el envase.
- Slider antes/después.
- Changuito con:
  - barra de envío gratis;
  - descuento automático de kit (3 productos = 15%, 4 o más = 20%);
  - sugerencias de "Completá tu rutina";
  - cuotas.
- Ficha de producto con:
  - galería con zoom;
  - tamaños "Para casa / Tamaño salón";
  - calculadora de envío;
  - acordeones;
  - "Agregar rutina completa";
  - reseñas;
  - relacionados;
  - barra de compra fija en el celular.
- Cursor con la "r", botón de WhatsApp y respeto de "movimiento reducido".

## Placeholders (a reemplazar)
| Qué | Hoy | Necesito |
|---|---|---|
| Tipografía display | Fredoka (parecida a Blur) | Archivo **Blur** (.woff2/.otf) + licencia web |
| Stickers | Redibujados en SVG a partir del PDF | Stickers originales en **SVG** |
| Logo | Recortado del PDF | Logo e isotipo en **SVG** |
| Envases de otros productos | Envase rosa real recoloreado | Fotos de cada producto con fondo transparente |
| Catálogo | 9 productos y precios **inventados** | Listado real: nombre, línea, tamaños, precios, descripción, INCI |
| Antes/después | Misma foto con filtro | Fotos reales de antes y después |
| Video | Foto de la campaña | Video de campaña |
| Colores | Tomados del PDF | Hex exactos del manual de marca |
| Datos | Envío gratis desde $50.000, WhatsApp de ejemplo | Monto real, número de WhatsApp, redes |

## Próximas etapas
2. Paso a WordPress: tema hijo de Hello Elementor + plantillas de Elementor + WooCommerce.
3. Guía de instalación en Hostinger.
