# Motorsportskalender 2026

PWA til iPhone/Android. Tryk på et løb for at se dansk sendetid, TV-kanal og streaming.

---

## CSV-format — races.csv

```
dato,serie,event,lokation,dansk_tid,tv_dk,stream_dk,highlight
21. jun,F1,Britisk Grand Prix,Silverstone - UK,16:00 søndag,TV3+,Viaplay / F1 TV,
21. jun,NASCAR,Anduril 250 — K-Mag!,San Diego,22:30,TV3 Sport,Amazon Prime Video,★
```

| Kolonne | Forklaring |
|---|---|
| dato | fx `21. jun` eller `25-28. jun` |
| serie | `F1` / `WEC` / `IMSA` / `IndyCar` / `NASCAR` / `GT3` |
| event | Løbets navn |
| lokation | By - Land |
| dansk_tid | Fx `15:00 søndag` eller `TBA` |
| tv_dk | Dansk TV-kanal(er) eller `—` hvis ingen |
| stream_dk | Streaming-muligheder |
| highlight | Lad stå tomt for normale løb. Skriv `★` for markeret løb |

---

## TV-rettigheder i Danmark (2026)

| Serie | TV | Streaming |
|---|---|---|
| F1 | TV3+ (løb), TV3 Sport (træning) | Viaplay, F1 TV Pro |
| WEC / Le Mans | Eurosport 1 | Discovery+ / FIA WEC+ |
| IMSA | — | IMSA.tv (geo-blokeret — brug VPN) |
| IndyCar | TV3 Sport / TV3 Max | Viaplay / IndyCar Live |
| NASCAR | TV3 Sport | Amazon Prime Video (jun) / Viaplay |
| GT3 / Spa 24h | Eurosport 1-2 | Discovery+ / YouTube (GT-WC) |

---

## Opsætning: GitHub + Cloudflare Pages

1. Opret GitHub-repo og upload filerne
2. Cloudflare Pages → Connect to Git → vælg repo
   - Build command: *(tomt)*
   - Output directory: `/`
3. Safari → Del → "Føj til hjemmeskærm"

## Opdatere løb
Rediger `races.csv` direkte på GitHub → Commit → siden opdateres automatisk.
