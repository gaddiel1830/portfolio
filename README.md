# Gaddiel Fragoso — Engineering Portfolio

A responsive portfolio for Jesus Gaddiel Fragoso Vallejo, Metallurgical and Materials Engineering student at The University of Texas at El Paso.

Built with React, JavaScript/JSX, HTML, and CSS. Includes scroll entrance animations, hover effects, a mobile navigation menu, keyboard focus styles, and support for reduced-motion preferences. All production scripts and images are local: no CDN, font service, API key, or server-side application is required.

## Preview immediately

Extract the ZIP and open `index.html` in a browser. The compiled React bundle is already included. Click project images to open the original extracted image at full size.

For an HTTP preview, run `python -m http.server 8000` from this folder and visit http://localhost:8000. Python is optional and only needed for this local server method.

## Publish with GitHub Pages

1. Create a public GitHub repository named `portfolio` (or use `YOUR-USERNAME.github.io` for a personal site at the root URL).
2. Upload the **contents** of this folder to the repository's `main` branch. Put `index.html` directly at the repository root, not inside an extra `portfolio` folder. Include `styles.css`, the complete `assets` folder, and `.nojekyll`. The source, documentation, and package files may also be committed. Do not upload `node_modules` or the ZIP itself.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select **main**, choose **/(root)**, and click **Save**.
6. Wait for the Pages deployment to finish. The Pages settings screen provides the published URL. A project repository normally uses `https://YOUR-USERNAME.github.io/portfolio/`; a personal repository uses `https://YOUR-USERNAME.github.io/`.

The compiled site is ready for branch publishing, so no GitHub Actions configuration or build command is necessary. Relative asset paths support both URL formats. Changes committed to the publishing branch will deploy again.

Official guidance: [Configure a GitHub Pages publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) and [Create a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Edit and rebuild

Use Node.js 20 or newer and pnpm. From this directory:

```sh
pnpm install --frozen-lockfile
pnpm run build
```

If your pnpm installation blocks esbuild's install script and the build cannot locate its binary, run `pnpm approve-builds`, select **esbuild**, then rebuild. The project was built using React 19.1.1 and esbuild 0.25.9; exact dependencies are recorded in `pnpm-lock.yaml`.

- Edit `src/main.jsx` for portfolio text, React components, image references, and navigation.
- Edit `styles.css` for layout, color, typography, and animation.
- Edit `index.html` for page title, description, and favicon.
- Keep images in `assets/images/` and use relative paths.
- After JSX changes, run the build and commit the updated `assets/app.js` and its accompanying license file.
- CSS changes do not require rebuilding JavaScript.

The source uses CSS for motion; no animation-library dependency is required. Visitors who request reduced motion receive a static experience.

## Contents

```text
index.html             HTML entry point and metadata
styles.css             Responsive layout and motion
src/main.jsx           Editable React source
assets/app.js          Ready-to-publish JavaScript bundle
assets/app.js.LEGAL.txt Third-party license notices
assets/images/         Extracted project images
package.json           Dependencies and build command
pnpm-lock.yaml         Reproducible dependency versions
pnpm-workspace.yaml    Allows the esbuild installation script
.nojekyll              Static GitHub Pages publishing
.gitignore             Excludes local dependencies
CONTENT_SOURCES.md     Content provenance and source limitations
README.md              This guide
```

## Content maintenance

The resume's “Present” employment dates and expected May 2027 graduation date are preserved as supplied. Update them as your experience changes. Contact uses the supplied email address. No GitHub or LinkedIn profile was invented. The original resume and reports are not published as downloads; selected images and summarized content are included instead.

The site contains About, Projects, Skills, Experience, Education, and Certifications sections. Project findings remain qualified where the source material is incomplete or internally inconsistent. See `CONTENT_SOURCES.md` before adding further numerical claims. No blanket open-source license is applied to personal content or project imagery. React's bundled license notices are retained.
