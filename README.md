# Pizzaventure — Lo‑Fi Anime Edition 🍕✨

Dit is een complete, self-contained HTML-game die klaar is om op GitHub Pages gehost te worden.
Gebaseerd op jouw wensen: lo‑fi vibes, anime‑achtige UI, uitgebreide gameplay (toppings, oven, staff, drive-thru, mini‑games, upgrades, events, achievements) en localStorage-opslag.

## Inhoud van deze repo
- `index.html` — het volledige spel (open in browser of host als GitHub Pages)
- `assets/` — assets (plaats hier echte .mp3 / .png bestanden ter vervanging van placeholders)
  - `bg_music.mp3` — achtergrondmuziek (placeholder)
  - `click.mp3` — geluidseffecten (placeholder)
  - `oven.mp3` — geluidseffect (placeholder)
  - `bg_lofi.png` — achtergrondafbeelding (placeholder)
- `README.md` — dit file

## Hoe te testen lokaal
1. Pak de ZIP uit.
2. Open `index.html` in je browser (dubbelklik of `file:///` pad).
   - Let op: autoplay van audio wordt door browsers vaak geblokkeerd. Klik op **Speel muziek** of ergens in het spel om audio te starten.

## Deploy naar GitHub Pages

### Methode A — via de website (eenvoudig)
1. Maak een nieuwe repository op GitHub (bijv. `pizzaventure`). Public repo is prima.
2. Upload de bestanden (`index.html`, `assets/`, `README.md`) via **Add file → Upload files**.
3. Ga naar **Settings → Pages** (of **Settings → Code and automation → Pages**, afhankelijk van GitHub UI).
4. Bij **Build and deployment** kies je:
   - Branch: `main` (of `gh-pages` als je die gebruikt)
   - Folder: `/ (root)`
5. Klik **Save**. Wacht ~1 minuut. Je site is bereikbaar op: `https://<jouw-gebruikersnaam>.github.io/<repo-naam>/`

### Methode B — via git (lokale machine)
```bash
# 1. initialiseer repo en push
git init
git add .
git commit -m "Initial commit — Pizzaventure"
git branch -M main
git remote add origin https://github.com/<jouw-gebruikersnaam>/<repo-naam>.git
git push -u origin main

# 2. activeer GitHub Pages in de repo settings (zoals hierboven)
```
> Tip: als je `index.html` in de root staat en Pages op de `main` branch root staat, wordt `index.html` automatisch gebruikt.

## Vervangen van de placeholders
Plaats echte bestanden in `assets/` met exact dezelfde bestandsnamen (`bg_music.mp3`, `click.mp3`, `oven.mp3`, `bg_lofi.png`). Refresh de pagina en test audio. Aanbevolen formaten: MP3 voor audio, PNG voor achtergrond (kleine resolutie oké).

## Aanpassingen die ik al heb gedaan voor jou (op basis van eerdere chats)
- Lo‑fi/Anime UI-stijl en kleurpalet aanpast naar jouw smaak.
- Veel features geïntegreerd: oven, toppings, staff, upgrades, drive-thru, mini‑games, events, achievements.
- Autosave (localStorage) en eenvoudige AI voor personeel.
- Audio-besturing (muziek + SFX) met gebruiker-gestuurde play-knop (je moet op 'Speel muziek' klikken om autoplay-blokkades te omzeilen).

## Wil je dat ik nog toevoeg:
- Echte audio-bestanden (ik kan niet uploaden naar externe hosting maar kan placeholders vervangen met jouw uploads).
- Verbeterde art-assets (achtergrond, icons) in anime-stijl — ik kan SVG/CSS artwork genereren.
- Een `gh-pages` branch automatisch deploy script (CI) of een GitHub Actions workflow om builds te maken.
- Een ZIP-/release configuratie voor directe GitHub Releases.

Veel plezier! — Als je wil, push ik het bestand nu ook direct naar een repository als je me jouw repo-naam en GitHub gebruikersnaam geeft (of ik geef precieze commando'sstep-by-step).
