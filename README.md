# Ewaen Erhahon: Business Analyst Portfolio

A static portfolio made of plain HTML, CSS and JavaScript. No npm, Node.js, React or build step. Open `index.html` to preview it locally.

## Upload to GitHub
1. Create a new repository on github.com (for example `portfolio`).
2. Choose **Add file > Upload files** and drag in **everything inside this folder** (not the folder itself), so `index.html` sits in the repository root.
3. Click **Commit changes**.

## Turn on GitHub Pages
**Settings > Pages > Build and deployment > Deploy from a branch > main > / (root) > Save.** GitHub serves `index.html` as the home page; your link appears on that page after a minute or two.

## Where to change things
Almost everything is in **`assets/js/data.js`**: name, title, location, tagline, bio, About text, skills, experience, projects (including case-study text), CV path, email, phone, LinkedIn, GitHub and the Formspree endpoint (`formspreeEndpoint`).
- **Page titles / SEO**: the `<head>` of `index.html`.
- **Photo**: replace `assets/images/profile.png` (or change `photo` in data.js).
- **CV**: replace the PDF in `assets/documents/` and update `resume` in data.js.
- **Add a project**: copy one `{ ... }` block inside `projects` in data.js, change the text, keep the commas.
- **Project images / supporting documents**: none were supplied, so cards are text only. To add images, place files in `assets/images/` and ask for an `image` field to be added to the card.
- **Colours**: CSS variables at the top of `assets/css/style.css` (`:root` for light, `[data-theme=dark]` for dark).
- **Fonts**: the Google Fonts link in `index.html` and the `--head` / `--body` variables in style.css.
- **Favicon**: `favicon.svg` in the root. Replace it with your own file of the same name.

## Contact form
The form posts to your Formspree endpoint. The first message you send may require you to confirm your email address in Formspree.
