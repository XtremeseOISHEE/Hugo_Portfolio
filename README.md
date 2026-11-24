# Asma-Ul-Husna Oishee — Personal Portfolio

My academic and software engineering portfolio, featuring student research, selected projects, education, leadership, certifications and creative activities.

**[Visit the live portfolio →](https://xtremeseoishee.github.io/Hugo_Portfolio/)**

## About

I am a master’s student in Computer Science and Engineering at Jahangirnagar University, Bangladesh. My interests include explainable AI, evidence-grounded reasoning, applied machine learning and intelligent systems. I also build Android applications, web software and wearable IoT prototypes.

## Explore the website

| Section | What you will find |
| --- | --- |
| About | Introduction, interests and featured work |
| Research | Explainable Clinical AI, BeyondFall and manuscript status |
| Projects | Project descriptions, contributions, screenshots, source code and available demos |
| Experience | Student research, leadership, technical skills, selected certifications and languages |
| Education | University education, coursework and scholarships |
| CV | Readable online CV and the current two-page PDF download |
| Beyond Academics | Milestones in writing, sport, creativity and community service |
| Contact | Email, professional profiles and social links |

## Featured work

- **[Multi-hop Explainable AI](https://github.com/XtremeseOISHEE/Thesis_4-2)** — retrieval-augmented clinical reasoning with per-hop evidence verification. [Streamlit demo](https://thesis4-2git-bdtpsgjip26eytq4wfqwbf.streamlit.app/)
- **[BeyondFall](https://github.com/XtremeseOISHEE/Beyond-Fall)** — wearable fall-detection research prototype with an Android companion. [ESP32 firmware](https://github.com/XtremeseOISHEE/Beyond-Fall-Arduino-Code-for-IOT-)
- **[AirSense Dhaka](https://github.com/XtremeseOISHEE/Air-Index-Prediction)** — PM2.5 forecasting experiments and historical pollution analysis.
- **[RotaShift](https://github.com/XtremeseOISHEE/RotaShift)** — an evidence-transparent crop-calendar prototype using NASA POWER climate records.
- **[FlowOrbit](https://github.com/XtremeseOISHEE/FlowOrbit)** — Android productivity app with focus sessions, tasks and usage insights.
- **[ArtNest](https://github.com/XtremeseOISHEE/Art-Gallery)** — Django-based artwork e-commerce platform built by a four-member team.

The project gallery also includes Tender Document Package Builder, Smart Escape, an ESP32 firefighting robot and earlier coursework. Research and prototype limitations are stated on the relevant pages; clinical validation and accepted publication status are not implied.

## Built with

- Hugo **Extended 0.138.0**
- Hugo Blox Academic CV starter and Tailwind module **v0.3.1**
- Markdown and YAML content, custom Hugo templates and CSS
- Pagefind for site search
- GitHub Actions and GitHub Pages for publishing

The site supports light and dark themes, responsive project cards, real project screenshots, embedded demonstrations and a downloadable CV.

## Run locally

Install Hugo Extended and Go. Node.js/npm are also needed to generate the search index.

```powershell
git clone https://github.com/XtremeseOISHEE/Hugo_Portfolio.git
cd Hugo_Portfolio
hugo server --cacheDir "$PWD/.hugo-cache"
```

Open the local address printed by Hugo. The first build downloads the pinned theme modules and requires network access. On Windows, keeping the cache path short helps avoid Go module path-length errors. Restart the server after configuration changes if needed.

## Production build

```powershell
hugo --environment production --minify --cacheDir "$PWD/.hugo-cache" --destination .pages-build
npx --yes pagefind --site .pages-build
```

The output is written to `.pages-build/`. Local Hugo preview does not automatically regenerate the Pagefind index.

## Editing content

| Location | Purpose |
| --- | --- |
| `content/_index.md` | Homepage sections and featured collection |
| `content/authors/admin/_index.md` | Biography, research, leadership, skills and selected certifications |
| `content/project/<project>/index.md` | Individual project page |
| `content/project/<project>/featured.*` | Project cover image |
| `content/research/`, `content/education/`, `content/beyond-academics/` | Research, academic background and personal milestones |
| `content/cv/index.md` | Online CV |
| `static/uploads/Asma-Ul-Husna-Oishee-CV.pdf` | Current downloadable PDF |
| `content/contacts/index.md` | Contact and social links |
| `config/_default/menus.yaml` | Navigation order |
| `config/_default/params.yaml` | Theme and site settings |
| `layouts/` | Custom page layouts, cards and styles |
| `static/images/` | Homepage background textures |
| `assets/media/icon.png` | Browser tab icon |

Projects are ordered by ascending `weight`; `featured: true` includes a project in the homepage selection. Keep PDF and online CV content aligned when updating them. Original template examples are retained as drafts and excluded from production.

## Deployment

Publishing is handled by [the GitHub Pages workflow](.github/workflows/publish.yaml).

1. Push reviewed source changes to `main`, or run the workflow manually from GitHub Actions.
2. The workflow builds Hugo into `.pages-build/`, generates the Pagefind index and uploads the result.
3. GitHub Pages publishes the artifact at **https://xtremeseoishee.github.io/Hugo_Portfolio/**.

The repository’s Pages source is **GitHub Actions**. The workflow supplies the correct repository base URL. Previously generated files under `public/` are not used for deployment; edit the source files instead.

## Contact

[Email](mailto:asmaul4husna94oishee@gmail.com) · [GitHub](https://github.com/XtremeseOISHEE) · [LinkedIn](https://www.linkedin.com/in/asma-ul-husna-oishee-57714a229/)

## Credits

Based on the Hugo Blox Academic CV starter. See [LICENSE.md](LICENSE.md) for the supplied code licence. Project screenshots, app icons, photographs and background artwork retain their respective ownership and usage terms.
