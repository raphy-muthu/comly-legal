# comly-legal

Public legal pages for Comly, served by GitHub Pages at https://comly.app.

| URL | File |
| --- | --- |
| https://comly.app/terms | `terms/index.html` |
| https://comly.app/privacy | `privacy/index.html` |
| https://comly.app/delete-account | `delete-account/index.html` |
| https://comly.app/contact | `contact/index.html` |
| https://comly.app/ | `index.html` (App Store marketing URL) |
| https://comly.app/support | `support/index.html` (App Store support URL) |

`terms.html` and `privacy.html` are generated from `src/legal/content.ts` in the
private Comly app repo (`npm run legal:html`). Don't edit them here. Copy the
regenerated files over and commit.

`CNAME` sets the custom domain. `.nojekyll` stops GitHub from processing the files.

`terms.html` / `privacy.html` are identical copies kept so the `.html` URLs also work.
GitHub Pages serves a folder's `index.html` at the folder URL, which is why the
pages live in `terms/` and `privacy/`. Update all four files when the text changes.

`delete-account/index.html` is hand-written (Google Play's account-deletion URL). Keep it in line with section 10 of the Privacy Policy.

`support/index.html` is hand-written; its FAQ mirrors `HelpSupportScreen.tsx` in the app. `logo.png` and `favicon.png` are resized from the app's `assets/icon.png`.

When the App Store listing is live, change the "Coming soon to iPhone" badge in `index.html` to a link to the listing.
