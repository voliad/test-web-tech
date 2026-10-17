# Lumina Learn — COS10026 Project Part 1

A four-page recruitment website for a fictional G04 Educational Technology company. Built with HTML and CSS for COS10026 Part 1.

## Website and project links

- [Live website](https://voliad.github.io/test-web-tech/)
- [Deployment repository](https://github.com/voliad/test-web-tech)
- [Team repository linked from the website](https://github.com/NguyenHieu-P/PROJECT-WEB-COS10026)
- [Team Jira board](https://hyo2108.atlassian.net/jira/software/projects/SCRUM/boards/1) — access may require permission.

## Pages and responsibilities

| Page | Purpose | Assigned member |
| --- | --- | --- |
| `index.html` | Company introduction, image slider, job-search interface and career table | Lê Thu Phương |
| `jobs.html` | Two advertised roles, expandable descriptions and application steps | Nguyễn Minh Hiếu |
| `apply.html` | Application form with native HTML validation and CSS feedback | Trần Gia Cát Anh |
| `about.html` | Group information, responsibilities, quotes and fun facts | Bùi Đào Việt Anh |

Shared styling and navigation require coordination across all four pages. This table describes page ownership; Git history and project records provide evidence of actual contributions.

## Run locally

Open `index.html` in a browser, or serve this folder with a static web server. For example, if Python is installed:

```sh
python -m http.server 8780
```

Then open http://localhost:8780/. Keep the HTML files, `styles.css` and `images/` together. The stylesheet is **`styles.css`**, not `style.css`.

## Structure

```text
index.html
jobs.html
apply.html
about.html
styles.css
404.html
images/
README.md
```

Images with `-480`, `-768` and `-1200` suffixes are responsive variants referenced by `srcset`. They are intentional assets, not duplicate files to delete without updating the HTML.

## Missing pages (404)

This local-preview version uses relative paths. Open 404.html directly beside styles.css and the images/ folder; the navigation and recovery buttons also work from a local file.

A plain static server normally shows its own default error response for missing URLs. For GitHub Pages deployment, project-root paths (for example /test-web-tech/styles.css) are needed in the deployed 404 page so assets and recovery links also work at nested missing URLs. This local version is intended for direct file preview.

## Part 1 scope and limitations

- HTML/CSS only: no JavaScript, frameworks or recruitment backend.
- The search interface opens the Jobs page; keyword filtering is not implemented.
- Applying sends form fields to the university test endpoint, not a real employer. Use fictional details when testing.
- The optional CV control previews a filename only; the file is not uploaded or stored.
- Date-of-birth validation uses a documented static cutoff. Review its pattern and accompanying text when finalising a later submission; HTML/CSS does not calculate today's date dynamically.
- Social icons currently link to the platforms' homepages as temporary destinations.
- Complete the remaining verified student information and real team images before submission.

## Accessibility and checking

The website includes skip links, semantic headings and tables, form labels, keyboard-operated disclosures, visible focus states, reduced-motion styles, and a manually controlled radio slider. The mobile menu's accessible name follows its visible Menu/Close text. Slider arrow glyphs are hidden from assistive technology while the named radios remain available.

HTML/CSS validator results and browser checks support testing; they do not certify full WCAG conformance. Screen-reader speech and cross-browser checks should be included in the final review.

## Sources and acknowledgement

Content and code were assisted by OpenAI Codex and reviewed by the team. See `images/README.txt` for the supplied image-file provenance; it does not establish original authorship or licensing. Record the actual image source or generation tool and any sources used for job descriptions before submission.

This repository is a student project, not an operational recruitment service.
