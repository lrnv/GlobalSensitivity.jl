# GlobalSensitivity.jl

GlobalSensitivity.jl package contains implementation of some the most popular GSA methods. Currently it supports Delta Moment-Independent, DGSM, EASI, eFAST, Morris, Fractional Factorial, RBD-FAST, Sobol and Regression based sensitivity methods.

[![Join the chat at https://gitter.im/JuliaDiffEq/Lobby](https://badges.gitter.im/JuliaDiffEq/Lobby.svg)](https://gitter.im/JuliaDiffEq/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Build Status](https://github.com/SciML/GlobalSensitivity.jl/workflows/CI/badge.svg)](https://github.com/SciML/GlobalSensitivity.jl/actions?query=workflow%3ACI)
[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](http://gsa.sciml.ai/stable/)
[![Dev](https://img.shields.io/badge/docs-dev-blue.svg)](http://gsa.sciml.ai/dev/)

## Tutorials and Documentation

For information on using the package,
[see the stable documentation](https://gsa.sciml.ai/stable/). Use the
[in-development documentation](https://gsa.sciml.ai/dev/) for the version of
the documentation, which contains the unreleased features.
[![ColPrac: Contributor's Guide on Collaborative Practices for Community Packages](https://img.shields.io/badge/ColPrac-Contributor's%20Guide-blueviolet)](https://github.com/SciML/ColPrac)

## Installation

The GlobalSensitivity.jl package can be installed with julia's package manager as shown below:

```julia
]add GlobalSensitivity
using GlobalSensitivity
```

## General Interface

The general interface for performing global sensitivity analysis using this package is:

```julia
res = gsa(f, method, param_range; samples, batch=false)
```
