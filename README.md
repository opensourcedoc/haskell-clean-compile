# haskell-clean-compile

Compile Haskell code without leaving behind temporary files.

## Overview

The Haskell compiler often generates intermediate files during compilation, which developers must clean up manually.  
This project provides a lightweight shell scripts — `haskell` — that compile Haskell code in a system temporary directory and automatically remove all intermediate files once the build is complete.

## Features

- **Clean builds**: Produces native executables without leaving behind `.hi` or other temporary artifacts.
- **Better code**: Turn on warning flags to catch issues early and ensure cleaner code.
- **Simple usage**: Just provide your source files — the scripts take care of the rest.

## System Requirements

- GHC `9.10+` (recommended)

## Usage

```shell
$ haskell main.ml
```

## Non-Goal

This project does not aim to replace Cabal.

Cabal remains the recommended build system for managing complex Haskell projects.  
haskell-clean-compile is intended only as a lightweight helper for quick compilation without clutter.

## License

MIT License (c) 2026 ByteBard
