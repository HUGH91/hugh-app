# Hugh app

A fan site for Hugh Augustine with sections for music, videos, a shop, shows, updates, a contact page and a "Proud to Pay" support page. It's built as one HTML page with no build step.

This is the design preview that was first built and hosted in ChatGPT (hugh-app.mellowplume303961.chatgpt.site). These are the same files that preview served, copied over unchanged on Nov 24, 2026.

## Files

- `index.html`: the whole app (HTML, CSS and JavaScript in one file)
- `assets/`: the four photos the app uses, from the *Please Wait to Be Seated* cover shoot (photography: Melian Junius / @violavioletti)

## Run it

Open `index.html` in a browser, or serve the folder from any static host:

```
python3 -m http.server 8000
```

Then go to http://localhost:8000.

To publish it for free, turn on GitHub Pages for this repo (Settings → Pages → deploy from the `main` branch). Pages on a private repo needs a paid GitHub plan, so you would need to make the repo public or upgrade.

## Current state

- **Contact form:** sends messages to yohugh91@gmail.com through FormSubmit (formsubmit.co). This was confirmed working in October 2026.
- **Shop and Proud to Pay:** previews only. No payments are collected and checkout isn't connected.
- **Music and videos:** the players only preview files from the visitor's own device. No audio or video has been uploaded yet.
- **Shows:** no confirmed dates yet.
- **Saved collection:** stored in the visitor's own browser (localStorage).
- The contact form's no-JavaScript fallback redirects to `thanks.html` on the old ChatGPT preview address. If the site moves, update the `_next` value in `index.html` to the new address.
