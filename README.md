# Tianxia Player Dashboard — GitHub Pages

## Publish
1. Create a **public** GitHub repository named `tianxia-dashboard`.
2. Upload **the contents of this folder** to the repository root (not the enclosing folder): `index.html`, `.nojekyll`, `music/playlist.json`, and all five MP3 files.
3. Go to repository **Settings → Pages → Build and deployment**. Select **Deploy from a branch**, `main`, `/(root)`, and **Save**.
4. Open `https://YOUR-USERNAME.github.io/tianxia-dashboard/`.

## Add or remove a soundtrack
- Upload additional MP3s inside the `music/` directory.
- Edit `music/playlist.json`, adding one object per track: `{ "name": "Display title", "file": "exact-name.mp3" }`.
- To remove a track from playback, delete its entry from the playlist (and optionally its MP3).
- Changes are visible after GitHub Pages deploys and the dashboard is refreshed.

## Controls and saved notes
- On opening, one random soundtrack is selected and an autoplay attempt is made. Most browsers require a click or keypress to start audible playback. One track plays as an intro and then stops unless Continuous Shuffle is enabled.
- The player journal is not automatically stored on the server. Players must export their JSON notes and import them again later, as before.
- Players may still add their own MP3s via the Music Library, saved only to their own browser when supported. These do not upload to GitHub.

## Privacy and licensing
- GitHub Pages content is publicly reachable. Only publish MP3s you have permission to redistribute, and do not commit private GM notes or secrets.
- The site fetches `./music/playlist.json` using HTTP(S); opening `index.html` directly from disk (`file://`) will not reliably load the playlist.
