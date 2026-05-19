# Gestión en Salud Dental — Dra. Sofía Saganía

Sitio web del consultorio odontológico de la Dra. Sofía Luciana Saganía, en Villa del Parque, CABA.

## Estado actual

**v1 (raíz)** es la versión elegida y la que se está iterando. **v2** queda guardada como referencia visual por si rescatamos elementos. v3 fue descartada.

Sofía no quiere un sistema de turnos: prefiere manejar la agenda ella misma. Todas las acciones de "reservar / pedir turno" abren WhatsApp directamente con un mensaje pre-armado.

## Variantes

| Versión | Ruta | Estética | Estado |
|---|---|---|---|
| **v1** | [`/index.html`](index.html) (raíz) | Pastel verde/rosa, tipografía serif elegante (Fraunces). | **Elegida** |
| **v2** | [`/v2-turquesa/index.html`](v2-turquesa/index.html) | Turquesa/coral del flyer, tipografía geométrica (Manrope). | Referencia |

Ambas tienen un selector flotante "Ver versiones" (esquina inferior derecha) para alternar durante la revisión.

## Orden de secciones (v1)

1. Inicio (hero)
2. Sobre mí (Dra. Saganía)
3. Servicios (los 11 tratamientos)
4. Horarios (atención + ubicación con mapa)
5. Contactame (CTA grande con WhatsApp + Instagram)

## Datos del consultorio

- **Profesional**: Dra. Sofía Luciana Saganía — Odontóloga (UBA), especializada en Prostodoncia.
- **Dirección**: Pedro Lozano 3235, 1° C — Villa del Parque, CABA.
- **Horarios**: Lun, Mar, Jue, Vie de 14:00 a 19:00 · Mié de 09:00 a 19:00.
- **Servicios**: Limpieza dental · Obturación dental · Extracciones · Prótesis fija · Prótesis removible · Blanqueamiento · Placa de bruxismo · Protector bucal · Certificado bucodental · Selladores de fosas y fisuras · Aplicación de flúor.

## Configuración pendiente

En `index.html` (y también `v2-turquesa/index.html` si se quiere mantener funcional como referencia) buscar y reemplazar:

```js
const WA_NUMBER = '5491140903128';   // Ya configurado (+54 9 11 4090-3128)
const IG_USER = 'gestionensaluddental';   // Confirmar usuario real de Instagram
```

Adicionalmente, agregar el archivo del logo:

```
img/Logo GES.png
```

(la página ya lo referencia en el navbar y el footer; falta subir el archivo binario al repo)

Email del footer (`contacto@gestionensaluddental.com`) y coordenadas del mapa también pueden ajustarse si hace falta.

## Estructura

```
.
├── index.html              # v1 (raíz) — versión elegida
├── v2-turquesa/
│   ├── index.html          # v2 — referencia
│   └── contacto.html       # formulario de contacto (sin enlazar, para rescate)
├── img/
│   ├── Logo GES.png        # ← pendiente de subir
│   ├── Dra. Saganía 2.png
│   ├── Dra. Saganía 4.png
│   └── Dra. Saganía 8.jpeg
├── CNAME
└── README.md
```

---

© 2026 Gestión en Salud Dental — Dra. Sofía Saganía
