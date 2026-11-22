# KampDJ

Kampmusikk for idrettshallen (MÅL!, Timeout, Pause) styrt via Spotify. Hele appen ligger i én fil: `index.html`.
Publiseres på https://kampdj.no via GitHub Pages (`CNAME`-fila peker dit).

## Domene (kampdj.no → GitHub Pages)
1. Hos domeneregistraren, legg inn DNS for `kampdj.no`:
   - `A`-poster: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - (valgfritt) `CNAME` for `www` → `pskjel.github.io`
2. GitHub → repo → **Settings → Pages**: deploy fra denne branchen, mappe `/ (root)`. Custom domain: `kampdj.no`. Huk av **Enforce HTTPS** når sertifikatet er klart.
3. Spotify Developer Dashboard → appen → **Redirect URIs**: legg til `https://kampdj.no/`.

## Tilgang
- Appen er låst bak Spotify-innlogging. Bare kontoer som er lagt til under **User Management** i Spotify Dashboard slipper inn.
- Sett `DEFAULT_CLIENT_ID` i `index.html` så brukerne slipper å skrive inn Client ID.
- Valgfritt: `ALLOWED_USERS` begrenser til bestemte Spotify-brukernavn/e-poster.

Snarveier: `Space`/`M` = MÅL!, `T` = Timeout, `P` = Pause, `S` = stopp med fade, `Esc` = nødstopp.
