# AGENTS.md: ifdv.nl

Gearchiveerd project: geen nieuwe features.

Instructies voor AI-agents en ontwikkelaars. Lees eerst `README.md` en `CHANGELOG.md`.

## Project
- Klant: Impactfonds Duurzame Voedselketen Rotterdam (IFDV) · Bedrijf: All This · SLA: Nee
- Status: archief, niet meer live (oktober 2026), noindex
- Stack: Astro 5, Tailwind 3, Node 22 (zie `.nvmrc`)
- CMS: geen (content in MDX onder `src/data/`)

## Werkwijze
- Niets verwijderen. Niet pushen naar `main`. Geen force-push.
- Alleen documentatie of archiefonderhoud, op een branch en via een PR.
- Commit nooit `.env`-bestanden of tokens.
- Bij een noodzakelijke wijziging: een regel onder de nieuwste datum in `CHANGELOG.md`.

## Conventies
- Geen nieuwe pagina's, features of dependencies.
- Site blijft op Netlify (`impactfontsdvr`) met `X-Robots-Tag: noindex, nofollow`.
- Afbeeldingen: geen vastgelegd profiel volgens `~/Code/_standards/IMAGES.md` (TODO, niet meer in te voeren).
