## 0.1.1 (unreleased)

FEATURES:

  - Can specify `-ldflags` for the go build in order to get things like
    variables injected into the compile.

IMPROVEMENTS:

  - Building toolchain no longer requires the GOROOT env var. It is
    now automatically detected using `go env`
  - On Windows builds, ".exe" is appended to the output path.

BUG FIXES:

  - When building toolchains with verbose mode, wait until output is fully
    read before moving on to next compilation.
  - Work with `-os` or `-arch` is an empty string.

## 0.1.0 (November 17, 2013)

Initial release
