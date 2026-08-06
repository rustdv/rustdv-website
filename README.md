# rustdv.org

The marketing site for [rustdv](https://github.com/rustdv/rustdv), a hardware
verification framework in Rust, and its companion book, *Rust for RTL
Verification*.

Plain HTML and CSS, no framework, no build step. Deployed to GitHub Pages by
`.github/workflows/deploy.yml` on every push to `main`; the custom domain is
`rustdv.org` (see `CNAME`).

| Path | What it is |
|---|---|
| `index.html` | Landing page: hero, how it works, benefits, the book, built-with-Claude |
| `introduction.html` | pyuvm-README-style introduction + the "What rustdv Provides" reference tables |
| `translations.html` | Python→Rust and SV-UVM→rustdv translation tables + the chapter map |
| `journey.html` | The level-5-development story (write-up in progress) |
| `book/` | The rendered mdBook HTML of *Rust for RTL Verification* |
| `css/style.css` | The one stylesheet |
| `assets/` | Logo and headshot |

The `book/` directory is generated: rebuild it with `mdbook build book-pdf` in
the rustdv repository and copy the HTML output here. The reference tables in
`introduction.html` and `translations.html` come from the book's Appendices A–D;
if an appendix changes, regenerate the tables rather than editing them by hand.
