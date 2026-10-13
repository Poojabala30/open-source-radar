# Haskell Quickstart

Haskell is a statically typed functional programming language.

## Prerequisites

Install the Haskell toolchain using [GHCup](https://www.haskell.org/ghcup/). It provides GHC, Cabal, and other useful tools.

Verify the installation:

```bash
ghc --version
cabal --version
```

## Create a project

Create a new project using Cabal:

```bash
cabal init
```

Follow the prompts to configure your project.

## Build and run

Build the project:

```bash
cabal build
```

Run the executable:

```bash
cabal run
```

## Run tests

Run the project's test suite:

```bash
cabal test
```

## Format code

You can use `fourmolu` or `ormolu` to format Haskell source files. Install and configure the formatter according to its official documentation.

## Useful resources

- [Haskell official website](https://www.haskell.org/)
- [GHCup installation guide](https://www.haskell.org/ghcup/)
- [Cabal user guide](https://cabal.readthedocs.io/)
