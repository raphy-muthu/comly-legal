# comly-legal

Public legal pages for Comly, served by GitHub Pages at https://comly.app.

| URL | File |
| --- | --- |
| https://comly.app/terms | `terms/index.html` |
| https://comly.app/privacy | `privacy/index.html` |
| https://comly.app/ | `index.html` |

`terms.html` and `privacy.html` are generated from `src/legal/content.ts` in the
private Comly app repo (`npm run legal:html`). Don't edit them here. Copy the
regenerated files over and commit.

`CNAME` sets the custom domain. `.nojekyll` stops GitHub from processing the files.

`terms.html` / `privacy.html` are identical copies kept so the `.html` URLs also work.
GitHub Pages serves a folder's `index.html` at the folder URL, which is why the
pages live in `terms/` and `privacy/`. Update all four files when the text changes.
