# cardinal-booking-widget

Hosted bundle of the **Cardinal Plaza Shell** online-booking widget, loaded by the
Duda site (`cardinalplazashell.com`) via a small fetch-and-inject loader.

- **`cardinal-booking.js`** — the built widget (CSS + JS + button wiring in one file).
  **Generated — do not edit by hand.** Source of truth is the `cardinal-booking`
  project's `cardinal-booking.html`; rebuild with `node build-widget.mjs` and push here.
- **`duda-loader.html`** — the one-time snippet pasted into Duda's site-wide Body/footer.

Updating the live widget = edit source → `node build-widget.mjs` → copy `cardinal-booking.js`
here → `git push`. No Duda re-paste. Propagation is near-instant (the loader cache-busts;
GitHub's raw CDN refreshes within a few minutes).
