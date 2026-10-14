# Avian Behaviour & Migration — GitHub Pages starter

A responsive, public-facing workshop website with a course homepage, a Reveal.js slide deck for Day 1, interactive MCQs, and short activities with suggested answers. Day 2 and Day 3 currently have programme scaffolds; they can be expanded as the teaching material is finalised.

## Files

- `index.html` — workshop landing page
- `day-1.html` — Day 1 browser-based slide deck, quiz questions and activities
- `day-2.html`, `day-3.html` — programme pages to expand next
- `assets/css/site.css` — homepage and page styling
- `assets/css/slides.css` — slide deck styling
- `assets/js/slides.js` — Reveal.js configuration
- `assets/js/activities.js` — MCQ feedback and answer-reveal interactions

## Publish on GitHub Pages

1. Create a **new public repository** on GitHub, for example `avian-behaviour-workshop`.
2. Download and unzip this project.
3. Upload the *contents* of the unzipped folder to the repository root. The root should contain `index.html`, `day-1.html`, `day-2.html`, `day-3.html`, `README.md`, and the `assets` folder.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Choose branch `main` and folder `/(root)`, then save.
7. Wait for the deployment to finish. GitHub will show the published URL in **Settings → Pages**. It will usually look like `https://YOUR-USERNAME.github.io/avian-behaviour-workshop/`.

## Preview before publishing

Open `index.html` in a browser to check the landing page. The slide deck uses Reveal.js loaded from a CDN, so an internet connection is needed for the slide controls and fonts to load. For a more accurate local preview, use a simple local web server or publish to a temporary public repository.

## Presenter notes

The slide deck contains notes in Reveal.js speaker-note blocks (`<aside class="notes">`). With the Day 1 deck open, press **S** to open presenter view. Check that this works in your browser before teaching.

## Important limitations

- The site is public; do not upload private participant details or sensitive information.
- MCQ feedback and answer reveals run in the browser. This starter does **not** collect participant answers or scores centrally.
- Because the site is public, do not put answer keys or presenter notes on the same public pages if they must remain confidential. Reveal.js presenter notes are not a secure access-control mechanism; the HTML source can be inspected.
- Fonts and Reveal.js are loaded from third-party CDNs, so an internet connection is required.
- This project is a starting point. Day 2 and Day 3 are programme scaffolds, not complete slide decks yet.

## Editing the slides

Open `day-1.html` in a code editor. Each `<section>` inside `<div class="slides">` is a slide. Edit the visible HTML within a section to change slide content. Keep the `<aside class="notes">` element for presenter notes. MCQs use `data-quiz`, `data-answer`, and `data-explanation` attributes; activities use `data-reveal` and a matching element `id`.

## Next recommended steps

1. Preview and publish this starter site.
2. Finish Day 2 slides, starting with “From research question to field method”.
3. Finish Day 3 slides and add references/credits for images and readings.
4. Test on desktop and mobile, including slide navigation, MCQs and presenter view.
