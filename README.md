# immgen.db

This package contains data compiled from the [Immunological Genome Project](http://www.immgen.org) (ImmGen). Currently it contains expression data and the ontogeny.

## Intallation

Because the expression dataset is larger than 100 Mb it is stored in a LFS repository. Therefore you need to install git-lfs in order to properly clone this repository. Follow the instructions [here](https://git-lfs.github.com). Once you have git-lfs then you can obtain `immgen.db` from github:

```R
devtools::install_github("ddiez/immgen.db")
```

## Usage

```R
library(immgen.db)
immgen # ExpressionSet object with 22,135 features and 678 samples.
```