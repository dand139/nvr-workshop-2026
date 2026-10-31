# NVR Workshop Dashboard — review prototype

Static bilingual FR/EN interface for the 2026 Tours workshop questionnaire.

## Run locally
From this folder run `python -m http.server 8000`, then open `http://localhost:8000`.

## Privacy warning — do not publish yet
`responses.json` contains **original unredacted free-text responses**, including personal anecdotes and descriptions of minors, families, institutions and allegations. The CSV metadata fields (timestamps, referrer names, owner email) were excluded. Before uploading to a public repository or enabling GitHub Pages, manually review and redact or obtain appropriate permission for each response. Public GitHub Pages makes the underlying JSON downloadable.

## Deployment after review
Create a GitHub repository, replace `responses.json` with the reviewed/redacted version, upload `index.html` and `responses.json`, and enable GitHub Pages from Settings → Pages → Deploy from branch → main / root. The interface is read-only for visitors, but GitHub repository collaborators can edit.

## Notes
The bilingual toggle displays English translations of French submissions (in `answers_en`); original responses remain in `answers`. English translations have not been approved by respondents. Qualitative themes are provisional observations, not formal coded findings. Quantitative bars count nonempty fields only. No personal metadata is published in the prototype data model.