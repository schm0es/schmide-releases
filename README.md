# schmide

An IDE built around Claude Code. This repository holds its releases.

## Install

```bash
curl -fsSL https://github.com/schm0es/schmide-releases/releases/latest/download/install.sh | bash
```

Windows (PowerShell):

```powershell
irm https://github.com/schm0es/schmide-releases/releases/latest/download/install.ps1 | iex
```

or run `schmide-windows-x86_64-setup.exe` from the latest release (unsigned:
SmartScreen asks first, More info → Run anyway).

Installs what schmide needs (WebKitGTK on Linux, git, Claude Code), then the
app: on Linux `~/.local/bin/schmide` with a menu entry, on macOS
`/Applications/schmide.app`. Linux x86_64 and arm64; macOS Intel and Apple
Silicon; Windows x64 (per user, `%LOCALAPPDATA%\schmide`, no admin; uninstall
from Settings > Apps).

- Skip Claude Code: `... | bash -s -- --no-claude`
- A specific version: `... | SCHMIDE_VERSION=v0.2.0 bash`
- Uninstall: `... | bash -s -- --uninstall`

schmide checks for updates on start and every few hours, downloads them in
the background (each is signature-checked) and offers **Restart to update** in
the title bar. The palette has **Check for Updates**.
