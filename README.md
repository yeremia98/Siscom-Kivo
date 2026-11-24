# SISCOM ERP & HRIS - Revamp Landing Page
Static site (HTML + CSS + ES modules + Three.js via CDN). Tanpa build step.

## Jalankan lokal
    python3 -m http.server 8000   # buka http://localhost:8000

## Deploy ke Vercel
1. `git init && git add . && git commit -m "revamp siscom" && git push` ke GitHub.
2. Vercel > Add New > Project > pilih repo. Framework Preset: **Other**, Build Command kosong, Output Directory `.`.
3. Hubungkan domain di Settings > Domains.

## Yang perlu diganti (cari `ISI` di index.html dan assets/js/main.js)
- Nomor WhatsApp `WA` di main.js, URL sosial media, GA4 ID, testimoni, nama klien, logo klien (assets/img), OG image.
- Three.js dimuat dari cdn.jsdelivr.net (three@0.160.0). Jika offline, hero tampil dengan latar gradien.
