# Andrómeda — Landing Page

Landing page de **Andrómeda**, agencia de desarrollo de software a la medida potenciada por IA. El sitio está diseñado para presentar los servicios de la empresa y capturar oportunidades de negocio a través de un formulario de contacto.

## Stack

El sitio es un único archivo HTML autocontenido. No requiere build ni servidor:

- **React 18** via CDN (renderizado del lado del cliente)
- **Babel Standalone** para transpilación de JSX en el navegador
- **CSS custom properties** para theming (tema oscuro cósmico, acento violeta)
- **Google Fonts**: Space Grotesk · DM Sans · JetBrains Mono
- **Canvas API** para el starfield animado del fondo

## Estructura

```
startup-project/
└── index.html   # Todo el sitio: HTML + CSS + JSX inline
```

## Secciones

| Sección | Descripción |
|---|---|
| **Hero** | Headline, CTA principal, showcase interactivo (flujo de propuesta + arquitectura) |
| **Servicios** | Desarrollo a la medida · Consultoría & arquitectura · Modernización & integraciones · Soporte |
| **IA** | Cómo se aplica IA en diseño, arquitectura, código y QA |
| **Tecnología** | Stack 2026: Next.js, React, TypeScript, Tailwind, Node.js, PostgreSQL, Vercel, Cloudflare, Supabase… |
| **Proceso** | 4 fases: Visión compartida → Diseño con propósito → Construcción ágil → Evolución continua |
| **Contacto** | Formulario con validación (nombre, email, empresa, tipo de proyecto, mensaje) |
| **Footer** | Links de navegación, contacto, copyright |

## Uso

Abre `index.html` directamente en el navegador. No requiere servidor local, aunque sirviéndolo desde uno (ej. `npx serve .`) se evitan posibles restricciones CORS en algunos navegadores.

```bash
npx serve .
# o
python3 -m http.server 3000
```

## Personalización

Las variables de color están definidas en `:root` dentro del `<style>` del HTML:

```css
--violet: #a855f7;        /* color de acento principal */
--violet-deep: #6b3fc7;   /* acento oscuro */
--violet-soft: #d4b8ff;   /* acento claro */
--bg: #06030f;            /* fondo base */
--ink: #f5f0ff;           /* texto principal */
```

Para cambiar los datos de contacto del footer (email, teléfono, ubicación), busca la sección `Footer` dentro del `<script type="text/babel">`.

## Sobre Andrómeda

Agencia de desarrollo de software a la medida y consultoría tecnológica. Equipo remote-first construyendo producto digital desde Latinoamérica (CDMX · Bogotá).

- **hola@andromeda.dev**
- Servicios: desarrollo a la medida, consultoría, modernización, soporte
- IA integrada en cada etapa: el equipo toma las decisiones, la IA acelera el proceso
