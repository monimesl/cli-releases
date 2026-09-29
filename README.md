# Monime CLI releases

This repository holds the releases of `monime`, the Monime command-line
interface, for macOS, Linux and Windows on amd64 and arm64. Download them
from the [releases page](https://github.com/monimesl/cli-releases/releases).

## Install

**macOS and Linux**

```sh
curl -fsSL https://cli.monime.io/install.sh | sh
```

The script downloads the latest release for your platform, checks it against
the published SHA-256 checksums and installs `monime` to `~/.local/bin`, adding
that folder to your `PATH` if needed. No sudo is required. To pick a version or
a directory:

```sh
curl -fsSL https://cli.monime.io/install.sh | MONIME_VERSION=1.2.3 MONIME_INSTALL_DIR="$HOME/bin" sh
```

**Windows** (PowerShell)

```powershell
irm https://cli.monime.io/install.ps1 | iex
```

It installs `monime.exe` to `%LOCALAPPDATA%\Programs\monime`, after checking
its checksum, and adds that folder to your user `PATH`. To pick a version or a
directory:

```powershell
$env:MONIME_VERSION = "1.2.3"; $env:MONIME_INSTALL_DIR = "C:\tools\monime"; irm https://cli.monime.io/install.ps1 | iex
```

Or download the zip for your platform from the
[latest release](https://github.com/monimesl/cli-releases/releases/latest),
extract it and put `monime.exe` on your `PATH`. Each release lists SHA-256
checksums in `monime_<version>_checksums.txt`.

**Update**

```sh
monime update
```
