# trtlgrd

A linter for RDF graphs written in Turtle or N-Triples. trtlgrd checks a
project's graph files against a rule set, and each rule is a script plugin.
The output is compact and color-free, so a coding agent or a CI job can read
it cheaply.

trtlgrd is the RDF member of the `*grd` family. The family shares one CLI
shape, config format and exit-code contract:

| Tool       | Checks                                  |
| ---------- | --------------------------------------- |
| `ctxgrd`   | Documents: ADRs, PRDs, READMEs          |
| `trtlgrd`  | RDF graphs: Turtle, N-Triples           |
| `wrkgrd`   | Code: build, tests, lint configuration  |

This repository holds the release binaries only. The source is not published.

## Install

```sh
brew install aktagon/tap/trtlgrd
```

Or download the archive for your platform from the
[releases page](https://github.com/aktagon/trtlgrd/releases) and check it
against `checksums.txt`. Releases cover macOS (Apple silicon and Intel) and
Linux (x86_64, statically linked).

## Use

```sh
trtlgrd init     # write a starter turtleguard.toml
trtlgrd          # lint the project tree
trtlgrd docs     # print the bundled user guide
```

## License

MIT. See [LICENSE](LICENSE).
