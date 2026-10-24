# HANDOFF — Landing Jay Personal Brand

Documento de traspaso. Léelo completo antes de empezar a trabajar en esta carpeta.

---

## Qué es este proyecto

Construir una landing page en HTML puro (un solo archivo autocontenido) para vender un producto digital de $17: un sistema de creación de guiones virales en Notion.

**Marca:** Jay Personal Brand
**Dominio:** jaypersonalbrand.com
**Nota:** el proyecto se llamaba antes "mrnotion.shop". Ese nombre está descartado. Si aparece en algún archivo viejo, reemplázalo por Jay Personal Brand.

Existe una versión previa de la página hecha en ClickFunnels. La reemplazamos por HTML propio.

---

## Decisiones ya cerradas (no volver a preguntar)

| Punto | Decisión |
|---|---|
| Precio | $17 USD, pago único |
| Valor total del stack | $358 |
| Ganchos | 50 (no "+100") |
| Prueba social | +1250 profesionales |
| Garantía | No hay. No inventar ninguna. |
| Checkout | Hotmart. URL todavía no existe: usar placeholder. |
| Plataforma de entrega | Notion (funciona con cuenta gratuita) |

---

## El producto

**Core — Sistema de Guiones Virales en Notion ($197)**
- 12 plantillas de guiones en 3 categorías: vender, autoridad, conversación
- 50 ganchos virales
- Un prompt de IA por plantilla
- Banco de referentes con la regla 10×10 (10 creadores × sus 10 videos más vistos = 100 ideas)
- Calendario de publicación y tracker de resultados

El core cierra su ciclo en: **guion terminado, con tu voz, listo para grabar.**
Esto es importante. Los bonos solo se leen como regalo si el core ya está completo antes de que aparezcan.

**Bonos**
- Bonus 1 — Del guion a la cámara ($67). No existe todavía, hay que grabarlo.
- Bonus 2 — Edición mínima viable ($47). No existe todavía, hay que grabarlo.
- Bonus 3 — Masterclass: 30 días de contenido en menos de 1 hora ($47). Ya existe.

---

## Sistema visual (congelado)

**Color**
```
--marker:     #F7C429   /* amarillo único: botones, subrayadores, checklist, glow del video */
--ink:        #17171C   /* tinta */
--testi-bg:   #000000   /* fondo sección testimonios */
--testi-card: #141416   /* cajas de testimonios */
```
Se unificó a un solo amarillo. El `#E0AE18` que se barajó antes quedó descartado.

**Tipografía**
- Montserrat, familia única en toda la página
- Titulares: peso 900
- Cuerpo: 400 / 500
- Énfasis: 600 / 700
- Inter y Archivo están fuera del proyecto

**Formas**
- Botones rectangulares con esquinas suaves (~8px). Nunca píldora.
- Fondo de botón `#F7C429`, texto negro.

**Efectos**
- El video del hero lleva un resplandor amarillo alrededor. Sutil, no neón.

**Sin barra superior negra.** Se eliminó.

---

## Estructura de la página (12 secciones)

1. Hero — eyebrow con punto amarillo + "+1250 profesionales ya confían en nuestro producto", VSL con glow, CTA
2. ¿Esto es para ti? — identificación
3. Por qué no es tu culpa — reencuadre
4. Qué es exactamente el sistema — el tour de los 4 espacios → **CTA**
5. Mecanismo 1: banco de referentes (regla 10×10) → testimonio Clara A
6. Mecanismo 2: la plantilla escribe por ti → testimonio Seul C → **CTA**
7. Prueba de nicho — comparativo lado a lado
8. Resultados — 4 testimonios sobre fondo negro → **CTA**
9. Todo lo que incluye — core primero, luego los 3 bonos
10. Precio — $358 tachado → $17 + argumento del porqué → **CTA**
11. FAQ — 6 preguntas, van DESPUÉS del precio
12. Cierre — contraste + **CTA final**

Son 7 botones en total (los 5 marcados arriba + barra fija móvil + hero).
Todos apuntan a la misma variable de checkout.

**El copy completo y aprobado está en `copy-landing.md`.** No reescribirlo sin pedirlo.

---

## Estructura de carpetas

```
jay-personal-brand-landing/
├── index.html
├── copy-landing.md
├── HANDOFF.md
└── img/
    ├── workspace.png
    ├── banco-referentes.png
    ├── ia-guion.png
    ├── nichos-comparativo.png
    ├── bonus-1-camara.jpg
    ├── bonus-2-edicion.jpg
    ├── bonus-3-masterclass.jpg
    └── testimonios/
        ├── seul.jpg
        ├── erika.jpg
        ├── rosa.jpg
        ├── anita.jpg
        ├── clara.jpg
        └── rae.jpg
```

Rutas relativas siempre (`img/workspace.png`), nunca absolutas. Todo en minúsculas, sin espacios ni tildes.

---

## Estado actual

**Hecho**
- Análisis de la oferta y de la estructura original
- Estructura de 12 secciones definida y aprobada
- Copy completo escrito (`copy-landing.md`)
- Sistema visual congelado

**Pendiente**
- Construir el `index.html` con la nueva estructura y el nuevo sistema visual
- Tomar las 4 capturas de producto y las 3 portadas de bonos
- Descargar las 6 fotos de testimonios (hoy viven en el CDN de ClickFunnels; si se cancela esa cuenta, se caen)
- Grabar bonos 1 y 2
- Conseguir la URL de checkout de Hotmart

**Advertencia sobre una versión vieja del HTML**
Puede existir un archivo previo llamado `landing-sistema-notion.html`. Está desactualizado: usa Inter y Archivo, botones tipo píldora, amarillo `#ffe24a`, barra superior negra, valor total $435, masterclass como bonus #4 y la marca mrnotion.shop. No sirve como base. Sirve solo como referencia de patrones CSS.

---

## Cómo continuar

Prompt sugerido para arrancar en Cowork:

> Lee HANDOFF.md y copy-landing.md. Construye index.html con las 12 secciones, siguiendo el sistema visual y usando rutas relativas a img/. Deja la URL de checkout como una variable única al inicio del archivo, comentada, para poder cambiarla después en un solo lugar.
