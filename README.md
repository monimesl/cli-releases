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

**Homebrew**

```sh
brew install --cask monimesl/tap/monime
```

**Windows, or manual download**

Download the archive for your platform from the
[latest release](https://github.com/monimesl/cli-releases/releases/latest),
extract it and put `monime` (`monime.exe` on Windows) on your `PATH`. Each
release lists SHA-256 checksums in `monime_<version>_checksums.txt`.

## Get started

```sh
monime login        # log in as a Monimeer in your browser
monime space use    # choose the space (organization) to work in
monime status       # see who you are logged in as, and where
monime --help
```

## About this repository

Releases are published here automatically. The CLI's source is not in this
repository, so please don't open pull requests here.
