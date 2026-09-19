# Still

A focus clock: Pomodoro, 12/24h, fullscreen, keeps your PC awake, light/dark, and music from
a pasted Spotify link or from your own files. Plain static files, no build step, no accounts, no keys.

## Deploy on Vercel

1. Put this folder in a GitHub repo (or run `vercel` inside the folder).
2. On Vercel: Framework Preset **Other**. Leave Build Command and Output Directory empty.
3. Open the URL Vercel gives you.

## Music

- **Spotify link**: open the music panel (button in the bottom bar, or press L), paste any
  open.spotify.com link (song, album, playlist, podcast) and it plays in Spotify's official embed.
  Log in to Spotify in the same browser for full songs (Premium); otherwise Spotify limits embeds to 30-second previews.
  The small arrow in the bottom bar shows the Spotify player, where you can skip songs and see the playlist.
- **My files**: drop songs or a folder anywhere on the page, or use Choose songs / Choose folder.
  Chrome and Edge remember your music folder, so next time you just press "Reopen".
  Works with mp3, m4a, aac, flac, wav, ogg and opus (whatever your browser can play).
  Titles, artists and cover art are read from the files' tags.
