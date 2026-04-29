# Installation

^dt is distributed as a single executable with no external dependencies.

You can either download a prebuilt binary or install from source using [Cargo].

## Download a prebuilt binary

- Go to [GitHub releases].
- Select a version and expand the **Assets** section
- Download the archive for your operating system.
- Extract it and run the ^dt executable.

## Install with Cargo

Make sure you have [Cargo] installed, then run:

```shell
cargo install dsntk
```

^caution
> Installing ^dt using [Cargo] may require installation of `gcc` (or a similar C/C++ toolchain like `clang`),
> as ^dt depends on math library written in C.

[Cargo]: https://doc.rust-lang.org/cargo/getting-started/installation.html
[GitHub releases]: https://github.com/DecisionToolkit/dsntk/releases

^footer
