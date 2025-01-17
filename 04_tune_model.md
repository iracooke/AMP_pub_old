Model tuning
================

    ## Warning: package 'lattice' was built under R version 3.6.2

The default models included with `ampir` are both SVMs with radial
kernel and have two tuning parameters, sigma and C (cost). Optimal
values for these tuning parameters were obtained by using model tuning
functions available in `caret`. Since this is computationally intensive
it was performed on an HPC system. The R script `scripts/tune_model.R`
provides a convenient wrapper for the required functions and allows it
to be run easily on an HPC system. See the `scripts` directory for
details of how this was run.

Inspecting the results for the mature peptide model reveals the
variation of model performance with the tuning parameters.

![](04_tune_model_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

Best tune:

    ##    sigma C
    ## 57  0.06 1

And for the precursor model:

![](04_tune_model_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

Best tune:

    ##     sigma C
    ## 104   0.1 4
