# Website Strategy Catalog

A static site showcasing industry-specific website strategy guides. Built with plain HTML and CSS — no frameworks.

Each guide covers the right audience-first thinking for a specific industry: who the visitor is, what they need to feel, what builds trust, what friction to remove, and how to structure the site for results.

---

## Deploying to GitHub Pages

### Step 1 — Push the repository to GitHub

If you haven't already:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/<your-username>/website-strategy-catalog.git
git push -u origin main
```

### Step 2 — Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings**
3. In the left sidebar, click **Pages**
4. Under **Build and deployment**, set:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Click **Save**

### Step 3 — Wait for deployment

GitHub will build and deploy the site. This usually takes 1–3 minutes.

### Resulting URL

Once deployed, your site will be available at:

```
https://<your-username>.github.io/website-strategy-catalog/
```

Replace `<your-username>` with your actual GitHub username.

> **Note:** The repository must be **public** for GitHub Pages to work on a free account. Private repositories require a paid GitHub plan for Pages deployment.

---

## Updating the Foundational Mile site link

Once deployed, update the catalog link in the main Foundational Mile site.

In `foundationalmile_site/src/pages/website-strategy-catalog.astro`, find:

```html
href="https://yourusername.github.io/website-strategy-catalog/"
```

Replace `yourusername` with your actual GitHub username or org name (e.g. `foundational-mile`).

---

## File Structure

```
/
├── index.html                    # Catalog home page
├── README.md
├── industries/
│   ├── ministries.html           # Ministry & Church strategy
│   ├── construction.html         # Construction Contractor strategy
│   ├── chiropractor.html         # Chiropractor strategy
│   ├── cleaning.html             # Cleaning Company strategy
│   └── private-school.html       # Private School strategy
└── assets/
    └── css/
        └── styles.css            # Global styles
```

---

## Adding More Industries

To add a new industry page:

1. Copy any existing file from `/industries/`
2. Update the `<title>`, `<meta description>`, and all content sections
3. Add a link to the new page in `index.html` inside the `.industry-grid` section

---

Built by [Foundational Mile](https://foundationalmile.com)
