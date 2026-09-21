# homebrew-tap

The Homebrew tap for [docket](https://github.com/didenkolab/docket) — Git and Obsidian, made
into one task tracker that a person and an AI agent both find obvious.

```bash
brew install didenkolab/tap/docket
docket --version
```

macOS and Linux, Apple silicon and Intel. The formula points at the binaries the release itself
built, and carries the checksums the release itself published — `script/packaging.sh` in the
main repository generates it from `checksums.txt`, so a formula cannot name a file the release
did not build.

Homebrew also clears the quarantine flag, which is worth knowing: the binaries are ad-hoc signed
rather than notarized by Apple, so a copy downloaded with a browser is refused by Gatekeeper.
Installing it this way, or with the [install script](https://github.com/didenkolab/docket#install),
avoids that entirely.

MIT, as the tool is.
