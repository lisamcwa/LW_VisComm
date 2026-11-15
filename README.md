# LAW of design — Portfolio Website

A custom, responsive portfolio site using your logo, with **free GitHub Pages hosting** and an **online editing dashboard from Pages CMS**.

## What's in this package
- `index.html` — homepage (Jekyll template)
- `_projects/` — projects managed in the dashboard
- `_data/settings.yml` — text and contact details managed in the dashboard
- `assets/images/` — logo and sample concept images
- `assets/uploads/` — your uploaded project photos
- `.pages.yml` — configuration for the content-editing dashboard
- `preview.html` — a standalone preview to open on your computer (not the live editable page)

## Set up your free website
1. Create a GitHub account at https://github.com if you don't already have one.
2. Create a **public** repository named `law-of-design-portfolio` (or any name you like). Choose **Add a README** only if you want to; it is optional.
3. Unzip the site package. Upload **all files and folders, including `.pages.yml`,** to the root of that repository. GitHub's web uploader may hide files that start with a dot on some systems; verify `.pages.yml` is present. On Mac, press Command+Shift+period to show hidden files in Finder.
4. Open the repository's **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/(root)`, then Save.
5. GitHub will build the Jekyll site and publish it at `https://YOUR-USERNAME.github.io/law-of-design-portfolio/`. The included project links and assets support project-repository subpaths. The URL may become available after GitHub finishes the first build.
6. Open https://pagescms.org/ and sign in with GitHub. Authorize access to your repository when requested, then choose your portfolio repository to open its editing dashboard. The CMS reads `.pages.yml` to expose **Website Text & Contact** and **Portfolio Projects**.
7. In the dashboard, first edit **Website Text & Contact** and add `contact_email`. Then open **Portfolio Projects** to replace the five illustrative sample entries or add new projects. You can upload cover images, change categories, reorder work, and write project stories.
8. Save changes in Pages CMS. They are saved to GitHub; GitHub Pages republishes the updated website. No HTML editing needed for routine content changes.

## IMPORTANT: repository URL and images
If your GitHub repository has a custom name, the free URL uses that exact name. Jekyll's `relative_url` filter requires `baseurl` in `_config.yml` to be set to `"/REPOSITORY-NAME"` for a **project** site. **Set `baseurl` before publishing:**

`baseurl: "/law-of-design-portfolio"`

If the repository is named `YOUR-USERNAME.github.io` (a user site), leave `baseurl: ""`.

For a purchased custom domain, GitHub Pages supports connecting it without buying a hosting plan. Read GitHub's custom-domain directions and set `url`/`baseurl` accordingly.

## Adding your own projects
In Pages CMS → Portfolio Projects → New entry:
- Enter a title and select a category.
- Upload the cover image (JPG, PNG or WebP recommended; 1400–2000px wide works well).
- Add a short description and year.
- Use **Display Order** to rearrange projects (lower numbers show first).
- Keep **Feature on Homepage** enabled to show the project in the grid.
- Fill in the rich-text story field with your description and additional images if desired.
- Save: the project gets its own page and appears automatically in the grid.

## About the preview
Open `preview.html` on your computer to see an approximation of the homepage immediately. The live site uses the real `index.html` template and reads dashboard content automatically through Jekyll. `preview.html` itself is not used for publishing.

## Notes
- The five starter thumbnails and project stories are clearly marked **samples**, not real client work.
- Replace the sample portfolio projects with actual work before sharing the site publicly.
- The contact button activates when you enter your email in the CMS. No email address is guessed.
- GitHub Pages requires the repository to be public on the standard free plan. Do not upload confidential client files.
- Pages CMS is a separate service. Its features and availability may change; confirm its current terms before relying on it.
- The portfolio's CSS/HTML design is custom and is not visually editable via Pages CMS; **content and images** are editable, but layout changes require code.
