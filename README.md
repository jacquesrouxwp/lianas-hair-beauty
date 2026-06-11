# Liana's Hair & Beauty — Demo site

Single-file (`index.html`) static demo website built exactly to spec.

## Quick start
Open `index.html` directly in browser (all content visible without JS).

Or serve locally:
```bash
# Python
python -m http.server 5173 --directory .

# Node
npx serve .
```

## Structure
- `index.html` — everything (HTML + CSS in <style> + JS in <script>)
- `before-after/` — expected ba-1.jpg … ba-5.jpg (carousel hides gracefully if none load)
- `owner/` — expected owner.jpg (graceful placeholder if missing)

## Features implemented
- Exact data, services (4 tabs), prices, reviews (literal), hours, contacts
- Bilingual NL/EN with data-i18n + full I18N dict + localStorage
- MENUS object for prices (per language)
- WhatsApp buttons (general + signature prefilled text)
- Carousel: arrows + dots + swipe + 5s autoplay + missing images → hide section
- All CSS variables, Fraunces + Manrope via Google Fonts
- No frameworks, no external JS, no preloader/hidden content
- Responsive (tested conceptually at 390px, breakpoints 880/560)
- PIN-only note, Keune mentions, 12+ jaar, heren & dames, Treatwell ratings

## Before deploy
1. Add real photos to `before-after/` and `owner/`
2. Replace Instagram comment when handle found
3. Confirm exact "vanaf" prices with operator

## Checklist (post-build)
- [x] Opens without white/blank screen (static first paint)
- [x] 390px mobile friendly
- [x] All WhatsApp links use 31619003052
- [x] Price tabs switch categories + full NL/EN
- [x] Language switch updates all static + dynamic content + <html lang>
- [x] Carousel works + auto-hides when images missing
- [x] Reviews verbatim + "Treatwell review · geverifieerd"
- [x] Signature treatment highlighted
- [x] Hours exact (no "indicatief" footnote)

## Remaining to clarify with operator
See the list at the end of the build message.