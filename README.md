# startwitha.xyz

Landing page for [Start with A](https://startwitha.xyz) — an open-source, self-hostable investment research platform for serious value investors.

## Deploy

Static single-file site. Push to `main` and enable GitHub Pages (source: root).

## Stack

- React 18 (CDN) + Babel standalone
- No build step — single `index.html`
- Three switchable themes (dark default)
- Mobile responsive

## Pages

- `/` — landing page (`index.html`)
- `/quiz/` — "Is Start with A right for you?" 7-question qualification quiz (`quiz/index.html`).
  CTA destinations live in `QUIZ_CONFIG` at the top of the script. Analytics events
  (`quiz_started`, `quiz_completed`, `quiz_cta_clicked`) are no-ops unless Plausible, Umami,
  gtag or a GTM `dataLayer` is present on the page. Shared results use `/quiz/?s=<score>`.

## License

AGPL-3.0
