# ayogiclife.de

Static website for A Yogic Life (Berg am Laim, Munich). Plain HTML and CSS, no build step, hosted on GitHub Pages.

## Structure
| Path | Page |
|---|---|
| `index.html` | English (main) |
| `de/index.html` | German |
| `impressum/` · `datenschutz/` | Legal pages (German) |
| `img/` | Photos (WebP + JPG, already colour-graded) |
| `fonts/` | Self-hosted fonts (Marcellus, Figtree, SIL OFL) |

## How to change things
- **Schedule:** search for `Weekly schedule` (EN) / `Wochenplan` (DE) and edit the table rows. Also update `openingHoursSpecification` in the JSON-LD block in the `<head>`.
- **Prices:** search for `price-grid` and `price-more`, in both language files.
- **Reviews:** search for `class="quotes"`. Copy reviews word for word from Google. Update the `5.0` / `12` count in the hero, the reviews section and `aggregateRating`.
- Always change **both** `index.html` and `de/index.html`.

## Publish
1. Repo → Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
2. Custom domain: once ayogiclife.de has moved away from Jimdo, enter `ayogiclife.de` in Settings → Pages (this creates the `CNAME` file) and set the DNS records at the new registrar:
   - `A` records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` for `www`: `<github-username>.github.io`
   - Then tick *Enforce HTTPS*.
3. Google Business Profile website link: `https://ayogiclife.de/?utm_source=google&utm_medium=gmb&utm_campaign=profile`

## Before launch
- [ ] Impressum: add USt-ID if there is one.
- [ ] Datenschutz: have it reviewed; add a section if a cookie-free counter is added.
- [ ] Add the LinkedIn link in "About me" (optional).
