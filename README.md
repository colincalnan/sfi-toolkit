# Safe Family Internet — Family Toolkit

The parent setup guides from the June 18 Safe Family Internet night (Lake Country),
hosted for the email-gated toolkit. Served as a static site via GitHub Pages.

- `index.html` — the branded toolkit page (the "full toolkit" link).
- `castle-model.pdf` / `screen-time.pdf` / `homeshield.pdf` / `dns.pdf` — the guides.

## Publish (GitHub Pages)
1. Create a public repo, push this folder.
2. Repo Settings → Pages → Source: Deploy from branch → `main` / root.
3. URLs become:
   - Toolkit page: `https://<user>.github.io/<repo>/`
   - A guide: `https://<user>.github.io/<repo>/screen-time.pdf`
4. (Optional) Point `downloads.safefamilyinternet.ca` at it with a CNAME for branded links.

Then drop those URLs into the pledge-email placeholders (`PASTE_*`) in
`scripts/gen_pledge_emails.py` and re-run it.

The gate is the pledge form plus the attribution footer on each PDF, not secrecy
(see wiki/concepts/sfii/pdf-gating.md).
