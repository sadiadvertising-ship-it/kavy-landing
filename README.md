# KAVY LOGISTICS — Landing

Landing estática (1 archivo, sin dependencias) para ofrecer el servicio WMS (SILOG) bajo la marca **KAVY LOGISTICS** · dominio `kavycorp.com`.

## Ver localmente
Doble clic en `index.html`, o:
```bash
open index.html
```

## Editar la marca
Los colores están en variables CSS al inicio de `index.html` (bloque `:root`). Cambia un hex y se actualiza todo el sitio. Paleta actual:
- `--navy #0E2A47` (base logística dominante)
- `--accent #FF6B35` (acento KAVY / CTAs)
- `--cyan #2BB7C7` (secundario)

> Cuando Diego pase el manual de marca KAVY, reemplazar estos 3 valores.

## Contacto (ya configurado)
- WhatsApp: `+57 300 576 8886` → `wa.me/573005768886`
- Correo: `gerencia@kavycorp.com`
- El **formulario** abre WhatsApp con los datos por defecto (funciona sin servidor).
  Para recibir leads por correo: crear form gratis en https://formspree.io, poner
  `USAR_FORMSPREE = true` y pegar el endpoint (ver bloque `<script>` al final del HTML).

## Desplegar a kavycorp.com (Vercel)
```bash
npm i -g vercel        # si no lo tienes
cd ~/Projects/kavy-logistics
vercel                 # primer deploy (preview)
vercel --prod          # producción
```
Luego en el dashboard de Vercel → Project → **Settings → Domains** → agregar `kavycorp.com`
y `www.kavycorp.com`, y apuntar los DNS del dominio según indique Vercel.

> Alternativa sin CLI: arrastrar la carpeta a https://vercel.com/new
