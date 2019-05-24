# gdstheme

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)

A Xaringan template with a Government Digital Services theme

Live template example: https://matt-dray.github.io/gdstheme/

# Purpose

This package provides a template that mimics the internal style of slides at [Government Digital Service](https://www.gov.uk/government/organisations/government-digital-service) (GDS), part of the UK's [Cabinet Office](https://www.gov.uk/government/organisations/cabinet-office). 

You can use it to integrate easily the outputs of R code and make your slides reproducible.

The template requires the [{xaringan}](https://github.com/yihui/xaringan) package by [Yihui Xie](https://yihui.name/), which provides an implementation of [remark.js](https://github.com/gnab/remark) through R Markdown.

# Install

```{r}
# install.packages("remotes")
remotes::install_github("matt-dray/gdstheme")
```

To open the template in RStudio, go to `File` > `New File` > `RMarkdown...` > `From Template` > `Slide template for GDS`

![](img/new-rmd.png)

You can also use the `draft()` function from the {rmarkdown} package:

```{r}
rmarkdown::draft(
  file = "doc_name.Rmd",
  template = "gdstheme",
  package = "gdstheme"
)
```

# Contribute

Please feel free [leave an issue](https://github.com/matt-dray/gdstheme/issues). Please follow [the code of conduct](https://github.com/matt-dray/gdstheme/blob/master/CODE_OF_CONDUCT.md).