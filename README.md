# ifdv.nl

> Archief van de All This-website voor Impactfonds Duurzame Voedselketen Rotterdam (IFDV): eenpagina-site over impactleningen in de Rotterdamse duurzame voedselketen.

| | |
|---|---|
| **Klant** | Impactfonds Duurzame Voedselketen Rotterdam / Impact First Group |
| **Bedrijf** | All This |
| **Status** | Archief · niet meer live (okt 2026), noindex |
| **SLA** | Nee |
| **Live** | Was `https://ifdv.nl` (domein wijst nu elders). Archief: [impactfontsdvr.netlify.app](https://impactfontsdvr.netlify.app) |
| **Netlify** | team All This, site `impactfontsdvr` → [impactfontsdvr.netlify.app](https://impactfontsdvr.netlify.app). Geen custom domain meer gekoppeld |
| **CMS** | geen (content in `src/data/*.mdx`) |
| **Repo** | [github.com/astrobuildclub/archive-ifdv.nl](https://github.com/astrobuildclub/archive-ifdv.nl) |
| **Notion** | TODO |

## Stack

- Astro 5 · Node 22 (`.nvmrc`) · static
- Styling: Tailwind 3 · Fonts: Adobe Fonts / Typekit (`tmw4ewt`)
- Animatie: Motion (SVG-lijn / secties)
- Consent: geen · Hosting: Netlify

## Lokaal starten

```bash
nvm use
npm install
npm run dev            # http://localhost:4321
```

Overige scripts: `npm run build`, `npm run preview`, `npm run astro …`.

Controle oktober 2026, Node 22: `npm install` en `npm run build` slagen.

### Environment-variabelen

Geen. Er is geen `.env.example`.

## Structuur

```
public/         Favicon, share-image, assets
src/
  components/   Hero, Footer, Drawing, Partners, …
  data/         MDX-secties (intro, invest, team, …)
  js/           Observatie- en SVG-animatie
  layout/       default.astro (SEO via astro-seo)
  pages/        index.astro
  styles/       global.css
```

## Content en CMS

Geen CMS. Copy en tabellen staan in MDX onder `src/data/` en worden via componenten op de homepage geladen.

## Privacy, toegankelijkheid en SEO

- Consent: geen tracking ingericht
- WCAG: semantische opzet, geen formele 2.2 AA-audit
- Archief: `X-Robots-Tag: noindex, nofollow` in `netlify.toml`; meta robots `noindex, nofollow` in de layout. Geen `Disallow` in robots.txt (bestaat niet). Sitemap-verwijzing: n.v.t.

## Deploy

- `main` → productie op Netlify (`impactfontsdvr`) · pull requests → deploy preview
- Werkwijze gold: branch → PR → preview → merge. Geen nieuwe features meer

## Bekende issues en afspraken

- Gearchiveerd in oktober 2026. Geen nieuwe features.
- `npm audit` meldt kwetsbaarheden. Niet opgelost.
- Build waarschuwt dat browserslist-/baseline-data verouderd is. Niet opgelost.
- Domein `ifdv.nl` wijst niet meer naar deze Netlify-site.

---

Eigenaar: All This · Wat er gedaan is: zie [`CHANGELOG.md`](CHANGELOG.md) · Werkafspraken voor ontwikkelaars en AI-agents: [`AGENTS.md`](AGENTS.md)
