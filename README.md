# yongjohnlee80/tap

Homebrew formulae for:

- [autodb](https://github.com/yongjohnlee80/autodb), a security-first SQL editor and PostgreSQL-wire
  gate for production databases;
- [autodoc](https://github.com/yongjohnlee80/autodoc), which indexes, searches and edits a tree of
  Markdown notes, from a TUI or an RPC API.

```sh
brew install yongjohnlee80/tap/autodb
brew install yongjohnlee80/tap/autodoc
```

Works on macOS and Linux, on Apple silicon, Intel and ARM64. Each formula
installs the release binaries and pins each one to the SHA-256 the release
published.

## How they stay current

[`scripts/update-formula.sh`](scripts/update-formula.sh) renders
`Formula/<name>.rb` from a release's published checksums
(`update-formula.sh autodoc v0.1.0`). A
[workflow](.github/workflows/update-formula.yml) runs it for every formula every
six hours, commits each formula when a new release appears, and installs and
tests each on macOS and Linux. To pick up a release sooner, run the workflow by
hand from the Actions tab, for one formula or all of them.

## License

[Apache-2.0](LICENSE), like autodb and autodoc.
