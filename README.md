# Personal portfolio

A single scrolling page made with HTML, CSS, and JavaScript. No installation or build step is required.

## Open in VS Code

Open this `portfolio` folder in VS Code. Open `index.html` in your browser, or use VS Code's Live Server extension for automatic refresh while editing.

- `index.html`: page content, timeline, and case studies
- `styles.css`: colors, typography, layout, and mobile styles
- `script.js`: mobile menu, current-section highlighting, and footer year
- `assets/`: local images and, later, your resume PDF

## Replace the placeholders

1. Search `index.html` for square brackets (`[`) and fill in your name, school, dates, organizations, case studies, and work samples. Update the page title and description too. Change the `Y.` brand mark and favicon if desired.
2. Put your headshot in `assets/`. Replace the portrait image's `src` and write accurate alt text such as `Headshot of Your Name`. The example SVG is just a placeholder.
3. Replace the two work image sources with your own photos or screenshots and update their alt text and captions. Use approved material with private information removed.
4. Put the four IT roles in their actual chronological order and use their official titles. The current order follows the conversation and has not been verified against dates. Add a truthful contribution under each role. Adjust the approach diagram if necessary so it reflects how you work.
5. Add `assets/resume.pdf`. Replace the disabled resume button with:

   ```html
   <a class="button button-dark" href="assets/resume.pdf" target="_blank" rel="noopener">Open resume (PDF) <span aria-hidden="true">↗</span></a>
   ```

   Update the accompanying text to indicate the PDF is available. A `download` attribute can be added if you prefer a download.
6. For each social profile, change the opening `<div class="social-card">` into `<a class="social-card" href="YOUR_REAL_PROFILE_URL" target="_blank" rel="noopener noreferrer">` and change its corresponding closing `</div>` into `</a>`. Replace the “coming soon” text with your handle or a short call to action. The inner div containing the title and description stays a div.
7. Replace each work sample's “coming soon” span with an anchor to your document or project, for example `<a class="text-link" href="assets/your-assignment.pdf">View assignment (PDF)</a>`.

Case studies use native expandable details, so they are accessible by keyboard and work even without JavaScript. The menu remains visible if JavaScript is disabled. The site also respects reduced motion settings.

## GitHub and Vercel

Copy these files into the root of your portfolio repository, keeping the `assets` folder beside `index.html`. If the repository already has an application, integrate the files with that application rather than overwriting its structure.

For a plain static project in Vercel, choose the **Other** framework preset, leave the build command empty, and serve the repository root (`.`). No package installation is needed. If the files remain in a subfolder, choose that folder as the project's Root Directory.

Pushing the configured production branch deploys the live site. Pushing another branch creates a preview under the usual Git integration settings. These files have not been pushed or deployed.
