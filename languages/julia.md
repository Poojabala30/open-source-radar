# Julia Quickstart

Julia is a programming language designed for numerical computing, scientific computing, and data analysis.

## Prerequisites

Install Julia using the [official Julia installation guide](https://julialang.org/install/).

Check that Julia is installed:

```bash
julia --version
```

## Set up a project

Open a terminal in your project directory and start Julia with the project environment:

```bash
julia --project
```

To create a project environment, open Julia and enter package mode by pressing `]`. Then run:

```julia
activate .
```

Press Backspace to return to the Julia prompt.

## Install project dependencies

From the project directory, run:

```bash
julia --project -e 'using Pkg; Pkg.instantiate()'
```

This installs the dependencies declared by the project.

## Run tests

Run the project's test suite with:

```bash
julia --project -e 'using Pkg; Pkg.test()'
```

## Format code

[JuliaFormatter.jl](https://github.com/domluna/JuliaFormatter.jl) can format Julia source code. Follow its documentation to install and configure it.

## Faster development

[Revise.jl](https://github.com/timholy/Revise.jl) can help reload code changes during an interactive Julia session. See its documentation for setup and usage.

## Useful resources

- [Julia documentation](https://docs.julialang.org/)
- [Julia package manager](https://pkgdocs.julialang.org/)
- [Julia installation guide](https://julialang.org/install/)
