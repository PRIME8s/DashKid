# Dash Kid (Sprite-Sheet + Parallax)

A lightweight HTML5 canvas endless runner using your sprite sheet and a canyon parallax background.

## Local Run
Open `index.html` in a browser. (No build step required.)

## Deploy to **GitHub Pages**
Two options:

### Quick (Pages from `main` via Action)
1. Create a new repo on GitHub, e.g. `dash-kid`.
2. Push this folder to `main`.
3. Go to **Settings → Pages** and set **Source: GitHub Actions**.
4. The included workflow will build & publish automatically to `https://<your-user>.github.io/dash-kid/`.

### Manual (Pages from `gh-pages` branch)
1. Create orphan branch:  
   ```bash
   git checkout --orphan gh-pages
   git rm -rf .
   git checkout main -- .
   git commit -m "Publish"
   git push -u origin gh-pages
   ```
2. In **Settings → Pages**, set **Source: Deploy from a branch**, then pick `gh-pages` and `/ (root)`.

## Development Notes
- All assets live in `/assets`.
- `index.html` contains the game code; tune constants at the top of the script (speed, gravity, spawn rates).
- Mobile friendly; tap canvas to jump.

## License
MIT
