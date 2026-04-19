# tyler-dist

Public release artifacts for [Tyler](https://github.com/JMcunst/agent-tyler), an operator CLI for continuity work.

This repository publishes versioned release artifacts only:

- macOS tarballs (`tyler_<version>_darwin_arm64.tar.gz`, `tyler_<version>_darwin_amd64.tar.gz`)
- `checksums.txt` alongside each release

This repository does **not** contain:

- the Tyler source code (that repo is private)
- private Obsidian vault repositories
- team-safe bundles
- secrets or access tokens
- any internal operator data

## Install

Most users should install through Homebrew:

```sh
brew install JMcunst/tyler/tyler
```

The [Homebrew tap](https://github.com/JMcunst/homebrew-tyler) resolves to the release artifacts hosted here.

## Repository model

Tyler ships from three repositories with distinct roles:

- **Private source repo** — source code and operator tooling. Remains private.
- **Public dist repo** (this repo) — release artifacts only, published per version.
- **Public tap repo** ([`homebrew-tyler`](https://github.com/JMcunst/homebrew-tyler)) — the Homebrew Formula that points at artifacts in this repo.

The source repo stays private while this repo handles public artifact distribution. No vault content, bundle data, or credentials cross the private/public boundary.
