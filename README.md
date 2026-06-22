# Suytex Portafolio Experience — Landing Page

Landing page estática para el curso. Diseño dark mode, responsive, sin frameworks.

---

## Editar el contenido

Todo el texto vive en **`assets/content.txt`**. Puedes editarlo directo desde GitHub sin tocar el HTML.

### Cómo hacerlo en 30 segundos

1. Abre [`assets/content.txt`](./assets/content.txt) en GitHub.
2. Haz clic en el ícono ✏️ (Edit this file).
3. Edita el texto que quieras.
4. Haz **Commit changes** → la página se actualiza sola.

### Estructura de `assets/content.txt`

El archivo tiene dos partes:

**1. Frontmatter** (al inicio, entre `---`):
```yaml
---
brand: Suytex Portafolio Experience
whatsapp: https://wa.me/18091234567?text=QUIERO
---
```
| Campo | Qué hace |
|---|---|
| `brand` | Nombre que aparece en el título del browser y el footer |
| `whatsapp` | URL del botón "Reserva tu cupo". Cambia el número por el tuyo. |

**2. Secciones** marcadas con comentarios HTML:
```markdown
<!-- section: hero -->
## Título principal

Texto del hero...

<!-- section: pain -->
## ¿Te suena familiar?

- Item 1
- Item 2
```

Los marcadores `<!-- section: TIPO -->` le dicen a la página cómo estilizar cada bloque. **No los borres ni los muevas** — solo edita el contenido debajo de ellos.

### Secciones disponibles

| Marcador | Qué renderiza |
|---|---|
| `hero` | Pantalla completa con CTA |
| `pain` | Grid de cards con puntos de dolor |
| `problem` | Texto centrado de impacto |
| `transformation` | 3 cards con los entregables |
| `outcomes` | Lista de resultados |
| `method` | Grid de los 7 principios |
| `philosophy` | Quote centrado en grande |
| `format` | Features del formato del curso |
| `includes` | Checklist de entregables |
| `for-who` | Dos columnas Sí/No |
| `pricing` | Card de precio |
| `faq` | Acordeón de preguntas |
| `cta` | Sección final de cierre |

---

## Activar GitHub Pages

1. Ve a **Settings** del repositorio.
2. Panel izquierdo → **Pages**.
3. En *Source*, selecciona **Deploy from a branch**.
4. Branch: `main` · Folder: `/ (root)`.
5. Guarda. En ~1 minuto tendrás la URL pública (ej: `https://suytex.github.io/suytex-academy-promo/`).

---

## Desarrollo local

Para previsualizar en local necesitas un servidor HTTP (el `fetch()` de JS no funciona con `file://`):

```bash
# Python
python3 -m http.server 3000

# Node
npx serve .
```

Luego abre `http://localhost:3000`.

---

## Estructura del repo

```
/
├── index.html        # Shell HTML + CSS + JS (no tocar para cambiar contenido)
├── assets/
│   └── content.txt   # TODO el contenido editable
└── README.md         # Este archivo
```
