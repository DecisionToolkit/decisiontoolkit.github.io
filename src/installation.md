# Installation

^dt ships as a single executable without any additional dependencies.

Binary version of ^dt may be obtained in the following ways:

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
> To proceed with the examples presented
> in this book, just rename the downloaded binary to:
> - **dsntk** for Linux and macOS,
> - **dsntk.exe** for Windows.

## Install using Cargo

Install [Cargo] and run:

```shell
cargo install dsntk
```

[Cargo]: https://doc.rust-lang.org/cargo/getting-started/installation.html
[GitHub releases]: https://github.com/DecisionToolkit/dsntk/releases
