# Kalorisnål Glass

Kalorisnål glass 2026 — Sveriges 20 kalorisnålaste glassar rankade per styck, plus tre systersidor som rankar samma produkter efter varsin egen modell.

**Live:** https://www.kalorisnalglass.se/

## Sidor

| Sida | Modell |
| --- | --- |
| `/` | Kalorier per styck, 20 glassar |
| `/nyttig-glass/` | Fyra kriterier × 1–3 p, max 12 p |
| `/god-glass-lag-kalori/` | Smakbetyg 1–5 under 135 kcal, plus kcal per smakpoäng |
| `/proteinglass/` | Kcal och protein grupperat per enhet, med omräknare |
| `/sannany/` | Produktsida för glassen på förstaplatsen |
| `/om/` | Metoden bakom rankningen |

Sidorna delar medvetet inte modell — det är så de slipper konkurrera om samma sökintention.

## Teknik

Statiska sidor, ingen build. Undersidorna delar `/styles.css`; startsidan, `/om/` och `/sannany/` har fortfarande sin CSS inline. GSAP är vendorat till `/vendor/` (ingen CDN).

SEO/GEO: canonical, Open Graph, `Organization`-, `WebSite`-, `WebPage`- (med `speakable`), `BreadcrumbList`-, `ItemList`- och `Product`-schema, sitemap.xml, robots.txt med explicita allow-regler för AI-crawlers (GPTBot, ClaudeBot, PerplexityBot m.fl.) samt llms.txt med samtliga rankingar som maskinläsbara fakta.
