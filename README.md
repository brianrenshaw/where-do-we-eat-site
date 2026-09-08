# Where Do We Eat public site

Static HTML and CSS hosted by GitHub Pages from main at https://brianrenshaw.github.io/where-do-we-eat-site/.

- `index.html`: public app overview and TestFlight link.
- `guide/index.html`: guide aligned with app beta build 15.
- `privacy/index.html`: existing privacy policy; wording preserved.
- `assets/`: original app icon and simulator screenshots with sample dining content.

Preview with `python3 -m http.server 8765`. No build step, external fonts, analytics, or client-side JavaScript. Keep guide labels aligned with the in-app How It Works copy. Check phone and desktop widths, dark appearance, keyboard focus, anchors, links, and image loading before pushing main.
