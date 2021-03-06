
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Computational text analysis of archaeological writing about race

<!-- badges: start -->

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/parkgayoung/racisminarchy/master?urlpath=rstudio)
[![Docker build
status](https://github.com/parkgayoung/racisminarchy/workflows/.github/workflows/docker-build.yaml/badge.svg)](https://github.com/parkgayoung/racisminarchy/actions)
<!-- badges: end -->

This repository contains the data and code for our paper. Our pre-print
is online here:

> Park, G., L-Y Wang, B. Marwick, (2020) *How do archaeologists write
> about race? Computational text analysis of 41 years of Society of
> American Archaeology Annual Meeting Abstracts*. , Accessed 21 Jun
> 2021. Online at <https://doi.org/10.31219/osf.io/zm73f>

### How to cite

Please cite this compendium as:

> Park, G., L-Y Wang, B. Marwick, (2020), (2021). *Compendium of R code
> and data for How do archaeologists write about race? Computational
> text analysis of 41 years of Society of American Archaeology Annual
> Meeting Abstracts*. Accessed 21 Jun 2021. Online at
> <https://doi.org/10.17605/OSF.IO/2N3RF>

## Contents

The most important parts of the compendium, for most users, are:

-   [:dart: \_targets.R](_targets.R): workflow instructions and
    information indicating the order that code needs to be run to
    generate the results. Run `targets::tar_make()` at the R console to
    start the analysis workflow.
-   [:file\_folder: analysis/scripts](/analysis/scripts): R script files
    that include code to reproduce the figures and tables generated by
    the analysis.
-   [:file\_folder: analysis/data](/analysis/data): Data used in the
    analysis.
-   [:file\_folder: analysis/figures)](/analysis/figures): Plots and
    other illustrations
-   [:file\_folder: analysis/paper](/analysis/paper): R Markdown
    document that combines our narrative text and code

## How to run in your broswer or download and run locally

This research compendium has been developed using the statistical
programming language R. To work with the compendium, you will need
installed on your computer the [R
software](https://cloud.r-project.org/) itself and optionally [RStudio
Desktop](https://rstudio.com/products/rstudio/download/).

The simplest way to explore the text, code and data is to click on
[binder](https://mybinder.org/v2/gh/parkgayoung/racisminarchy/master?urlpath=rstudio)
to open an instance of RStudio in your browser, which will have the
compendium files ready to work with. Binder uses rocker-project.org
Docker images to ensure a consistent and reproducible computational
environment. These Docker images can also be used locally.

You can download the compendium as a zip from from this URL:
[master.zip](/archive/master.zip). After unzipping:  
- open the `.Rproj` file in RStudio, this will open our project in
RStudio on your computer  
- run `renv::restore()` to ensure you have the packages this analysis
depends on (also listed in the [DESCRIPTION](/DESCRIPTION) file).  
- run `targets::tar_make()` to run our reproducible workflow. This will
run the R code that produces the figures and numerical results presented
in the paper, and generate our manuscript by rendering our R Markdown
document into a Microsoft Word document.

### Licenses

**Text and figures :**
[CC-BY-4.0](http://creativecommons.org/licenses/by/4.0/)

**Code :** See the [DESCRIPTION](DESCRIPTION) file

**Data :** [CC-0](http://creativecommons.org/publicdomain/zero/1.0/)
attribution requested in reuse

### Contributions

We welcome contributions from everyone. Before you get started, please
see our [contributor guidelines](CONTRIBUTING.md). Please note that this
project is released with a [Contributor Code of Conduct](CONDUCT.md). By
participating in this project you agree to abide by its terms.
