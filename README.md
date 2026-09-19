# Still

A focus clock: Pomodoro, 12/24h, fullscreen, keeps your PC awake, light/dark, and your Spotify library.
Plain static files. No build step, no server code.

## Deploy on Vercel

1. Put this folder in a GitHub repo (or run `vercel` inside the folder).
2. On Vercel: Framework Preset **Other**, leave Build Command and Output Directory empty.
3. Note your production URL, e.g. `https://still-yourname.vercel.app`.

## Connect Spotify

1. Go to https://developer.spotify.com/dashboard and create an app. Tick **Web API** and **Web Playback SDK**.
2. Add this Redirect URI exactly (with the trailing slash): `https://YOUR-PROJECT.vercel.app/`
3. In the app's **User management**, add the email of your Spotify account.
4. Copy the app's **Client ID** into `config.js`, commit, and Vercel redeploys.
   (Or leave it empty and paste it in the app once per browser.)

Notes
- Use your production domain. Preview deployments get different URLs, and Spotify only accepts redirect URIs you registered.
- Playing music inside the page needs Spotify Premium.
- Spotify development-mode apps need a Premium owner and allow 5 users. They can only list songs for playlists you own or collaborate on; other playlists can still be played whole.
- Local testing: Spotify rejects `localhost`. Use `http://127.0.0.1:PORT/` and register that URI too.
