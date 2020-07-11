<a href="https://covid19datahub.io"><img src="https://storage.covid19datahub.io/logo.svg" align="right" height="128"/></a>

# Julia Interface to COVID-19 Data Hub
[![DOI](https://joss.theoj.org/papers/10.21105/joss.02376/status.svg)](https://doi.org/10.21105/joss.02376)

[Julia](https://julialang.org/) is a dynamic high-level programming language for scientific computing focused on high performance.

For parsing csv Julia [CSV](https://juliadata.github.io/CSV.jl/stable/) is used. Install it by typing into Julia console

```julia
using Pkg
Pkg.add("CSV")
```

Once installed, fetch the data with

```julia
using CSV
# download
url = "https://storage.covid19datahub.io/data-1.csv"
data = CSV.read(download(url))
```
