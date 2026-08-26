# AI Learning Notes

A personal AI learning blog built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) and deployed to GitHub Pages.

## Local development

Requires Python 3.10 or newer.

```bash
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Open <http://127.0.0.1:8000/>. MkDocs reloads the site when files change.

## Add content

- Add topic-based notes under `docs/notes/` and include them in `nav` in `mkdocs.yml`.
- Add dated blog posts under `docs/blog/posts/`. Copy the front matter from the example post.
- Preview changes locally with `mkdocs serve`.

## Deployment

A push to `main` triggers `.github/workflows/pages.yml`. The workflow builds the site and deploys it with GitHub's official Pages actions. It can also be started manually from the repository's **Actions** tab.

In the repository's **Settings → Pages**, ensure **Source** is set to **GitHub Actions**.
