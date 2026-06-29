# FitRun Example — Demo para clientes

Prototipo de demostración de **FitRun**, una plataforma de gestión para escuelas y equipos de **running**, que conecta a entrenadores con sus alumnos: planes de entrenamiento semanales, pagos y cuotas, carnés de salud, carreras, comunicados y seguimiento del progreso.

> ⚠️ Marca y datos **ficticios**. Es un prototipo de presentación, no la aplicación de producción.

## Estructura

```
fitrun-demo/
├── index.html              # Landing de presentación (hero, features, galería, contacto WhatsApp)
├── prototipo/
│   └── index.html          # Prototipo interactivo navegable (5 pantallas, escritorio + móvil)
├── assets/
│   └── screens/            # Capturas en alta resolución dentro de chasis MacBook / iPhone
├── vercel.json             # Configuración de despliegue
└── README.md
```

## Cómo verlo localmente

Es HTML estático, sin build. Abrí `index.html` en el navegador, o serví la carpeta:

```bash
npx serve fitrun-demo
# o
python3 -m http.server --directory fitrun-demo 8080
```

## Despliegue en Vercel

El proyecto es estático; Vercel lo sirve directo (sin framework).

```bash
vercel        # preview
vercel --prod # producción
```

## Personalización

- **Color de marca:** se define en las variables CSS `--orange*` del `<style>` de `index.html` y del prototipo.
- **Link a la app real:** en `index.html`, botón con `id="demoRealBtn"`. Mientras `data-pending="true"`, el botón abre WhatsApp; al pegar la URL real, cambiá el `href` y quitá el `data-pending`.
- **Contactos WhatsApp:** enlaces `wa.me` en la sección `#contacto`.

## Contacto

| Nombre | WhatsApp |
|---|---|
| Santiago Neira | [+598 91 274 380](https://wa.me/59891274380) |
| Cesar Martinez | [+598 94 469 680](https://wa.me/59894469680) |
