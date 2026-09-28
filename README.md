# yongjohnlee80/tap

Homebrew formulae for [autodb](https://github.com/yongjohnlee80/autodb), a
security-first SQL editor and PostgreSQL-wire gate for production databases.

```sh
brew install yongjohnlee80/tap/autodb
```

Works on macOS and Linux, on Apple silicon, Intel and ARM64. The formula
installs the release binaries and pins each one to the SHA-256 the release
published.

## How it stays current

[`scripts/update-formula.sh`](scripts/update-formula.sh) renders
`Formula/autodb.rb` from a release's published checksums. A
[workflow](.github/workflows/update-formula.yml) runs it every six hours, commits
the formula when a new release appears, and installs and tests it on macOS and
Linux. To pick up a release sooner, run the workflow by hand from the Actions
tab.

## License

[Apache-2.0](LICENSE), like autodb.
