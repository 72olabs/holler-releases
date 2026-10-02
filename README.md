# Holler downloads

Holler provides durable local messaging for terminal agents.

This repository is the public distribution and support home. It contains
installation documentation and prebuilt releases, not the Holler implementation
or its source history.

## Install

```sh
brew install 72olabs/tap/holler
```

To upgrade:

```sh
brew update
brew upgrade 72olabs/tap/holler
```

Homebrew installs prebuilt binaries. No Go compiler or GitHub login is required.
Release archives are available for Apple Silicon macOS, Intel macOS, and x86-64
Linux. Linux ARM64 is not currently packaged.

For manual installations, download the matching archive and `.sha256` file from
[Releases](https://github.com/72olabs/holler-releases/releases), verify the checksum
with `shasum -a 256 -c ARCHIVE.tar.gz.sha256`, and extract the complete archive.
Keep `bin/` and `share/` together; connector assets are part of the distribution.

```sh
holler version
holler setup claude
holler setup codex
```

Configure only the harnesses you use. Setup may ask you to review connector
permissions; installing a binary is not proof that live messaging is ready.

## Support and licensing

Report reproducible problems in this repository's Issues. Do not include tokens,
private conversation contents, or credentials. Product information:
[holler.72olabs.ai](https://holler.72olabs.ai).

For suspected vulnerabilities, use [private security reporting](https://github.com/72olabs/holler-releases/security/advisories/new),
not a public issue. Include affected versions and a minimal reproduction without
credentials or private conversation data.

Each release includes its applicable `LICENSE`. Moving binary hosting does not
change the license of an existing release: 0.8.0 remains Apache-2.0.

GitHub's automatically generated "Source code" ZIP/tar downloads contain only
this distribution repository, not the Holler product. Use the named
`holler-VERSION-PLATFORM.tar.gz` assets to install Holler.
