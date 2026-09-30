# Awesome Terminal

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Entries](https://img.shields.io/badge/entries-104-blue)](data/terminal.json)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

A curated list of the **terminal stack**: terminal emulators (the core of this list), multiplexers, shells, prompt engines, shell frameworks, terminal UX infrastructure, fonts, color schemes, and remote/web terminals.

> **Scope:** this list covers the terminal *stack* — emulators, multiplexers, shells, prompts, and the UX layer around them. Pure CLI/TUI utilities (file managers, fuzzy finders, git UIs, editors, system monitors) belong in [awesome-cli](https://github.com/dakotac1994/awesome-cli) and [awesome-oss-cli](https://github.com/dakotac1994/awesome-oss-cli), even when they run in a terminal. Overlap with those lists is intentional only where the tool *is* terminal infrastructure (multiplexers, shells, prompts).
> **Honesty policy:** every entry was checked against an official source (project repo, LICENSE file, or official site) as of 2026-09-30 — **99/104 verified**. Unverified entries carry a stated reason. Proprietary products are explicitly labeled `"proprietary"` and never presented as open source. Machine-readable data lives in [`data/terminal.json`](data/terminal.json).

## Contents

- [GPU-Accelerated Emulators](#gpu-accelerated-emulators) — 7 entries
- [Electron & Web-Based Emulators](#electron--web-based-emulators) — 5 entries
- [Linux Desktop-Integrated Emulators](#linux-desktop-integrated-emulators) — 15 entries
- [Classic & Minimal Emulators](#classic--minimal-emulators) — 8 entries
- [Windows & macOS Emulators](#windows--macos-emulators) — 12 entries
- [Terminal Multiplexers](#terminal-multiplexers) — 7 entries
- [Shells](#shells) — 9 entries
- [Prompts & Prompt Engines](#prompts--prompt-engines) — 6 entries
- [Shell Frameworks & Plugin Managers](#shell-frameworks--plugin-managers) — 8 entries
- [Terminal UX](#terminal-ux) — 7 entries
- [Fonts](#fonts) — 7 entries
- [Color Schemes](#color-schemes) — 8 entries
- [Remote & Web Terminals](#remote--web-terminals) — 5 entries

## Choosing the right terminal

New here? Start with the [choosing-a-terminal](docs/choosing-a-terminal.md) guide (GPU vs integrated vs minimal, per-platform picks, emulator vs multiplexer, licensing notes), the [glossary](docs/glossary.md), and [status-changes](docs/status-changes.md) (renames, archival notices, license gotchas).

## GPU-Accelerated Emulators

Modern emulators that render on the GPU — the performance frontier: low-latency input, smooth high-refresh scrolling, and native image protocols. If you are picking one emulator in 2026, start here. (7 entries)

- [Ghostty](https://ghostty.org) — Fast, feature-rich terminal emulator with GPU acceleration and native OS integration. *(MIT · ⭐ 61,736)*
- [WezTerm](https://wezterm.org) — GPU-accelerated terminal emulator and multiplexer with built-in tabs, panes, and SSH. *(MIT · ⭐ 29,082)*
- [Alacritty](https://alacritty.org) — Fast, cross-platform OpenGL terminal emulator focused on simplicity and performance. *(Apache-2.0 · ⭐ 65,868)*
- [kitty](https://sw.kovidgoyal.net/kitty/) — GPU-based terminal emulator with tabs, tiling, image display, and extensive configurability. *(GPL-3.0-only · ⭐ 35,130)*
- [Rio](https://rioterm.com) — Hardware-accelerated terminal emulator built in Rust, targeting a modern out-of-box experience. *(MIT · ⭐ 7,566)*
- [Contour](https://contour-terminal.org) — Modern C++ terminal emulator with GPU-accelerated text rendering. *(Apache-2.0 · ⭐ 3,035)*
- [foot](https://codeberg.org/dnkl/foot) — Fast, lightweight Wayland-native terminal emulator with sixel support. *(MIT · ⭐ 2,234)*

## Electron & Web-Based Emulators

Emulators built on web technology — maximum extensibility and a familiar hacking surface, trading some resource efficiency for it. (5 entries)

- [Tabby](https://tabby.sh) — Highly customizable cross-platform terminal app with SSH, serial, and plugin support. *(MIT · ⭐ 74,760)*
- [Hyper](https://hyper.is) — Extensible terminal built on web technologies (Electron) with a plugin ecosystem. *(MIT · ⭐ 44,743)*
- [Wave](https://www.waveterm.dev) — Open-source AI-native terminal with workspaces, widgets, and session persistence. *(Apache-2.0 · ⭐ 22,390)*
- [Electerm](https://electerm.github.io) — Terminal/SSH/SFTP client with sync, themes, and a built-in file manager. *(MIT · ⭐ 15,236)*
- [Extraterm](https://extraterm.org) — Terminal emulator that adds images, rich text, and GUI controls to shell output. Actively maintained (commits 2026). *(MIT · ⭐ 2,826)*

## Linux Desktop-Integrated Emulators

Emulators that ship with or target Linux desktop environments — deep DE integration, dropdown (quake-style) modes, and tiling-friendly workflows. (15 entries)

- [GNOME Terminal](https://apps.gnome.org/Terminal/) — Default terminal emulator for the GNOME desktop. *(GPL-3.0-or-later · ⭐ 72)*
- [GNOME Console](https://apps.gnome.org/Console/) — Simple, modern terminal for GNOME, focused on a clean uncluttered UI. *(GPL-3.0-or-later · ⭐ 75)*
- [Konsole](https://apps.kde.org/konsole/) — KDE's feature-rich terminal emulator with tabs, profiles, and split views. *(GPL-2.0-or-later)*
- [Yakuake](https://apps.kde.org/yakuake/) — Drop-down (Quake-style) terminal emulator for KDE, based on Konsole technology. *(GPL-2.0-only)*
- [Tilix](https://gnunn1.github.io/tilix-web/) — Tiling terminal emulator for GNOME with layouts, tabs, and synchronized input. *(MPL-2.0 · ⭐ 5,724)*
- [Terminator](https://gnome-terminator.org) — Terminal emulator supporting multiple resizable terminals in one window. *(GPL-2.0-only · ⭐ 2,673)*
- [Guake](https://guake.github.io) — Drop-down terminal for GNOME inspired by Quake consoles. *(GPL-2.0-or-later · ⭐ 4,671)*
- [QTerminal](https://github.com/lxqt/qterminal) — Lightweight Qt terminal emulator, part of LXQt. *(GPL-2.0-or-later · ⭐ 717)*
- [Tilda](https://github.com/lanoxx/tilda) — Highly configurable GTK drop-down terminal. *(GPL-2.0-or-later · ⭐ 1,338)*
- [Xfce4 Terminal](https://docs.xfce.org/apps/terminal/start) — Lightweight terminal emulator for the Xfce desktop. *(GPL-2.0-or-later · ⭐ 44)*
- [Ptyxis](https://apps.gnome.org/Ptyxis/) — Modern container-focused terminal for GNOME (renamed from Prompt after a trademark conflict). *(GPL-3.0-or-later · ⭐ 123)*
- [Black Box](https://gitlab.gnome.org/raggesilver/blackbox) — Stylish GTK4 terminal emulator for GNOME. *(GPL-3.0-or-later · ⭐ 152)*
- [Sakura](https://github.com/dabisu/sakura) — Simple GTK terminal emulator with tabs. *(GPL-2.0-only · ⭐ 230)*
- [Terminology](https://www.enlightenment.org/about-terminology) — Enlightenment's terminal emulator with rich media display and visual flair. *(BSD-2-Clause · ⭐ 737)*
- [cool-retro-term](https://github.com/Swordfish90/cool-retro-term) — Terminal emulator mimicking the look and feel of old cathode-ray tube screens. Actively maintained (2026). *(GPL-3.0-or-later · ⭐ 26,466)*

## Classic & Minimal Emulators

The old guard and the minimalists: decades-old X11 workhorses and suckless-style terminals that do one thing fast. (8 entries)

- [xterm](https://invisible-island.net/xterm/) — The reference terminal emulator for the X Window System. *(MIT)*
- [rxvt](https://sourceforge.net/projects/rxvt/) — Lightweight vt102 terminal emulator for X; dormant since 2.6.4 (2003). *(GPL-2.0-only)*
- [rxvt-unicode](http://dist.schmorp.de/rxvt-unicode/) — Unicode-aware, daemon-capable fork of rxvt (urxvt). *(GPL-3.0-or-later)*
- [aterm](https://sourceforge.net/projects/aterm/) — rxvt-based terminal with fast transparency, aimed at AfterStep users. *(GPL-2.0-or-later)*
- [Eterm](https://sourceforge.net/projects/eterm/) — Enlightenment's color vt102 terminal emulator with themes and configurability. *(MIT)*
- [mlterm](https://github.com/arakiken/mlterm) — Multilingual terminal emulator with input-method, bidi, and RTL support. *(BSD-3-Clause · ⭐ 236)*
- [st](https://st.suckless.org/) — suckless's simple, minimal terminal emulator for X. *(MIT)*
- [Zutty](https://www.zutty.org/) — Efficient, low-latency X11 terminal emulator; removed from GitHub, now self-hosted. *(GPL-3.0-or-later)*

## Windows & macOS Emulators

Platform-native and platform-first emulators for Windows and macOS. Proprietary products are explicitly labeled. (12 entries)

- [Windows Terminal](https://github.com/microsoft/terminal) — Microsoft's modern multi-shell terminal for Windows. *(MIT · ⭐ 105,038)*
- [ConEmu](https://conemu.github.io) — Customizable Windows console emulator with tabs and splits. *(BSD-3-Clause · ⭐ 9,265)*
- [Cmder](https://cmder.app) — Portable console emulator for Windows bundling ConEmu, Clink, and Git-for-Windows. *(MIT · ⭐ 27,010)*
- [mintty](https://mintty.github.io) — Terminal emulator for Cygwin, MSYS2, and WSL. *(GPL-3.0-or-later · ⭐ 1,789)*
- [PuTTY](https://www.putty.org/) — Free SSH and Telnet client for Windows and Unix. *(MIT)*
- [Tera Term](https://teratermproject.github.io/) — Long-running open-source terminal emulator for Windows with SSH and macro scripting. *(BSD-3-Clause · ⭐ 1,060)*
- [MobaXterm](https://mobaxterm.mobatek.net/) — Enhanced Windows terminal with X11 server, tabbed SSH, and network tools (freemium: Home free, Professional paid). *(proprietary)*
- [SecureCRT](https://www.vandyke.com/products/securecrt/) — Commercial rock-solid SSH/Telnet client for Windows, macOS, and Linux (30-day evaluation). *(proprietary)*
- [FluentTerminal](https://github.com/felixse/FluentTerminal) — Modern UWP-style terminal emulator for Windows. Actively maintained (2025). *(GPL-3.0-only · ⭐ 9,604)*
- [iTerm2](https://iterm2.com/) — Feature-rich terminal emulator for macOS. *(GPL-2.0-only · ⭐ 18,107)*
- [Warp](https://www.warp.dev/) — AI-powered commercial terminal for macOS and Linux (freemium: Free/Build/Max/Business/Enterprise tiers). *(proprietary)*
- [Royal TSX](https://www.royalapps.com) — Commercial remote-management app for macOS with an iTerm2-based terminal plugin (shareware mode free with limits). *(proprietary)*

## Terminal Multiplexers

Session persistence, panes, windows, and detachable workspaces that live inside any emulator. (7 entries)

- [tmux](https://github.com/tmux/tmux) — Terminal multiplexer: multiple panes and windows in one terminal, with detachable sessions. *(ISC · ⭐ 49,591)*
- [zellij](https://zellij.dev) — A terminal workspace with batteries included: multiplexer with layouts, plugins, and floating panes. *(MIT · ⭐ 35,601)*
- [GNU screen](https://www.gnu.org/software/screen/) — The classic full-screen terminal multiplexer from the GNU project. *(GPL-3.0-or-later)*
- [byobu](https://byobu.org) — Text-based window manager and terminal multiplexer: elegant profiles and status over GNU Screen or tmux. *(GPL-3.0-only · ⭐ 1,721)*
- [tmate](https://tmate.io/) — Instant terminal sharing: a tmux fork for remote pair-programming sessions. *(ISC · ⭐ 6,130)*
- [abduco](https://www.brain-dump.org/projects/abduco/) — Session management (detach/reattach) for programs; with dvtm a minimal, cleaner tmux/screen alternative. *(ISC · ⭐ 988)*
- [mtm](https://github.com/deadpixi/mtm) — Perhaps the smallest useful terminal multiplexer in the world. *(GPL-3.0-or-later · ⭐ 1,226)*

## Shells

The command interpreters themselves — from POSIX workhorses to structured-data shells. (9 entries)

- [bash](https://www.gnu.org/software/bash/) — The GNU Bourne-Again SHell: the default login shell on most Linux systems. *(GPL-3.0-or-later)*
- [zsh](https://www.zsh.org) — A shell designed for interactive use, although it is also a powerful scripting language. *(custom MIT-style license — see notes · ⭐ 4,305)*
- [fish](https://fishshell.com) — The user-friendly command-line shell with autosuggestions and sane scripting. *(GPL-2.0-only · ⭐ 34,247)*
- [nushell](https://www.nushell.sh/) — A new type of shell: pipelines carry structured data, not just text. *(MIT · ⭐ 40,593)*
- [elvish](https://elv.sh/) — Powerful scripting language and versatile interactive shell. *(BSD-2-Clause · ⭐ 6,383)*
- [xonsh](http://xon.sh) — Python-powered, full-featured, cross-platform shell blending Python and shell syntax. *(BSD-2-Clause · ⭐ 9,657)*
- [PowerShell](https://microsoft.com/PowerShell) — Cross-platform task automation shell and scripting language from Microsoft. *(MIT · ⭐ 55,556)*
- [Oils](https://oils.pub/) — Upgrade path from bash to a better language and runtime (formerly Oil). *(Apache-2.0 · ⭐ 3,397)*
- [murex](https://murex.rocks) — A smarter shell and scripting environment designed for usability, safety, and productivity. *(GPL-2.0-only · ⭐ 1,915)*

## Prompts & Prompt Engines

Fast, informative, cross-shell prompt renderers. (6 entries)

- [starship](https://starship.rs) — The minimal, blazing-fast, infinitely customizable prompt for any shell. *(ISC · ⭐ 60,104)*
- [oh-my-posh](https://ohmyposh.dev) — The most customizable and low-latency cross-platform/shell prompt renderer. *(MIT · ⭐ 23,529)*
- [powerlevel10k](https://github.com/romkatv/powerlevel10k) — A fast, flexible Zsh theme with instant prompt. *(MIT · ⭐ 55,171)*
- [spaceship-prompt](https://spaceship-prompt.sh) — Minimalistic, powerful, and extremely customizable Zsh prompt. *(MIT · ⭐ 20,577)*
- [liquidprompt](https://liquidprompt.readthedocs.io/) — A full-featured and carefully designed adaptive prompt for Bash and Zsh. *(AGPL-3.0-or-later · ⭐ 4,678)*
- [pure](https://github.com/sindresorhus/pure) — Pretty, minimal, and fast ZSH prompt. *(MIT · ⭐ 14,433)*

## Shell Frameworks & Plugin Managers

Plugin ecosystems and configuration frameworks for zsh, fish, and bash. (8 entries)

- [oh-my-zsh](https://ohmyz.sh) — A delightful community-driven framework for managing zsh configuration (300+ plugins, 140+ themes). *(MIT · ⭐ 190,005)*
- [prezto](https://github.com/sorin-ionescu/prezto) — The configuration framework for Zsh. *(MIT · ⭐ 14,570)*
- [fisher](https://git.io/fisher) — A plugin manager for Fish. *(MIT · ⭐ 9,431)*
- [zinit](https://github.com/zdharma-continuum/zinit) — Flexible and fast ZSH plugin manager. *(MIT · ⭐ 4,865)*
- [bash-it](https://github.com/Bash-it/bash-it) — A community Bash framework. *(MIT · ⭐ 15,265)*
- [oh-my-fish](https://github.com/oh-my-fish/oh-my-fish) — The Fish Shell framework. *(MIT · ⭐ 11,391)*
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) — Fish-like autosuggestions for zsh. *(MIT · ⭐ 36,100)*
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) — Fish shell-like syntax highlighting for zsh. *(BSD-3-Clause · ⭐ 23,017)*

## Terminal UX

Infrastructure that upgrades the terminal experience itself: inline image display, image protocols, and terminal-aware dotfile management. (7 entries)

- [chafa](https://hpjansson.org/chafa/) — Image-to-ANSI/Unicode art converter plus a C library API; the most capable terminal image renderer. *(LGPL-3.0-or-later · ⭐ 5,289)*
- [viu](https://github.com/atanunq/viu) — Terminal image viewer with native support for the iTerm2, Kitty, and sixel graphics protocols. *(MIT · ⭐ 3,286)*
- [timg](https://github.com/hzeller/timg) — Terminal image and video viewer (sixel/kitty/iTerm2 graphics) built on ImageMagick/GraphicsMagick. *(GPL-2.0-only · ⭐ 2,769)*
- [lsix](https://github.com/hackerb9/lsix) — Like ls, but for images — shows thumbnails in the terminal using sixel. *(GPL-3.0-or-later · ⭐ 4,175)*
- [pixcat](https://github.com/mirukana/pixcat) — CLI and Python API for displaying images on Kitty terminals via the Kitty graphics protocol. *(LGPL-3.0-only · ⭐ 54)*
- [libsixel](https://github.com/saitoha/libsixel) — C encoder/decoder for the SIXEL image protocol — the infrastructure behind sixel terminal graphics. *(MIT · ⭐ 2,851)*
- [chezmoi](https://www.chezmoi.io/) — Dotfile manager across diverse machines — the terminal-config-relevant pick for managing shell/terminal setup. *(MIT · ⭐ 21,781)*

## Fonts

Monospaced fonts built for the terminal — ligatures, symbol coverage, and legibility at small sizes. (7 entries)

- [Nerd Fonts](https://www.nerdfonts.com) — Iconic font aggregator and patcher (3,600+ glyphs); patcher code MIT, patched fonts OFL-1.1 (dual licensing). *(MIT · ⭐ 64,774)*
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) — JetBrains' free monospace typeface for developers, with increased x-height for code readability. *(OFL-1.1 · ⭐ 13,053)*
- [Fira Code](https://github.com/tonsky/FiraCode) — Free monospaced font with programming ligatures. *(OFL-1.1 · ⭐ 82,075)*
- [Cascadia Code](https://github.com/microsoft/cascadia-code) — Microsoft's monospaced font with programming ligatures (Windows Terminal default). *(OFL-1.1 · ⭐ 27,909)*
- [Iosevka](https://typeof.net/Iosevka/) — Versatile, highly customizable typeface for code, from code. *(OFL-1.1 · ⭐ 22,797)*
- [IBM Plex Mono](https://www.ibm.com/plex/) — IBM's corporate monospace typeface, open-sourced. *(OFL-1.1 · ⭐ 11,664)*
- [Hack](https://sourcefoundry.org/hack/) — Typeface designed for source code (a DejaVu/Bitstream Vera derivative); project work MIT-licensed. *(MIT · ⭐ 17,360)*

## Color Schemes

The notable terminal color schemes. Apply once, enjoy everywhere. (8 entries)

- [Tokyo Night](https://github.com/folke/tokyonight.nvim) — Clean dark theme for Neovim (and 100+ ports), inspired by Tokyo at night. *(Apache-2.0 · ⭐ 8,208)*
- [Catppuccin](https://catppuccin.com) — Soothing pastel theme for 100+ apps, in four flavors (Latte, Frappe, Macchiato, Mocha). *(MIT · ⭐ 19,802)*
- [Dracula](https://draculatheme.com) — One dark theme for 400+ applications, from terminals to editors. *(MIT · ⭐ 23,591)*
- [Gruvbox](https://github.com/morhetz/gruvbox) — Retro-groove warm color scheme for Vim (and many ports); no license file ships in the repo. *(terms vary — see notes · ⭐ 15,772)*
- [Nord](https://www.nordtheme.com) — Arctic, north-bluish color palette for terminals and editors. *(MIT · ⭐ 6,888)*
- [Solarized](https://ethanschoonover.com/solarized) — Precision 16-color palette (light/dark) designed for reduced eye strain. *(MIT · ⭐ 16,021)*
- [Everforest](https://github.com/sainnhe/everforest) — Comfortable, warm green-based color scheme for Vim and ports. *(MIT · ⭐ 4,239)*
- [Kanagawa](https://github.com/rebelot/kanagawa.nvim) — Dark Neovim colorscheme inspired by the palette of The Great Wave off Kanagawa. *(MIT · ⭐ 6,410)*

## Remote & Web Terminals

Share a terminal over the network, survive flaky connections, or run a terminal in the browser. (5 entries)

- [ttyd](https://tsl0922.github.io/ttyd/) — Share your terminal over the web — C-based single binary with an xterm.js frontend. *(MIT · ⭐ 12,450)*
- [wetty](https://github.com/butlerx/wetty) — Terminal in the browser over HTTP/HTTPS via WebSocket; delegates auth to the system ssh binary. *(MIT · ⭐ 5,451)*
- [gotty](https://github.com/sorenisanerd/gotty) — Community-maintained fork of yudai/gotty (stalled since 2017): share your terminal as a web app. *(MIT · ⭐ 2,548)*
- [tty-share](https://tty-share.com) — Share your Linux/macOS terminal over the internet via a relay. *(MIT · ⭐ 1,001)*
- [mosh](https://mosh.org) — Mobile shell: remote terminal that roams across networks and survives disconnects. *(GPL-3.0-or-later · ⭐ 14,527)*

## Notable exclusions

Things people expect here that are deliberately left out — with the evidence for why.

| Project | Why it's not listed |
|---|---|
| antigen | Real zsh plugin manager (8.4k stars, MIT) but development has slowed and it is superseded by zinit/zplug-class managers; dropped to keep the list tight. |
| blink shell | Mobile-only (iOS) terminal; out of desktop scope. |
| dtach | Precursor to abduco by the same author; superseded by abduco. |
| dvtm | Real dynamic virtual terminal manager by the abduco author (MIT); pairs with abduco but the abduco entry covers that combo; dropped for count. |
| eternal-terminal | Remote shell focused on reconnection, not a terminal multiplexer. |
| final term | Abandoned; never reached a stable release. |
| ion-shell | Real Redox OS shell (MIT); dropped to keep the shell section tight. |
| kristopolansky/pixcat | Repo 404s (deleted/renamed); the canonical pixcat is mirukana/pixcat, which is included instead. |
| libsixel/libsixel | Archived fork; the canonical maintained repo is saitoha/libsixel (MIT, pushed 2026-09-16), which is included instead. |
| mosh | Mobile-shell remote protocol, not a terminal emulator. Also: Mobile/remote shell with roaming and intermittent connectivity; not a terminal multiplexer. |
| onedark | No canonical repo: fragmented across onedark.vim / onedark.nvim forks with no single official home; dropped rather than endorse an unofficial fork. |
| powerline | Statusline framework for vim/tmux/shells; a statusline, not a prompt engine per se. |
| royalterminal | .NET terminal component library (royalapplications), not a standalone emulator app. |
| shellinabox | Dormant: last code commit 2019-01-28 (v2.21 roll); the 2025-09-06 push on shellinabox/shellinabox was only a README/authority note, no code activity in 6+ years. |
| smux | Simple tmux-like multiplexer; obscure, could not confirm an active community. |
| stow / yadm / dotbot | Considered as dotfile managers but cut to keep the dotfile slice tight; chezmoi kept as the terminal-config-relevant representative. |
| terminal.app | macOS built-in; proprietary Apple software with no public source. |
| termite | Archived/unmaintained upstream. |
| tmux | Terminal multiplexer, not a terminal emulator. |
| tmuxinator | Real and popular (tmux session manager), but it manages tmux sessions rather than multiplexing itself; out of scope. |
| twin | Text-mode window manager/multiplexer; obscure, tiny community. |
| ueberzug | Upstream dead: jstkdng/ueberzug no longer exists as the original project — the name now resolves to an empty fork stub (0 stars, 0 forks, created 2023-01-16, not archived). Community development moved to the ueberzugpp fork. |
| wemux | Multi-user wrapper around tmux; niche, small community; dropped for count. |
| wstty (aroz-online/wstty) | Deprecated by its own author: README states the project is deprecated and replaced by Zoraxy's Web SSH feature; last updated ~3 years ago. |
| xterm.js | Terminal emulator component library for the browser, not a standalone emulator app. |
| yudai/gotty | Upstream unmaintained since 2017 (last release v2.0.0-alpha.3, 2017-12-13); the maintained community fork sorenisanerd/gotty (pushed 2026-08-05) is included instead. |
| zellij | Terminal multiplexer/workspace, not a terminal emulator. |
| zplug | Real next-gen zsh plugin manager (6.1k stars, MIT); dropped to keep the list tight alongside zinit. |
| kitty (terminal-ux duplicate) | The terminal-ux track produced a second 'kitty' entry identical to the GPU-Accelerated one (same repo, site, stars); dropped at merge. The kitty graphics protocol is covered in the glossary. |

## Related

- [awesome-cli](https://github.com/dakotac1994/awesome-cli) — the broad awesome-list of command-line tools; terminal-adjacent CLI utilities (file managers, fuzzy finders, git UIs, monitors) live there.
- [awesome-oss-cli](https://github.com/dakotac1994/awesome-oss-cli) — the open-source-only sibling of awesome-cli.
- [awesome-oss-macos](https://github.com/Awesome-llms-labs/awesome-oss-macos) — open-source macOS applications, including native terminal-adjacent tools.

## License

This list is [MIT](LICENSE). The projects it catalogs keep their own licenses, shown per entry.
