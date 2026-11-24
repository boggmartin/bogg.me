# bogg.me

Källkod för www.boggma.se: en enda statisk HTML-sida med inbäddad CSS, utan bilder, skript eller externa typsnitt.

## Struktur

- `web-bio/` är sajten. Allt i den här mappen publiceras.
- `arkiv/` innehåller bilder som inte används på sajten. Den publiceras inte.

## Publicering (Cloudflare Pages)

Sajten publiceras automatiskt av Cloudflare Pages vid varje push till `master`.

- Build command: *(tomt)*
- Build output directory: `web-bio`


## DNS (Loopia)

- `www.boggma.se`: CNAME till `<projekt>.pages.dev`
- `boggma.se`: 301-omdirigering till `https://www.boggma.se` (Loopia). Cloudflare Pages kan bara ta huvuddomänen om DNS flyttas till Cloudflare.
- MX-posterna (Google) påverkas inte.
