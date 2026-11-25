# Homebrew tap for Dromon

[Dromon](https://github.com/fatihdogmus/dromon) is a small, fast SFTP file browser.

```sh
brew install --cask fatihdogmus/tap/dromon
```

`brew upgrade` picks up new releases. Apple silicon, macOS 14 or newer.

`Casks/dromon.rb` is written by Dromon's
[`homebrew.yml`](https://github.com/fatihdogmus/dromon/blob/main/.github/workflows/homebrew.yml)
each time a release is published, after it checks the DMG against the release's `SHA256SUMS`
and its build attestation. Do not edit it here.

Dromon is not notarized by Apple yet, so the cask removes macOS's quarantine flag from
`Dromon.app` after installing it; otherwise macOS refuses to open it. Once releases are
notarized, the cask stops doing that.
