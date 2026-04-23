# Ghostnote Labs — Studio Site

Business-focused context for this repo. Keep scope here to the **studio identity and legal pages** — this is not the product repo.

## What this repo is

The Ghostnote Labs studio website at https://ghostnotelabs.studio. Also hosts the public privacy policy + terms of service (served at `/privacy` and `/terms`).

- Org-root GitHub Pages repo (special name `ghostnote-labs/ghostnote-labs.github.io`).
- Custom domain `ghostnotelabs.studio` pointed via Cloudflare DNS.
- Single custom layout at `_layouts/default.html` — no Jekyll theme package. Dark palette pulled directly from the brand logo (bg `#111213`, text `#e8e2d4`, muted `#908070`, accent teal `#3db8a8`).

## Entity at a glance

| Field | Value |
|---|---|
| Legal name | Ghostnote Labs LLC |
| Entity | Oregon Domestic LLC, single-member |
| Oregon registry # | 255831597 |
| EIN | 42-1822270 |
| D-U-N-S | 145000069 |
| Principal address | 6210 SE Hazel St, Portland OR 97206 |
| Contact | ghostnotelabsllc@gmail.com |
| Sole member | Evan J. Smelser |

## Trademark caution rules — follow strictly

Unreleased product codenames and character names **must not appear in this public repo** until the underlying trademark work is complete. That includes this README, the landing page, the privacy policy, the terms of service, commit messages, and issue titles — anywhere content ends up indexable.

The game currently in private alpha has a product codename; it is not cleared for public use yet. Refer to it only generically on this site — e.g. "our first project," "a fitness role-playing game," "our in-development game." No specific name, no specific character names.

Canonical versions of the privacy policy + terms of service (which DO use real product names, for developer clarity) live in the private product repo under `docs/legal/`. When pulling an update from there into this repo, strip product-specific terms per the workflow below.

### Strip-before-publish workflow

1. Start from the canonical markdown in the private product repo's `docs/legal/`.
2. Replace every product-specific name with a generic placeholder:
   - Product codename → `the App` or `our mobile application`
   - Character names → `the AI familiar`, `characters`
3. Preserve Jekyll frontmatter (`---\nlayout: default\ntitle: ...\npermalink: /...\n---`).
4. Commit + push to `main`. Pages rebuilds within ~1 minute.

Restore real names when USPTO trademark for the product name is filed and cleared, OR public announcement / Kickstarter campaign launches (whichever is sooner).

## Visual + voice language

From the parent project's GDD: "stone and shadow, muted textures, gold and deep earth tones, power contained rather than flashy." Apply the same sensibility here.

- Copy is restrained — no breathless marketing language, no exclamation points, no buzzwords.
- Palette is dark + warm; teal accent comes from the logo and should stay on the accent role (links, small emphasis), not broad surfaces.
- Typography leans sans-serif body. Serif display is fine if it's clean; avoid decorative scripts.
- No stock photography. Illustrative assets only if they match the hand-crafted / ascetic tone.

## Publishing / ops

- Push to `main` → GitHub Pages rebuilds on its own. Free.
- DNS managed at Cloudflare Registrar (domain registered there too). **No AWS resources are or should be provisioned for this site.** The hosting model is intentionally GitHub Pages — free, simple, sufficient. If this ever needs to migrate to a self-hosted CDN (unlikely for an indie studio site), any cloud resources MUST be defined via Pulumi IaC, not manually created in any console — same standard as the product backend. Until then, there is nothing to provision.
- Pages enforces HTTPS automatically.
- 404s currently return the GitHub default page — fine for now, custom `404.md` is a future polish.

## Things NOT in scope for this repo

- Product marketing pages for any specific game (live on a separate product domain once trademark clears, e.g. `numen.app`).
- Blog / press / company news (add later if there's actual content to post).
- Recruiting / careers pages (nobody's hiring; add when that changes).
- Contact forms (mailto link to the LLC email is sufficient at this stage).

## Related repos

- `ghostnote-labs/legal` — being retired; content migrated here. Can be archived.
- Product codebase (private) — canonical legal docs live there under `docs/legal/`.
