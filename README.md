# Asma-Ul-Husna Oishee — Portfolio

Academic and engineering portfolio built with Hugo Extended and Hugo Blox (Tailwind module v0.3.1).

Configured address: https://xtremeseoishee.github.io/Hugo_Portfolio/

## Local development

Install Hugo **Extended 0.138.0** and Go. From the repository root:

```powershell
hugo server --cacheDir "$PWD/.hugo-cache"
```

Open the URL printed by Hugo. A short cache path avoids Windows long-path failures in the Go module cache. The first build downloads pinned theme modules and needs network access.

Build without overwriting the existing tracked `public/` files:

```powershell
hugo --cacheDir "$PWD/.hugo-cache" --destination .preview-build --noBuildLock
```

## Content map

| Location | Purpose |
| --- | --- |
| `content/authors/admin/_index.md` | Biography, education, experience, skills and awards |
| `content/_index.md` | Homepage and selected work |
| `content/project/` | Case studies and earlier personal projects |
| `content/research/index.md` | Research and manuscript status |
| `content/cv/index.md` | Public CV |
| `static/uploads/Asma-Ul-Husna-Oishee-CV.pdf` | Original two-page CV supplied by Oishee; primary download |
| `static/uploads/Asma-Ul-Husna-Oishee-CV.md` | Text version aligned with the supplied PDF |
| `content/contacts/index.md` | Contact page |
| `config/_default/` | Site URL, navigation and appearance |
| `layouts/partials/hooks/head-end/portfolio-style.html` | Visual and print refinements |

The November 2026 update uses the supplied master CV as factual source material. Internal notes and academic referees were excluded from public content. Research metrics retain experimental limitations; manuscripts are not presented as accepted publications.

Template posts, teaching material, sample events and sample publications are retained as drafts and excluded from production builds. Earlier personal projects remain accessible but are no longer featured. The old resume PDF is excluded; the supplied current two-page PDF is the CV download.

## Deployment

`.github/workflows/publish.yaml` builds source and deploys to GitHub Pages on a push to `main` or manual workflow dispatch. Configure Pages source as GitHub Actions. The workflow uses the Pages-provided base URL for repository-subpath support.

The workflow builds into a fresh `.pages-build/` directory, generates the Pagefind search index there, and uploads that directory. Existing tracked `public/` output is not used for deployment.

## Outstanding information

- Hosted XAI Streamlit URL supplied and checked on 25 November 2026; linked on the XAI project page.
- GridWise: substantial nested documentation found; individual contribution needs confirmation before featuring.
- Jotno, electronic circuits and joystick-game links need confirmation.

Repository review notes and README drafts are maintained separately from the deployed portfolio source.

## Attribution

Based on the Hugo Blox Academic CV starter. Retain the supplied [MIT licence](LICENSE.md).
