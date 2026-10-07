# Baaz — Violet Edition

A faithful local recreation of https://bajkamalsingh.me/ with the supplied Adobe Color palette:

- Magenta: `#DC1EFE`
- Violet: `#7030F1`
- Deep purple: `#4D2999`
- Near-black: `#0B0721`
- White: `#FFFEFE`

## Open the website

Open `index.html` in a browser, or serve this folder with any static web server. For example, from this folder:

```sh
python -m http.server 4173
```

Then open http://localhost:4173.

## Included

The original intro sequence, hero video, cursor interactions, sound toggle, scroll timelines, notebook, project cards, Metro navigation and case studies, image-trail gallery, contact links, and legal pages are retained. The original portfolio content and external destinations remain in place.

Media, fonts, animation libraries, icons, and compiled styles are stored locally. Artwork and photographs retain their original colors; the hero video is tinted with a CSS filter. Website surfaces, typography, accents, borders, and motion colors use the new palette.

`index.html` contains the page and original animation logic. Palette and layout styles live in `css/`. Legal pages live in `pages/`. Images and video live in `assets/`. `vendor/` and `fonts/` contain local dependencies.

The reference website's deployment-specific analytics and Cloudflare challenge scripts are excluded. The icon dependency was repaired and sound/navigation buttons have accessible labels.

## Project structure

```text
index.html              Home page (inline CSS and animation JavaScript)
css/                    Palette and precompiled layout styles
pages/                  Privacy and terms pages
assets/images/          Gallery, logos, and case-study artwork
assets/video/           Hero video
vendor/                 Local animation and icon libraries
fonts/                  Local fonts and font-face stylesheets
.nojekyll               Enables ordinary static assets on GitHub Pages
```

No installation, build step, API key, or environment variables are required. The JavaScript for the interactions is fully included in `index.html`; it is not a remote embed of the reference website.

## Put this project on GitHub

Extract the ZIP, create an empty GitHub repository, and run the following inside this project folder. Replace `YOUR-USERNAME` and `YOUR-REPOSITORY` with your actual repository details:

```sh
git init
git add .
git commit -m "Add complete portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

For static hosting, use this folder as the website root. The entry page is `index.html`, and asset paths are relative, so the site can also run under a GitHub Pages repository path.

The project contains approximately 150 MB of media. Push the extracted project files to your repository. The export excludes private hosting credentials, temporary work, and repository history.

The original website's names, portfolio content, contact destinations, and third-party library notices are retained. This export does not add a new license to those materials.
