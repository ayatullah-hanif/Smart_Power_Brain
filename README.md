# Smart Power Brain (SPB)

**One brain for every power source.**

Smart Power Brain is a retrofit device concept that helps protect appliances from damaging power conditions and switches automatically between grid, solar, battery and generator. This repository contains the presentation website for the project.

> **Status:** Concept stage. The images on the site are concept illustrations, not photos of an installed unit, and the features describe the intended product.

## The problem

In Nigeria, poor power quality (not only outages) quietly damages appliances and batteries: voltage sags, surges, overvoltage and floating neutral faults. Stabilizers, surge protectors and transfer switches each address one part of the problem, and they operate independently of each other.

## The idea

SPB sits between a building's electrical panel and its power sources, and works with the equipment people already own.

- **Instant protection:** a passive protection stage limits fast surges before they reach the panel.
- **Continuous monitoring:** voltage, current, frequency and neutral health are watched constantly. When supply becomes unsafe, SPB isolates it and moves compatible loads to a healthier source. Loads that cannot be powered safely are disconnected.
- **Appliance diagnostics:** learns each appliance's normal power pattern and flags unusual changes early.
- **Battery economics:** estimates battery wear and shows decisions in naira.
- **Neighbourhood power map (planned):** with owner consent, units can share anonymized power quality readings to map unstable areas.

SPB reduces exposure to damaging power. It does not make appliances immune, and proper earthing is still required.

## Progress so far

- 10+ customer interviews completed. Interviewees described the problem first-hand and showed strong interest.
- Interest is not yet sales; hardware and pilots are still ahead.

## About this website

A single-page static site, with no build step and no dependencies.

- Plain HTML, CSS and a little JavaScript
- Google Fonts (Sora and Figtree)
- Includes an interactive "simulate a power sag" demo (a simulation, not live data)

### Project structure

```
.
├── index.html
├── assets/
│   ├── concept-board.jpg
│   ├── concept-home.jpg
│   └── logo.png
└── README.md
```

## Run locally

Open `index.html` in your browser, or serve the folder:

```bash
npx serve .
```

## Deploy on Vercel

1. Push this repository to GitHub.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Set **Framework Preset** to **Other**. Leave the build command and output directory empty.
4. Click **Deploy**.

Keep the `assets` folder next to `index.html` and keep file names exactly as they are (Vercel is case-sensitive). To check images after deploying, open `your-project.vercel.app/assets/concept-board.jpg`.

## Editing

- **Contact details:** edit the `CONTACT` object near the bottom of `index.html`.
- **Images:** replace the files in `assets/` using the same file names, or update the paths in `index.html`.
- **Colours:** change the CSS variables at the top of the `<style>` block (`--bg`, `--teal`, `--blue` and so on).

## Contact

- Email: hanifayatullah2@gmail.com
- Phone / WhatsApp: +234 808 895 0364
- LinkedIn: https://www.linkedin.com/in/ayatullah-hanif-showunmi-411bb1288/

## License

All rights reserved. © 2026 Smart Power Brain.
