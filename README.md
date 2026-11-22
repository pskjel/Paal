# Idrettshall Soundboard

Målmusikk-portal for idrettshall, integrert med Spotify Web Playback SDK. Hele appen ligger i én fil: `index.html`.

## Publisering
- **Netlify Drop:** dra `index.html` (eller mappen) inn på https://app.netlify.com/drop
- **GitHub Pages:** Settings → Pages → deploy fra branch, rot-mappen.

## Oppsett
1. Åpne den publiserte siden og fold ut «Spotify Oppsett».
2. Trykk «Kopier URL» og lim inn under *Redirect URIs* i https://developer.spotify.com/dashboard (huk av for Web API + Web Playback SDK).
3. Lim inn Client ID, og trykk «Logg inn med Spotify». Krever Spotify Premium og en nettleser på PC/Mac.

Snarveier: `Space`/`M` = MÅL!, `S` = stopp med fade, `Esc` = nødstopp.
