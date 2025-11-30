# Data Sharing In A Box

!!! warning "Sample Content Only"
    This page contains **example language and placeholders** designed to help registry teams build their own data sharing site.  
    Please **replace all placeholder text** with details specific to your own project, policies, and governance requirements.
    
## ☀️ How to Set Up and Use the Patient Registry Template

This template helps patient registry teams create a public-facing website to share data documentation, governance policies, and data access instructions. It’s built using [MkDocs](https://www.mkdocs.org/) with the [Material theme](https://squidfunk.github.io/mkdocs-material/).

### 1. Copy This Template Repository

You have two options:

- **Use GitHub’s “Use this template” button** (recommended):
  - Go to the [template repository](https://github.com/BoyceLab/DataSharingInABox).
  - Click **"Use this template"** to create your own copy.
  - Name your new repository (e.g., `my-registry-docs`) and choose whether it will be public or private.

- **Manual download**:
  - Download this repo as a ZIP and upload the contents to a new GitHub repo.
  - Or use `git clone` and rename the folder.

---

### 2. Customize Your Site Metadata

Open `mkdocs.yml` and update:

- `site_name`: The name of your registry or project.
- `site_url`: The final URL of your documentation site (optional during setup).
- `repo_url` and `repo_name`: If you want to link back to your GitHub repository from the site.
- Replace the logo in `assets/img/` with your registry’s logo and update the `logo:` path in `mkdocs.yml`.

---

### 3. Fill in the Content

All pages live in the `docs/` folder. Edit the following Markdown files to reflect your project:

| File | What to Include |
|------|------------------|
| `index.md` | Overview of your registry and what’s on the site |
| `data_dictionary.md` | Your full data dictionary or variable descriptions |
| `derived_fields.md` | Description of any calculated/derived fields |
| `irb.md` | IRB approval info, protocol number, ethics contact |
| `dua.md` | Summary or full text of your data use terms |
| `researchers.md` | Step-by-step instructions for requesting and using data |
| `faq.md` | Any common questions people may have |
| `acknowledgements.md` | Credit your contributors, funders, institutions |
| `key_resources.md` | Key references and external tools or policies |

Use plain Markdown or HTML, and feel free to add new pages as needed.

---

### 4. Preview Your Site Locally (Optional)

Have a technical team member run a local preview:

```bash
pip install mkdocs mkdocs-material
mkdocs serve
```

This starts a local server (usually at `http://127.0.0.1:8000`) where you can preview the documentation.

---

### 5. Deploy with GitHub Pages

This site is configured to deploy automatically with GitHub Actions. When you push changes to `main`, the workflow builds and updates your site at the GitHub Pages URL (e.g., `https://your-org.github.io/my-registry-docs/`).

To enable deployment:
- Go to your repo's **Settings > Pages**.
- Choose `GitHub Actions` as the source.
- Ensure that your `mkdocs.yml` and `.github/workflows/deploy.yml` are correctly configured.

---

### ✅ Need Help?
If you're new to MkDocs or run into issues:
- Visit the [MkDocs documentation](https://www.mkdocs.org/).
- Explore the [Material for MkDocs guide](https://squidfunk.github.io/mkdocs-material/).
- Check out [GitHub Actions documentation](https://docs.github.com/en/actions).

Happy documenting! 📝
