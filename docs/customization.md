# Data Sharing In A Box

!!! warning "Sample Content Only"
    This page contains **example language and placeholders** designed to help registry teams build their own data sharing site.  
    Please **replace all placeholder text** with details specific to your own project, policies, and governance requirements.
    
## ☀️ How to Set Up and Use the Patient Registry Template

This template helps patient registry teams create a public-facing website to share data documentation, governance policies, and data access instructions. It’s built using [MkDocs](https://www.mkdocs.org/) with the [Material theme](https://squidfunk.github.io/mkdocs-material/).

### 1. Copy This Template Repository

You have two options:

- **Use GitHub’s “Use this template” button** (recommended):
  - Go to the [template repository](https://github.com/BoyceLab/DataSharingInABox/tree/main).
  - Click **"Use this template"** in the upper right to create your own copy.
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
- Replace `logo.png` in `assets/img/` with your registry’s logo and update the paths in `mkdocs.yml`.

---

### 3. Fill in the Content

All pages live in the `docs/` folder. Edit the following Markdown files to reflect your project:

| File | What to Include |
|------|------------------|
| `index.md` | Overview of your registry and what’s on the site |
| `data_dictionary.md` | Your full data dictionary or variable descriptions |
| `derived_fields.md` | Description of any calculated/derived fields |
| `irb.md` | IRB approval info, protocol number, ethics contact |
| `data_use_agreement.md` | Summary or full text of your data use terms |
| `access_data.md` | Instructions for how to request the data |
| `faq.md` | Any common questions people may have |
| `acknowledgements.md` | Credit your contributors, funders, institutions |

Use plain Markdown or HTML, and feel free to add new pages as needed.

---

### 4. Preview Your Site Locally (Optional)

Have a technical team member run a local preview:

```bash
pip install mkdocs mkdocs-material
mkdocs serve
