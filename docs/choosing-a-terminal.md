# Choosing a terminal

How to pick from the [Awesome Terminal](../README.md) catalog without falling down a week-long rabbit hole.

## The 30-second answer

- **Just want a great daily driver?** Pick a GPU-accelerated emulator for your OS: [Ghostty](https://ghostty.org) or [iTerm2](https://iterm2.com/) on macOS, [Ghostty](https://ghostty.org), [WezTerm](https://wezterm.org), or [Alacritty](https://alacritty.org) on Linux, [Windows Terminal](https://github.com/microsoft/terminal) or [WezTerm](https://wezterm.org) on Windows.
- **Want sessions that survive disconnects?** Add a multiplexer ([tmux](https://github.com/tmux/tmux), [zellij](https://zellij.dev)) — it works inside *any* emulator.
- **Want a nicer prompt?** [starship](https://starship.rs) works in almost every shell; [powerlevel10k](https://github.com/romkatv/powerlevel10k) is the zsh speed king.

## GPU-accelerated spotlight

These render on the GPU instead of the CPU: lower input latency, smooth scrolling at high refresh rates, and native inline-image protocols (kitty graphics, sixel).

| Emulator | Platforms | License | Notes |
|---|---|---|---|
| [Ghostty](https://ghostty.org) | macOS, Linux | MIT | Native UI per platform, fast, deeply configurable |
| [WezTerm](https://wezterm.org) | macOS, Linux, Windows | MIT | Multiplexer built in, Lua configuration |
| [Alacritty](https://alacritty.org) | macOS, Linux, Windows, BSDs | Apache-2.0 | Minimal by design — no tabs, pair with tmux |
| [kitty](https://sw.kovidgoyal.net/kitty/) | macOS, Linux | GPL-3.0-only | Tabs, tiling, image display; defines the kitty graphics protocol |
| [Rio](https://rioterm.com) | macOS, Linux, Windows | MIT | Rust, WebGPU renderer |
| [Contour](https://contour-terminal.org) | macOS, Linux, Windows | GPL-3.0-only | Modern C++ VT implementation |
| [foot](https://codeberg.org/dnkl/foot) | Linux (Wayland) | MIT | Wayland-native, extremely fast and light |

## By platform

**macOS.** [iTerm2](https://iterm2.com/) is the long-standing power choice (GPL-2.0-only, decades of polish). [Ghostty](https://ghostty.org) is the modern native alternative. [Warp](https://www.warp.dev/) is proprietary (freemium) — listed for completeness, labeled as such.

**Linux.** If your desktop ships one ([GNOME Terminal](https://gitlab.gnome.org/GNOME/gnome-terminal)/[Console](https://apps.gnome.org/Console/), [Konsole](https://apps.kde.org/konsole/), [Xfce4 Terminal](https://docs.xfce.org/apps/terminal/start)), it's a fine default. For dropdown/Quake-style workflows: [Yakuake](https://apps.kde.org/yakuake/), [Guake](https://guake.github.io), [Tilda](https://github.com/lanoxx/tilda). For minimalism: [st](https://st.suckless.org/) or [foot](https://codeberg.org/dnkl/foot).

**Windows.** [Windows Terminal](https://github.com/microsoft/terminal) (MIT) is the default answer. [WezTerm](https://wezterm.org) if you want cross-platform consistency. [ConEmu](https://conemu.github.io)/[Cmder](https://cmder.app) for the classic console-wrapper workflow; [mintty](https://mintty.github.io) with Cygwin/MSYS2.

## Emulator vs multiplexer vs tabs

These solve different problems and compose: the **emulator** draws the window; the **multiplexer** (tmux, zellij, screen) owns sessions, panes, and detach/reattach; **tabs** are a UI convenience either can provide. If you SSH into persistent servers, learn tmux or zellij regardless of emulator — a dropped connection stops costing you work.

## Shells

- Stay default: **bash** (Linux default) is fine.
- Interactive upgrade: **fish** (sane defaults, autosuggestions) or **zsh** + a framework.
- Structured data pipelines: **nushell**.
- Windows: **PowerShell** (also cross-platform now).
- Tinkerers: **elvish**, **xonsh** (Python-powered), **Oils** (bash upgrade path), **murex**.

## Prompts & frameworks

Cross-shell: [starship](https://starship.rs) or [oh-my-posh](https://ohmyposh.dev). zsh-only speed: [powerlevel10k](https://github.com/romkatv/powerlevel10k). Frameworks: [oh-my-zsh](https://ohmyz.sh) (biggest ecosystem), [prezto](https://github.com/sorin-ionescu/prezto) (lighter), [zinit](https://github.com/zdharma-continuum/zinit) (plugin manager), [fisher](https://git.io/fisher)/[oh-my-fish](https://github.com/oh-my-fish/oh-my-fish) for fish, [bash-it](https://github.com/Bash-it/bash-it) for bash.

## Fonts & color schemes

Install a [Nerd Font](https://www.nerdfonts.com) (patched with prompt glyphs) if your prompt theme needs symbols — or a clean mono like [JetBrains Mono](https://www.jetbrains.com/lp/mono/), [Fira Code](https://github.com/tonsky/FiraCode) (ligatures), or [Cascadia Code](https://github.com/microsoft/cascadia-code). Then pick one scheme everywhere ([Tokyo Night](https://github.com/folke/tokyonight.nvim), [Catppuccin](https://catppuccin.com), [Dracula](https://draculatheme.com), [Gruvbox](https://github.com/morhetz/gruvbox), [Nord](https://www.nordtheme.com)) — most ship ports for editors too, so your terminal matches your editor.

## Remote terminals

Need a terminal in a browser tab or a shareable session link? [ttyd](https://tsl0922.github.io/ttyd/) and [wetty](https://github.com/butlerx/wetty) serve terminals over HTTP/WebSocket. On flaky networks, [mosh](https://mosh.org) (mobile shell) roams across IP changes instead of dropping.

## Licensing notes

Emulator licenses only constrain redistribution and modification, not *using* the terminal — GPL emulators (kitty, Contour) are fine for daily use, including at work. Proprietary emulators in this list (Warp, MobaXterm, SecureCRT, Royal TSX) are explicitly labeled; check their tiers before committing. Font/scheme licenses in this list are recorded as found — a few schemes ship no license file at all (noted per entry).
