immgen.db
================

This package contains data compiled from the [Immunological Genome Project](http://www.immgen.org) (ImmGen). Currently it contains expression data and the ontogeny.

Installation
------------

Because the expression dataset is larger than 100 Mb it is stored in a LFS repository. Therefore you need to install git-lfs in order to properly clone this repository. Follow the instructions [here](https://git-lfs.github.com). Once you have git-lfs then you can obtain `immgen.db` from github:

``` r
devtools::install_github("ddiez/immgen.db")
```

Usage
-----

``` r
library(immgen.db)
immgen # ExpressionSet object with 22,135 features and 678 samples.
```

    ## ExpressionSet (storageMode: lockedEnvironment)
    ## assayData: 22135 features, 678 samples 
    ##   element names: exprs 
    ## protocolData
    ##   sampleNames: GSM399362 GSM399363 ... GSM920647 (678 total)
    ##   varLabels: ScanDate
    ##   varMetadata: labelDescription
    ## phenoData
    ##   sampleNames: GSM399362 GSM399363 ... GSM920647 (678 total)
    ##   varLabels: FileName CellType
    ##   varMetadata: labelDescription
    ## featureData
    ##   featureNames: 100009600_at 100009609_at ... 99982_at (22135
    ##     total)
    ##   fvarLabels: ENTREZID SYMBOL GENENAME
    ##   fvarMetadata: labelDescription
    ## experimentData: use 'experimentData(object)'
    ## Annotation: mogene10stmmentrezg
