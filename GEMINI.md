# Proyecto: Linaje Valderrey

Página web conmemorativa y genealógica dedicada al apellido **Valderrey**. Documenta la historia, heráldica, distribución y personalidades de este linaje de origen leonés.

**URL en producción:** https://valderrey.com  
**Repositorio:** GitHub Pages, rama `main` → dominio personalizado vía Cloudflare  
**Creador:** Iván Roque Valderrey González — ivan@valderrey.com

---

## Estructura de ficheros

```
/
├── index.html          # Página principal
├── styles.css          # Todos los estilos
├── CNAME               # Dominio: valderrey.com
├── GEMINI.md           # Este archivo
└── assets/
    └── img/
        ├── escudo_valderrey.png       # Escudo heráldico principal
        ├── piedad_valderrey.jpg       # Foto de Piedad Valderrey
        ├── creaciones_valderrey.jpg   # Foto del taller de Piedad
        ├── valderrey_etimologia.jpg   # Imagen sección Origen
        ├── piedad_taller_1.jpg        # Foto adicional taller (sin usar en HTML)
        └── piedad_taller_2.jpg        # Foto adicional taller (sin usar en HTML)
```

> **Importante:** Todas las imágenes están en `assets/img/`. No poner imágenes sueltas en la raíz.

---

## Secciones de la página (en orden)

1. **Navbar** fija — transparente, se vuelve oscura al hacer scroll. Hamburguesa en móvil.
2. **Hero** (`#`) — Escudo flotante, título "Valderrey", tagline, botón CTA "Explorar el Linaje".
3. **Origen y Etimología** (`#origen`) — Apellido toponímico, "Val de Rey", Maragatería, Reino de León.
4. **Benavides de Órbigo** (`#benavides`) — Municipio leonés donde vive la familia del creador. Río Órbigo, Paso Honroso, tarjeta de datos geográficos.
5. **Distribución en España** (`#distribucion`) — Barras CSS con datos del INE. León (412), Madrid (76), Barcelona (45)... Total: 651 personas con el apellido como primero.
6. **Personalidades Destacadas** (`#personalidades`) — Ely Valderrey (fútbol, Venezuela), Julio Valderrey (poesía, Venezuela), Eduardo Valderrey (arte, España), Piedad Valderrey (artesanía cristal, Menorca), Marquesado de Valderrey.
7. **Heráldica** (`#heraldica`) — Análisis del escudo: Sinople, Azur, Oro y Plata.
8. **Footer** — Escudo, lema, nombre del creador, email, copyright 2026.

---

## Tecnologías

- **HTML5 / CSS3** — sin frameworks
- **Tipografías:** Cinzel, Lora, Playfair Display (Google Fonts)
- **Animaciones:** AOS 2.3.4 (Animate On Scroll, cdnjs)
- **Fondo hero:** Unsplash (URL directa, funciona en producción)
- **Textura imagen etimología:** transparenttextures.com (castle-outline, mix-blend-mode)

---

## Diseño y estética

Estilo **"Premium Heritage"**. Paleta:
- `--gold: #C5A028` / `--gold-light: #E8D18D`
- `--sinople: #1B4332` (verde heráldico)
- `--azur: #002855` (azul heráldico)
- `--bg-dark: #0A0A0A` / `--bg-light: #FDFBF7`

Secciones alternas claro/oscuro (`section-dark`). Animaciones AOS en todas las secciones.

---

## Responsive

- **Navbar:** hamburguesa con panel lateral en `≤768px`
- **Hero:** `min-height: 100svh` (fix barra navegador móvil). Tipografía fluida con `clamp()`.
- **Breakpoints:** 992px, 768px, 480px

---

## Contexto histórico del apellido

- **Origen:** Toponímico, villa de Valderrey, comarca de la Maragatería, sur de León.
- **Significado:** "Val de Rey" — Valle del Rey. Dominio real durante el Reino de León.
- **Raíces familiares:** La familia del creador lleva generaciones en **Benavides de Órbigo** (comarca Ribera del Órbigo, León).
- **Heráldica:** Escudo partido. 1º Sinople con torre de oro. 2º Azur con puente de plata sobre ondas.
- **Distribución:** ~651 personas con Valderrey como primer apellido en España (INE). Concentración en León (>60%).

---

## Reglas para no romper nada

1. **Imágenes** → siempre en `assets/img/`, referenciadas como `assets/img/nombre.jpg` en HTML y CSS.
2. **Commits** → solo a rama `main`. Cada push actualiza valderrey.com en minutos.
3. **Datos del INE** → no inventar cifras. Los datos actuales están contrastados.
4. **Estilo** → no añadir frameworks CSS (Bootstrap, Tailwind, etc.). Todo va en `styles.css`.
5. **Sección eliminada** → "Crónica de un Linaje" (timeline) fue eliminada intencionadamente. No restaurar.

---

*Documento actualizado: abril 2026*
