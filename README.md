# gov

`gov` is a super simple version manager for the Go toolchain.  `gov` downloads,
unpacks, and makes available versions of Go from golang.org.

## Installation

* Place `gov` on your `$PATH`
* Add `$HOME/.go/active/bin` to your `$PATH`
* Run `gov download 1.11.1` (for Go 1.11.1)

`gov` stores versions of Go in `$HOME/.go` in folders named after the specifc
version of Go and manages a symlink called `active` that points to the specific
version of Go in use.

## Usage

Download and install versions of Go with `gov download`.  Activate installed
versions of Go with `gov use`.

## Why another version manager?

I wrote `gov` to scratch a personal itch of mine and fit into my personal
preferences.  `gov` installs go versions in a separate managed directory inside
my home directory, without messing with the rest of the system.  `gov` expects
you to have a single `GOPATH`, shared among all versions of Go and a single
active version of Go at a time.  `gov` avoids recompiling Go itself and just
uses the precompiled distribution from golang.org.  `gov` is written as a
simple shell script, so you don't need to download a random binary from the
Internet or have a pre-existing Go toolchain to compile it.

Feel free to use `gov`, or to ignore it.

