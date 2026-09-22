# My TourBee

Website for My TourBee international tour packages, with an admin panel and visa guides for Indian passport holders.

## Files
- `index.html` — the public site.
- `admin.html` — the admin panel (sign in, edit packages and visa guides, upload photos, publish).
- `data.json` — all editable content: packages, visa guides and contact details. `index.html` and `admin.html` both read this file.
- `images/` — the brand logo and mascot (used by `index.html` itself; not needed for package photos any more — those are now uploaded through the admin panel and stored inside `data.json`).

## Using the admin panel
1. Put all files on GitHub Pages (see below) — the admin panel needs to be opened through a web address, not by double-clicking the file, because it loads `data.json` over the network.
2. Go to `https://<your-pages-url>/admin.html`.
3. Sign in with username `admin` and password `TourBee@2026`. **Change this password immediately** from the Site settings tab.
4. Edit packages, visa guides, WhatsApp number and email from the tabs.
5. Go to **Save & publish**:
   - **Download data.json** always works — download it, then upload it to your GitHub repo to replace the existing `data.json` (Add file → Upload files → Commit).
   - **Publish to GitHub** saves changes straight to your repo, if you give it a GitHub personal access token (Settings → Developer settings → Fine-grained tokens → give it Contents: Read and write, scoped to this repo only). The token is stored only in your own browser.

## Security note
This is a static website with no server of its own, so the login is a convenience gate, not bank-grade security — someone who reads the page's source code could find a way around it. The real protection is the GitHub token, which only you hold. Use a strong password, don't share the token, and use a fine-grained token limited to this one repository.

## Hosting
Host free with GitHub Pages: Settings → Pages → Deploy from branch → `main` / root. The site appears at `https://kumarbluebill-sudo.github.io/MTB/` within a few minutes, and the admin panel at `.../admin.html`.

Visa information in `data.json` was checked on 21 September 2026 and must be re-verified against official sources before use.
