# homebrew-frontier

Homebrew tap for the `frontier` CLI (Federal Frontier Platform). macOS (Apple silicon, Intel)
and Linux (amd64, arm64).

    brew tap eupraxialabs/frontier
    brew install eupraxialabs/frontier/frontier
    frontier version

If your Homebrew asks you to trust third-party taps, run `brew trust eupraxialabs/frontier` once.

Binaries come from `https://downloads.federalfrontier.ai/frontier-cli` (public, no login). Each
download is pinned by the SHA-256 in the formula, generated from the release's signed `SHA256SUMS`.

Mirror inside your own network / air-gapped install: host the release files yourself and set the
download base before installing (the SHA-256 pins still apply):

    export HOMEBREW_FRONTIER_BASE_URL=https://mirror.example.lan/frontier-cli
    brew install eupraxialabs/frontier/frontier

Expected layout under the base: `v<version>/frontier-<version>-<os>-<arch>.tar.gz`.

This repository is a public mirror. It holds only the formula, never source. Changes are made
upstream by the maintainers and mirrored here with each release; please report issues to
Federal Frontier support rather than opening pull requests.
