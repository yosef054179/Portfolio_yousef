# Yousef Hamdey — Portfolio

Static bilingual portfolio website with project previews, local image assets, a downloadable CV, and WhatsApp contact.

## Publish on GitHub Pages

1. Push this repository to GitHub on the `main` branch.
2. Open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
3. The workflow in `.github/workflows/deploy.yml` will publish the site automatically after each push to `main`. You can also start it from the **Actions** tab with **Run workflow**.
4. When the deployment finishes, open the site URL shown in the workflow's **deploy** job. For a project repository, it is usually `https://<owner>.github.io/<repository>/`.

The published site uses `index.html` as its homepage and includes the `assets/`, `projects/`, profile image, and downloadable CV. The `.nojekyll` file is included in the deployment artifact so GitHub Pages serves static files without Jekyll processing.

## Google Search Console

The homepage includes the Google site-verification meta tag. After the site is publicly deployed, add its final GitHub Pages URL in Search Console and complete verification. Keep the verification tag in `index.html`.
