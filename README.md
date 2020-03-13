
# ampir <a href='https://github.com/Legana/ampir'><img src="figures/ampir_hex.png" width="90" align="right" height="100" /></a>

# AMP prediction

This repository contains code used for the
[ampir](https://github.com/Legana/ampir) R package paper

  - `01_collate_databases.Rmd`
      - combines AMPs obtained from online AMP databases for positive
        training set
  - `02_create_model.Rmd`
      - trains and tests the ampir model
  - `03_benchmark_auroc.Rmd`
      - benchmarks ampir against multiple AMP predictors and makes a
        combined ROC curve plot
  - `04_alpha_prcurve.Rmd`
      - creates the alpha curve and also combines the ROC curve plot to
        make Figure1
