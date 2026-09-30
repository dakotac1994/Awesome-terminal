# Contributing to Awesome-terminal

Thanks for helping keep this list accurate. This repo has strict honesty rules — please read them before opening a PR.

## What belongs here

- The terminal **stack**: terminal emulators, multiplexers, shells, prompt engines, shell frameworks/plugin managers, terminal UX infrastructure (image display, image protocols, terminal-aware dotfile management), terminal fonts, color schemes, remote/web terminals.
- Pure CLI/TUI utilities (file managers, fuzzy finders, git UIs, editors, system monitors) are **out of scope** — they belong in [awesome-cli](https://github.com/dakotac1994/awesome-cli) / [awesome-oss-cli](https://github.com/dakotac1994/awesome-oss-cli).

## Entry requirements (all must hold)

1. **Real and verifiable.** The project must exist at the linked URL. `verified` is `true` only if you confirmed the entry on an official source (the project's repo, LICENSE file, or official site) — never from a blog roundup alone.
2. **Honest license.** Copy the SPDX identifier from the project's actual LICENSE file. Proprietary emulators are `"proprietary"` — never imply a paid product is open source. If the license can't be confirmed, set `"license": null`, `"verified": false`, and explain in `"unverified_reason"`.
3. **No invented facts.** No guessed star counts or descriptions. If you can't verify it, leave it `null` and say why.
4. **One category each.** Pick the single best-fitting `category`.

## How to add an entry

1. Add the entry to `data/terminal.json` (keep the file's existing ordering: grouped by category):
   ```json
   {
     "name": "Example Term",
     "description": "One-line description, no hype.",
     "license": "MIT",
     "category": "gpu-accelerated",
     "repo": "https://github.com/org/example-term",
     "homepage": "https://example-term.org",
     "official_site": "https://example-term.org",
     "stars": 1234,
     "verified": true,
     "unverified_reason": null
   }
   ```
   Use `null` (not `""`) for unknown `repo`/`official_site`/`stars`/`unverified_reason`.
2. Add the matching bullet to the right section in `README.md`: `- [Example Term](https://example-term.org) — one-line description.`
3. Run the CI validation locally if you can (`python` 3.12+, see `.github/workflows/ci.yml`): it checks JSON validity, duplicate names/URLs, the README↔JSON cross-check, section counts, and TOC anchors.
4. Open a PR describing what you verified and where (link the official source).

## Link hygiene

- Prefer `https://` URLs; no URL shorteners.
- If a project renamed/moved, update to the canonical URL and note it in `docs/status-changes.md`.
- Commercial product links should point at official docs or pricing pages, not marketing landing pages, where possible.

## What gets rejected

- Entries with invented licenses, stars, or descriptions.
- Proprietary products presented as open source.
- Pure CLI/TUI utilities (wrong list), dead links, or projects you can't confirm exist.
