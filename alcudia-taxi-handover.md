# Alcúdia Taxi — handover

- Live URL: https://tasar1-ship-it.github.io/-alcudia-taxi/
- Repo: tasar1-ship-it/-alcudia-taxi (leading hyphen in the name) (GitHub Pages, main branch, root)
- For: MJ and Ronald, iPhone home-screen app
- Current version: service worker `alcudia-taxi-v2` (2 Nov 2026)

## Files
- `index.html` — the whole app, English / Korean switch (CSS-only radios), inline CSS and ES5 JS
- `sw.js` — offline cache; network first, cache fallback. Bump `CACHE` on every change to a cached file
- `manifest.json`, `icon-180.png`, `icon-512.png` — home-screen install

## Constants as they are
- ES5 only, no CDN, no Google Fonts (system fonts)
- localStorage key: `at1_lang` (remembers English or Korean)
- No Firebase
- `noindex` meta tag; the page carries Ronald's name and apartment address

## Content
- Taxis: Taxis Alcúdia 971 549 870 (main), Taxi Riera Ramis 616 909 588, Radio Taxi Pollença 971 866 213
- Accident: 112, Policía Local Alcúdia 971 545 006, Guardia Civil Port d'Alcúdia 971 546 908
- Open Uber button (https://m.uber.com/ul/) under the main taxi number; Uber has no phone booking in Spain (v2)
- Alcúdia numbers shown in red; 112 in black; Pollença in blue
- Pick-up address: Carrer de Canet del Rosselló 19, 07400 Alcúdia
- Numbers checked 2 Nov 2026 (TIB taxi list, Páginas Amarillas, alcudiamallorca.com); none test-called

## Known open points
- Guardia Civil Port d'Alcúdia office may be seasonal; main post is Pollença 971 865 842 (not on page yet)
- Hospital numbers (Inca 971 88 85 00, Juaneda Muro 971 89 19 00) offered, not added
