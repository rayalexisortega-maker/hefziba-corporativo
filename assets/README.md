# Assets — Hefzi-bá Corporativo

La página **detecta los archivos automáticamente**. Deja caer el logo con el nombre y ruta exactos de abajo, recarga el navegador, y aparece solo. Mientras no exista, se muestra un monograma "H" temporal (no rompe nada).

## Estructura

```
assets/
├── logo/
│   ├── logo.svg        ← logotipo horizontal (navbar + footer)
│   └── isotipo.svg     ← símbolo cuadrado (tarjeta del hero)
├── favicon/
│   ├── favicon.svg     ← ícono de pestaña (recomendado SVG)
│   ├── favicon.png     ← respaldo 32×32 px
│   └── apple-touch-icon.png  ← 180×180 px (iOS)
├── social/
│   └── og-image.jpg    ← al compartir en WhatsApp/Facebook (1200×630 px)
└── img/                ← fotos de equipo/oficina (opcional, uso futuro)
```

## Qué poner en cada uno

| Archivo | Dónde se usa | Recomendación |
|---|---|---|
| `logo/logo.png` | Tarjeta del hero **y** animación de intro | Logotipo completo (símbolo + nombre). **Ya está puesto.** ✅ |
| `logo/isotipo.svg` **o** `isotipo.png` | **Navbar y footer** | Solo el símbolo "H", cuadrado, **fondo transparente**. La página prueba `.svg`, luego `.png`, y si no existe usa el monograma azul temporal. |
| `favicon/favicon.png` | Pestaña del navegador | Cuadrado, recorte del símbolo, legible en 16 px. (Hoy usa `logo.png`.) |
| `social/og-image.jpg` | Vista previa al compartir link | 1200×630 px, con logo + tagline. |
| `img/equipo-1.jpg` … `equipo-8.jpg` | **Carrusel del hero** | Fotos del equipo. Nómbralas en orden; las que no existan se descartan solas. Horizontal 5:4 se ve mejor. |

## Notas

- **Formato:** el HTML apunta a `.svg`. Si tu archivo es PNG/JPG, o lo renombras (`logo.svg`) o cambias la extensión en `index.html` (busca `assets/logo/`).
- **El logo horizontal ya incluye el nombre "HEFZI-BÁ Corporativo"?** Entonces borra el `<span>HEFZI-BÁ<small>Corporativo</small></span>` que está junto a la imagen en el navbar y el footer, para no duplicar el texto.
- Los archivos `.gitkeep` en cada carpeta solo mantienen las carpetas vacías en git — puedes ignorarlos.
