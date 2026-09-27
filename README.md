# nuance.lab site

Public landing site for **nuance.lab** (Jason Yee · Utrecht).

Static HTML/CSS/JS — deployable on [Vercel](https://vercel.com) with zero build configuration.

**Domain:** [nuancelab.info](https://nuancelab.info) (DNS at [mijn.host](https://mijn.host); hosting on Vercel)

## Local preview

From this directory:

```bash
# Python
python3 -m http.server 8080

# or Node
npx --yes serve -l 8080
```

Open [http://localhost:8080](http://localhost:8080).

## Deploy on Vercel

1. Go to [vercel.com/new](https://vercel.com/new) and **Import** the GitHub repo `jayyeeaf/nuancelab-site`.
2. Leave Framework Preset as **Other** (or auto-detect). Root directory `.`, no build command, output directory `.` (or leave blank — Vercel serves static files from the repo root).
3. Click **Deploy**. You should get a `*.vercel.app` URL with no build errors.

## Custom domain (nuancelab.info)

DNS stays at **mijn.host**; point the domain at Vercel:

1. In the Vercel project → **Settings → Domains**, add `nuancelab.info` (and optionally `www.nuancelab.info`).
2. At mijn.host, create the DNS records **using the exact values Vercel shows** after you add the domain (typically an `A` / `AAAA` for the apex and/or a `CNAME` for `www`). Prefer Vercel’s live instructions over memorized IPs — they can change.
3. Wait for DNS propagation, then confirm HTTPS is active in Vercel.

## Brand

- Palette: taupe `#B4AEA2`, charcoal `#2C2C2C` / `#3A3A3A`, mid gray `#6E6E6A`, light `#E8E6E0` / `#F5F3ED`
- Affiliation line: **nuance.lab · Utrecht**
- Motion logo: `assets/nuance_lab_logo_motion_03.mp4` (poster + static JPG fallback)

## License

Site content © Jason Yee / nuance.lab. Brand assets reserved.
