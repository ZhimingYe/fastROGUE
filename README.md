# fastROGUE: A Parallelized Version of the Original ROGUE

fastROGUE enables accelerated computation on complex data by utilizing parallel processing. The main update allows the rogue function to specify `ncores` for parallel computation.

``` r
rogue(
  expr,
  labels,
  samples,
  platform = NULL,
  k = NULL,
  min.cell.n = 10,
  remove.outlier.n = 2,
  span = 0.9,
  r = 1,
  filter = F,
  min.cells = 10,
  min.genes = 10,
  mt.method = "fdr",
  ncores = 4, # <--- This one! 
  fix_to_numbers = T
)
```

**Installing fastROGUE**\
To install fastROGUE, run:

```         
if (!requireNamespace("devtools", quietly = TRUE)) install.packages("devtools")
devtools::install_github("ZhimingYe/fastROGUE")
```

------------------------------------------------------------------------

Origin readme:

------------------------------------------------------------------------

# ROGUE (Ratio of Global Unshifted Entropy)

## Contents

-   [Overview](#overview)
-   [Installation Guide](#installation-guide)
-   [Tutorial](#tutorial)
-   [Reproduction instructions](#Reproduction-instructions)
-   [License](./LICENSE)
-   [Citation](#citation)
-   [Contact](#Contact)

## Overview {#overview}

Often, it is not even clear whether a given cluster is uniform in unsupervised scRNA-seq data analyses. Here, we proposed the concept of cluster purity and introduced a conceptually novel statistic, named ROGUE, to examine whether a given cluster is a pure cell population.

## Installation Guide {#installation-guide}

**Installing dependency package**\
Before installing ROGUE, the “tidyverse” package should be installed first:

```         
install.packages("tidyverse")
```

**Installing ROGUE**\
To install ROGUE, run:

```         
if (!requireNamespace("devtools", quietly = TRUE)) install.packages("devtools")
devtools::install_github("PaulingLiu/ROGUE")
```

## Tutorial {#tutorial}

For more details and basic usage see following tutorials: 1. [Guided Tutorial](https://htmlpreview.github.io/?https://github.com/PaulingLiu/ROGUE/blob/master/vignettes/ROGUE_Tutorials.html) (It takes a few seconds to load the HTML file)

## Reproduction instructions {#reproduction-instructions}

The scripts for producing all the quantitative results in our manuscript can be found in [scripts](./scripts).

## Citation {#citation}

If you use ROGUE in your research, please considering citing: - [Liu et al., Nature Communications 2020](https://www.nature.com/articles/s41467-020-16904-3)

## Contact {#contact}

Please contact us:\
Baolin Liu: [pauling.liu\@pku.edu.cn](mailto:pauling.liu@pku.edu.cn){.email}\
Zemin Zhang: [zemin\@pku.edu.cn](mailto:zemin@pku.edu.cn){.email}

## Copyright

©2019 Baolin Liu, Chenwei Li. [Zhang Lab](http://cancer-pku.cn/). All rights reserved.
