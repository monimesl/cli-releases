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
the published SHA-256 checksums and installs `monime`. To pick a version or a
directory:

```sh
curl -fsSL https://cli.monime.io/install.sh | MONIME_VERSION=1.2.3 MONIME_INSTALL_DIR="$HOME/.local/bin" sh
```
