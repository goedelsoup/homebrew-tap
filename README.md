# goedelsoup/homebrew-tap

Homebrew formulae for [goedelsoup](https://github.com/goedelsoup) tools.

```sh
brew install goedelsoup/tap/yidam
```

## What is in here

| Formula | Upstream | What it is |
|---|---|---|
| `yidam` | [goedelsoup/yidam](https://github.com/goedelsoup/yidam) | Corpus analysis and index CLI for yidam-derived repositories |

`yidam` is a **binary** formula. It downloads the prebuilt light `reports` build
for your platform from the upstream release and verifies its checksum — the
whole point of the tap is to skip a compile. `--features full` (`index-build`,
`serve --mcp`, the sqlite/rdf exports) needs protoc and an ONNX runtime and
remains a source build; see the upstream README.

## Do not edit the formulae

`Formula/yidam.rb` is **generated**. Upstream's release workflow runs
[`render-formula.sh`](https://github.com/goedelsoup/yidam/blob/main/render-formula.sh)
against the checksums of the assets it has just published, and pushes the result
here. A hand edit survives until the next release and then vanishes without a
trace.

Fix the generator upstream instead. If a formula here is wrong, the release that
wrote it is the thing that was wrong.
