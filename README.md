# Minglearn

**Where Learning Meets Connection** — a location-based peer study and student community platform that connects students with peers by subject, study goals and availability.

## Features
- Discover study groups and nearby campus map (Leaflet + OpenStreetMap)
- Virtual Pomodoro study lounge
- Open resource library
- Dark / light theme
- Safety, privacy and report tools
- Optional Supabase backend configuration (via in-app modal)

## Project structure
```
minglearn/
├── index.html     # The whole app (HTML, CSS, JS)
├── logo.svg       # App logo
├── favicon.svg    # Browser tab icon
├── 404.html       # Redirects unknown URLs back to the app
├── .nojekyll      # Tells GitHub Pages to skip Jekyll
├── .gitignore
├── LICENSE
└── README.md
```

## Run locally
Open `index.html` in a browser, or serve it:
```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploy on GitHub Pages
1. Push all files to a GitHub repository (branch `main`).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. Your site will be live at `https://<username>.github.io/<repo-name>/`.

## Tech / CDN dependencies
Tailwind CSS, Leaflet, Lucide Icons, canvas-confetti, Google Fonts, DiceBear avatars. These load from CDNs, so an internet connection is required.

## Security note
Never commit real Supabase service keys. Only use the public `anon` key in client-side code.
