# Gestión en Salud Dental — Dra. Sofía Saganía

Sitio web del consultorio odontológico de la Dra. Sofía Luciana Saganía, en Villa del Parque, CABA.

Este repositorio contiene **tres variantes de diseño** para que la clienta elija la que mejor represente al consultorio. Cada versión propone una estética y funcionalidad distintas.

## Variantes disponibles

| Versión | Ruta | Estética | Funcionalidad |
|---|---|---|---|
| **v1** — Pastel verde/rosa | [`/index.html`](index.html) (raíz) | Suave, cálida, femenina. Tipografía serif elegante (Fraunces). | Turnero completo: calendario + selección de horario + formulario + integración con Google Apps Script. |
| **v2** — Turquesa & coral | [`/v2-turquesa/index.html`](v2-turquesa/index.html) | Clínica, profesional, fiel a la paleta del flyer existente. Tipografía geométrica (Manrope). | Formulario de contacto completo. Envío por Apps Script o `mailto:` como fallback. |
| **v3** — Editorial moderna | [`/v3-mezcla/index.html`](v3-mezcla/index.html) | Minimal, contemporánea, mezcla de tonos sage y peach. Tipografía editorial (Cormorant Garamond). | Solo CTAs por WhatsApp con mensajes pre-armados por servicio. Sin formularios. |

Cada versión incluye un **selector flotante "Ver versiones"** (esquina inferior derecha) para saltar entre las variantes durante la revisión.

## Datos del consultorio

- **Profesional**: Dra. Sofía Luciana Saganía — Odontóloga (UBA), especializada en Prostodoncia.
- **Dirección**: Pedro Lozano 3235, 1° C — Villa del Parque, CABA.
- **Horarios**: Lun, Mar, Jue, Vie de 14:00 a 19:00 · Mié de 09:00 a 19:00.
- **Servicios**: Limpieza dental · Obturación dental · Extracciones · Prótesis fija · Prótesis removible · Blanqueamiento · Placa de bruxismo · Protector bucal · Certificado bucodental · Selladores de fosas y fisuras · Aplicación de flúor.

## Configuración pendiente

Los siguientes valores deben reemplazarse antes de publicar la versión elegida:

### v1 (turnero completo) — `turnero.html`
```js
const GOOGLE_SCRIPT_URL = 'REEMPLAZAR_CON_URL_APPS_SCRIPT';
const WA_NUMBER = 'REEMPLAZAR_CON_NUMERO_WSP';
```

### v2 (formulario) — `v2-turquesa/contacto.html`
```js
const GOOGLE_SCRIPT_URL = '';                 // Opcional, si vacío usa mailto
const WA_NUMBER = 'REEMPLAZAR_CON_NUMERO_WSP';
const EMAIL_TO = 'contacto@gestionensaluddental.com';
```

### v3 (WhatsApp) — `v3-mezcla/index.html`
```js
const WA_NUMBER = 'REEMPLAZAR_CON_NUMERO_WSP';
```

Adicionalmente, en todas las versiones revisar:
- Enlaces de Instagram (`href="#"` en los íconos sociales).
- Email de contacto en el footer.
- Coordenadas del mapa OpenStreetMap (actualmente apunta a una zona aproximada de Villa del Parque).

## Estructura

```
.
├── index.html              # v1 (raíz)
├── turnero.html            # v1 — sistema de turnos
├── v2-turquesa/
│   ├── index.html          # v2
│   └── contacto.html       # v2 — formulario
├── v3-mezcla/
│   └── index.html          # v3 (todo en una página)
├── img/
│   ├── Dra. Saganía 2.png
│   ├── Dra. Saganía 4.png
│   └── Dra. Saganía 8.jpeg
├── CNAME
└── README.md
```

## Próximos pasos

1. La clienta revisa las 3 variantes y elige la que prefiera.
2. Se ajustan textos finales, colores secundarios y detalles puntuales.
3. Se completan los valores de configuración (WhatsApp, email, Apps Script si aplica).
4. Se publica la versión elegida en la raíz y se eliminan las descartadas.

---

© 2026 Gestión en Salud Dental — Dra. Sofía Saganía
