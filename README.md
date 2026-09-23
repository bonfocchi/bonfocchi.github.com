# bonfocchi.com

Source for [bonfocchi.com](https://bonfocchi.com), the personal website of Ricardo Bonfocchi Ventura: product leader, former CTO and founder, and engineer based in Lisbon.

The site is a single-page résumé covering background, experience, skills, education, and contact details.

## How it's built

- **One file.** Everything lives in `index.html`: markup, styles, and scripts. No build step, no framework, no dependencies to install.
- **Fonts:** [Lora](https://fonts.google.com/specimen/Lora) and [DM Sans](https://fonts.google.com/specimen/DM+Sans) from Google Fonts.
- **Hero globe:** a rotating orthographic globe drawn on `<canvas>` with [D3](https://d3js.org/), [TopoJSON](https://github.com/topojson/topojson), and the world topology bundled with [Datamaps](https://datamaps.github.io/), all loaded from cdnjs. It pins cities I've lived or worked with, draws a connection between two visible pins every couple of seconds, and shows a tooltip on hover. It is purely decorative: it respects `prefers-reduced-motion`, and the page works fine if the scripts fail to load.

## Running locally

Open `index.html` in a browser, or serve the folder with any static server:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Deployment

The site is hosted on [GitHub Pages](https://pages.github.com/) from the `master` branch. The `CNAME` file maps it to the custom domain `bonfocchi.com`. Pushing to `master` publishes the changes.

## Contact

- Email: [hey@bonfocchi.com](mailto:hey@bonfocchi.com)
- LinkedIn: [linkedin.com/in/bonfocchi](https://linkedin.com/in/bonfocchi)

## License

Copyright © 2026 Ricardo Bonfocchi Ventura. All rights reserved.
