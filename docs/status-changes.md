# Status Changes

Renames, archival notices, dormancy, and license gotchas affecting entries in this list. Last reviewed 2026-09-30.

## Renames / moves

- **Oils** — `oilshell/oil` renamed to `oils-for-unix/oils` (the project itself renamed Oil to Oils).
- **liquidprompt** — moved from `nojhan/liquidprompt` to its own org `liquidprompt/liquidprompt`.
- **zinit** — moved from `zdharma/zinit` to the community org `zdharma-continuum/zinit` after the maintainer left.
- **Ptyxis** — formerly named "Prompt"; renamed after a trademark conflict with Panic (per the author's GNOME blog, 2024-02-29). Canonical repo: `gitlab.gnome.org/chergert/ptyxis`.
- **pixcat** — `kristopolansky/pixcat` 404s; canonical is `mirukana/pixcat`.
- **libsixel** — `libsixel/libsixel` is an archived fork; the maintained repo is `saitoha/libsixel`.
- **gotty** — `yudai/gotty` stalled since 2017; this list uses the maintained fork `sorenisanerd/gotty`.
- **Terminology** — canonical upstream is `git.enlightenment.org`; `borisfaure/terminology` on GitHub is a mirror (used for stars).
- **Wave** — the repo is `wavetermdev/waveterm`; `wave/wave` is an unrelated profile-config repo.
- **Tilda** — the repo is `lanoxx/tilda`; `tilda/tilda` is an unrelated profile-config repo.
- **zsh** — `zsh-users/zsh` describes itself as a mirror; zsh.org lists SourceForge as the primary origin.

## Archived / dormant

- **Termite** — archived/unmaintained upstream; excluded.
- **Final Term** — abandoned before a stable release; excluded.
- **shellinabox** — dormant (last code commit 2019-01-28); excluded.
- **ueberzug** — upstream dead (name now resolves to an empty stub); excluded.
- **Black Box** — the GNOME-adjacent Rust terminal; verify current status before adopting (see repo).
- **Zutty** — deleted from GitHub; official source is now the self-hosted `git.hq.sig7.se/zutty.git`.

## License gotchas (verified on official sources)

- **zsh** — custom MIT-style "Zsh licence" with no SPDX identifier; recorded as `zsh`, not MIT.
- **Yakuake** — SPDX header is a disjunction (`GPL-2.0-only OR GPL-3.0-only OR LicenseRef-KDE-Accepted-GPL`); the first-listed identifier is recorded, full expression noted here. License read via KDE's official GitHub mirror (invent.kde.org requires login) — flagged unverified.
- **Konsole** — GPL-2.0-or-later, read via KDE's official GitHub mirror for the same reason — flagged unverified.
- **FluentTerminal** — LICENSE is generic GPLv3 text with no per-file "or later" grant; kept as GPL-3.0-only, unverified pending an authoritative grant statement.
- **foot** — MIT per the project's own documentation, but codeberg.org was unreachable from the research environment so the LICENSE text was not directly read — flagged unverified.
- **Eterm** — project page says "BSD License, MIT License" with no single SPDX id; `eterm.org` itself is unreachable (HTTP 500) — flagged unverified.
- **fish** — GPL-2.0-only (COPYING says "version 2", no "or later").
- **byobu** — GPL-3.0-only (source headers say "version 3", no "or later").
- **murex** — GPL-2.0-only per its LICENSE text (no "or later" statement).
- **liquidprompt** — AGPL-3.0-or-later (Affero; or-later per source headers).
- **mtm** — GPL-3.0-or-later verified from README and source headers (the repo ships no LICENSE file).
- **timg** — GPL-2.0-only; **lsix** — GPL-3.0-or-later; **chafa** — LGPL-3.0-or-later; **pixcat** — LGPL-3.0-only; **kitty** — GPL-3.0-only.
- **cool-retro-term** — the app is GPL-3.0-or-later (QML source headers); its bundled qmltermwidget submodule is GPL-2.0.
- **Tera Term** — BSD-3-Clause per the official manual's copyright page.
- **rxvt (original)** — GPL-2.0-only per the SourceForge project page (release tarball unretrievable, so "or later" could not be ruled in or out).
- **Nerd Fonts** — dual-licensed: patcher code MIT, patched fonts OFL-1.1; recorded MIT with the split in the description.
- **Hack** — MIT (relicensed 2018), not OFL as older third-party claims say.
- **Gruvbox** — ships no license file (GitHub license API 404s); recorded with a null license and a caveat.

## Naming notes (2026-09-30)

- **Wave** is the company/product name; the repo is `wavetermdev/waveterm`.
- **Oils** (not "Oil") is the current project name.
- **Ptyxis** is not related to Panic's Prompt app (the rename was forced by that conflict).
