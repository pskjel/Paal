# KampDJ

Kampmusikk for idrettshallen (Mål, Timeout, Pause). Hele appen ligger i én fil: `index.html`.
Publiseres på https://kampdj.no via GitHub Pages (`CNAME`-fila peker dit).

## Lydkilder
- **Plex (standard):** musikk fra klubbens egen Plex-server. Appen er åpen for alle uten innlogging.
  Administrator kobler Plex til hver enhet én gang via `https://kampdj.no/#admin` → «Koble til Plex».
  Plex-serveren må ha **Fjerntilgang** slått på.
  - *Gjør klar til kamp* lagrer sangene på enheten (virker uten nett).
  - *Foreslå dropp automatisk* analyserer lyden og setter starttid.
- **Spotify:** krever innlogging, Premium og at brukeren er lagt til under User Management i Spotify Dashboard.

## Konfigurasjon (øverst i skriptet i `index.html`)
- `DEFAULT_SOURCE` – `'plex'` eller `'spotify'`.
- `PLEX_SHARED_TOKEN` – valgfri token for en egen, begrenset Plex-konto, slik at alle enheter får musikk uten oppsett. Blir offentlig synlig – bruk aldri din egen hovedkonto.
- `OWNER_NAME`, `OWNER_EMAIL`, `TERMS_VERSION` – brukes i brukervilkår og personvernerklæring (endre versjon for å be om ny godkjenning).
- `DEFAULT_CLIENT_ID`, `ALLOWED_USERS` – for Spotify.

## Domene (kampdj.no → GitHub Pages)
DNS hos Gigahost: fire A-poster (`185.199.108.153`–`185.199.111.153`) og `www` CNAME → `pskjel.github.io`.

Snarveier: `Space`/`M` = Mål, `T` = Timeout, `P` = Pause, `S` = stopp med fade, `Esc` = nødstopp.
