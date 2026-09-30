# Glossary

Terms you'll meet across the [Awesome Terminal](../README.md) catalog.

- **PTY (pseudoterminal)** — the kernel device pair that makes a shell believe it's talking to a real terminal. Every emulator and multiplexer allocates one per session.
- **Terminal emulator** — the application that draws the window, interprets escape sequences, and hosts the PTY. (This list's core section.)
- **Escape sequences** — byte sequences the application sends to control the terminal: **CSI** (Control Sequence Introducer, `ESC [` — colors, cursor movement), **OSC** (Operating System Command, `ESC ]` — window titles, clipboard, hyperlinks), **SGR** (Select Graphic Rendition — text styling).
- **True color (24-bit)** — `ESC[38;2;R;G;Bm` sequences for ~16.7M colors; assumed by most modern schemes.
- **Sixel** — a bitmap graphics protocol from DEC terminals, revived for inline images ([libsixel](https://github.com/saitoha/libsixel) implements it).
- **Kitty graphics protocol** — kitty's chunked, GPU-friendly image transmission protocol; supported by a growing set of emulators and tools.
- **OSC 52** — the escape sequence for clipboard read/write through the terminal; the standard trick for copy/paste over SSH.
- **Scrollback** — the terminal's stored history of past output; search and persistence vary by emulator.
- **Multiplexer** — a program that owns PTYs and multiplexes them into panes/windows with detachable sessions (tmux, zellij, screen).
- **Shell** — the command interpreter running inside the terminal (bash, zsh, fish…).
- **Prompt** — the rendered command line prefix; **prompt engines** (starship, powerlevel10k) render it fast with git/context segments.
- **Plugin manager / framework** — ecosystems that install and update shell plugins and themes (oh-my-zsh, fisher, zinit).
- **Dotfiles** — version-controlled shell/terminal configuration; **dotfile managers** (chezmoi) deploy them across machines.
- **Nerd Fonts** — monospaced fonts patched with thousands of prompt/status glyphs (devicons, powerline symbols).
- **Ligatures** — combined glyphs for multi-character sequences (`->`, `=>`); a font feature, rendered by the emulator.
- **GPU rendering** — drawing terminal cells with the GPU instead of the CPU; the main latency/throughput win of modern emulators.
- **Latency vs throughput** — input latency (keystroke-to-photon time) matters more for feel than raw scroll throughput; GPU emulators optimize the former.
- **VT100 / xterm compatibility** — the de facto escape-sequence dialect; "xterm-compatible" means an emulator speaks the dialect everything expects.
- **Quake-style / dropdown terminal** — a terminal that slides down from the top of the screen on a hotkey (Yakuake, Guake, Tilda).
- **Tiling** — splitting one window into multiple panes without overlapping windows (kitty, WezTerm, Terminator, Tilix do it natively).
