# schmide

An IDE built around Claude Code. This repository holds its releases.

## Install (Linux, macOS)

```bash
curl -fsSL https://github.com/schm0es/schmide-releases/releases/latest/download/install.sh | bash
```

Installs what schmide needs (WebKitGTK on Linux, git, Claude Code), then the
app: on Linux `~/.local/bin/schmide` with a menu entry, on macOS
`/Applications/schmide.app`. Linux x86_64 and arm64; macOS Intel and Apple
Silicon.

- Skip Claude Code: `... | bash -s -- --no-claude`
- A specific version: `... | SCHMIDE_VERSION=v0.2.0 bash`
- Uninstall: `... | bash -s -- --uninstall`

schmide checks for updates on start and every few hours, downloads them in
the background (each is signature-checked) and offers **Restart to update** in
the title bar. The palette has **Check for Updates**.
