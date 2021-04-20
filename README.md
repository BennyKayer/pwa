# PWA

## HTTPS
- Requires HTTPS to run at all — some stuff that it's doing is sensitive
- Let's encrypt gives free certificates
- Cloudflare encrypts automatically and has a free plan to host files

## Manifest
- Contains stuff for splash screens, app icons etc.

## Service Worker
- Another worker, thread, background worker
- Programmable proxy, control per request behavior
- Intercepts request and checks whether communication with network is necessary
- He goes to Cache API and fetches stuff

## Adding PWA
1. Can't be done locally
2. You need to install gh-pages with `npm install gh-pages`
3. Then define a homepage (above deps) for gh-page `"homepage": "https://BennyKayer.github.io/learning",`
4. Then add 2 scripts `"predeploy": "npm run build",` and `"deploy": "gh-pages -d build",`
5. In new `NPX` created apps you need to `serviceWorker.register()`