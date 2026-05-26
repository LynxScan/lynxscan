# Landing LynxScan · Contexto

Landing comercial de **LynxScan Technology** — sistemas de escaneo industrial 2D/3D para aserraderos y madera transformada. Material fuente: folletos `LYNXSCAN_ES.pdf` y `LYNXSCAN_EN.pdf` en `recursos/`.

## Stack

Caso A de la skill `landing-pages-pro`: single file (HTML + CSS + JS inline). Sin backend, sin formulario — contacto directo por teléfono y email.

```
landing-lynxscan/
├── index.html        Single-file (HTML + CSS + JS i18n)
├── assets/           Logo + 8 fotos extraídas de los folletos
├── recursos/         PDFs originales ES/EN + logo fuente
└── contexto.md       Este archivo
```

## Identidad visual

Tomada del folleto:
- **Sage / verde-gris**: `#9CAA94` (fondo hero, sectores), `#6F7E68` (oscuro), `#C7D1BF` (claro)
- **Amarillo Lynx**: `#F4D81C` (acento), `#D9BE00` (oscuro para títulos en blanco)
- **Oscuro**: `#1F2420`
- **Tipografía**: Barlow Condensed (títulos) + Inter (cuerpo). Misma que landing BotLynx.

## Estructura

1. Header sticky con switch ES/EN
2. Hero — "Escanea · Optimiza · Crece" con render del LS-501
3. Valor (4 cards) — Trazabilidad / Automatización / Visibilidad / Beneficio
4. Sectores — Aserraderos + Madera Transformada
5. Productos — LS-501-PRO (featured con foto) + LS-301-PRO + LS-201-PRO
6. Software — Captura ScanWood + lista features
7. **BotLynx** — sección verde con mockup de chat Telegram, link a `https://bittingenieria.github.io/botlynx/`
8. Galería — 6 fotos en producción
9. Why LynxScan (4 razones)
10. CTA final — tel + email
11. Footer

## i18n

JS inline con objeto `I18N` (es/en). Botones ES/EN en header. Estado persistido en `localStorage`. Default: detecta `navigator.language` o cae en ES.

Todos los textos con `data-i18n="key"`. Añadir nuevo texto = añadir clave en ambos diccionarios.

## Contacto (igual en ambos idiomas)

- **Tel**: +34 607 30 62 19
- **Email**: electronica@lynxscan.com
- **Dirección**: Av. Santander 157, 34880 Guardo, Palencia (Spain)

## Gama de productos

| Modelo | Tipo | Destacado |
|---|---|---|
| **LS-501-PRO** | Escáner multi-cara con optimización de corte | 6 caras, 120 m/min, 1200-6500 mm, defectos geom+bio |
| **LS-301-PRO** | Escáner 3D de troncos | Volumen 3D, diámetros, curvatura, conicidad |
| **LS-201-PRO** | Cubicador 2D | Volumen 2D, longitud, conteo, expulsores |

## BotLynx · integración

Sección dedicada con mockup de chat Telegram. Link directo a `https://bittingenieria.github.io/botlynx/`. Mensaje:
- IA local · datos no salen del aserradero
- Consultas en lenguaje natural
- Alertas si la línea cae
- Informe mensual PDF (Telegram + email)
- Llave en mano

## Publicación

- **URL pública**: https://lynxscan.github.io/lynxscan/
- **Repo**: https://github.com/LynxScan/lynxscan (cuenta `LynxScan`, propia, separada de `bittingenieria`)
- **Para actualizar**: editar `index.html` o `assets/`, luego `git add -A && git commit -m "..." && git push`. Pages republica en ~30-60 s.

## Estado · 2026-05-26

- Folletos ES + EN leídos, info y fotos extraídas
- 8 fotos curadas en `assets/` (escáner exterior, interior, render, software UI, panel control, troncos, línea, escáner con troncos)
- Logo: `assets/logo.png` (de `recursos/logo_lynx.png`)
- `index.html` completo, single-file, biling�e ES/EN funcional
- Probada localmente en navegador
- Repo `LynxScan/lynxscan` creado y publicado en https://lynxscan.github.io/lynxscan/ — 200 OK
