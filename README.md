# Mingyun Cho — Academic Homepage

A lightweight, responsive academic homepage inspired by the editorial/minimal aesthetic of academic CV sites. This is an independently written implementation (not a copy of another repository's code).

## Preview locally

Open `index.html` in a browser. The fonts are loaded from Google Fonts, so they may require an internet connection; fallback fonts work offline.

## Edit your information

- **Name, school, research interests, news, projects, and education:** Open `index.html`, find the relevant text, and edit it directly.
- **Email:** In `index.html`, search for `TODO:` under the Contact section. Replace the placeholder with your real PUBLIC email address and an `mailto:` link. Do this before sharing your site publicly if you want people to contact you.
- **CV PDF:** If you'd like a downloadable CV, put a PDF in `assets/` and add a hyperlink to it from the header or About section, e.g. `<a href="assets/Mingyun_Cho_CV.pdf">CV ↗</a>`.
- **Projects:** The medical AI repository URL is a team repository. Add individual GitHub and project URLs only when you have verified links.
- **Style:** Edit the custom properties at the top of `style.css` to change colors, and the section styles to change spacing.

## Publish on GitHub Pages (no command line required)

1. In GitHub, create a new **Public** repository named `YOUR_GITHUB_USERNAME.github.io` (substitute your exact GitHub username).
2. Extract this ZIP. **Do not upload the ZIP as a single file.** Upload `index.html`, `style.css`, `.nojekyll`, `README.md`, and `favicon.svg` into the root of your repository. GitHub's web upload UI may not show hidden dotfiles on every system; `.nojekyll` is optional here.
3. In the repository, open **Settings → Pages → Build and deployment**. Set **Source** to **Deploy from a branch**, **Branch** to `main`, and folder to `/(root)`, then save.
4. Open `https://YOUR_GITHUB_USERNAME.github.io/` after publishing has completed.

GitHub's official guide: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Content notes

The site reflects a **November 2026 starting draft**. Research interests are aspirational directions, not claims about completed publications. Add publications only after they exist. Check project descriptions, lab affiliation, and dates before publishing.

## Version 2 — soft sky-blue refresh

- All warm red/brown tones changed to soft sky-blue, pale blue-white, and slate-blue neutrals.
- Corrected the English name to **Mingyun Cho** in page content, metadata, and footer.
- Reduced the hero name size and simplified the introduction.
- Removed hero shortcut links and the right-side affiliation sidebar.
- Added a profile-photo placeholder. To add your own photo, put a photo named `profile.jpg` next to `index.html`, then find `hero-portrait` inside `index.html` and replace the `portrait-placeholder` div with:

  ```html
  <img class="portrait-image" src="profile.jpg" alt="Portrait of Mingyun Cho">
  ```

**Updating GitHub:** Upload `index.html`, `style.css`, and `favicon.svg` to the repository root. In GitHub's upload screen, commit the changed files. (You can upload this README too.) Leave `.nojekyll` as-is.
