# Installation

^dt is distributed as a single executable with no external dependencies.

Prebuilt binaries of ^dt can be obtained in the following ways:

- Download released version from [GitHub releases].
- Build and install from source using [Cargo].

## Download released version

- Head to [GitHub releases](https://github.com/dsntk/dsntk-rs/releases).
- Expand the **Assets** section in selected release version.
- Download the binary of your choice, according to the operating system you use.

^tip
> Released binary file names contain _version number_ and _operating system name_ like this:
> ```text
> ^dsntk-small-^dsntk-ver-linux-x86_64
> ```
> In order to proceed with the examples presented in this documentation, rename the downloaded binary to the following:
> - `dsntk` for Linux and macOS,
> - `dsntk.exe` for Windows.

## Install using Cargo

Install [Cargo] and run:

```shell
cargo install dsntk
```

^caution
> Installing ^dt using [Cargo] may require installation of `gcc` (or a similar C/C++ toolchain like `clang`),
> because ^dt relies on math library written in C.

[Cargo]: https://doc.rust-lang.org/cargo/getting-started/installation.html
[GitHub releases]: https://github.com/DecisionToolkit/dsntk/releases

^checked
