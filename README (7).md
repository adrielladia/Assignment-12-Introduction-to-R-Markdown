# Assignment #12 – My R Markdown Primer

A short R Markdown document that combines narrative text, LaTeX math, and executable R code, knit to HTML.

## Files

| File | Description |
|:-----|:------------|
| [`My_R_Markdown_Primer.Rmd`](My_R_Markdown_Primer.Rmd) | R Markdown source |
| [`My_R_Markdown_Primer.html`](My_R_Markdown_Primer.html) | Knit HTML output ([view rendered page](https://htmlpreview.github.io/?https://github.com/adrielladia/Assignment-12-R-Markdown-Primer/blob/main/My_R_Markdown_Primer.html)) |
| [`images/`](images) | Screenshots of the rendered output |

## What's in the document

- **Introduction:** what R Markdown is and how knitting works (knitr → Markdown → Pandoc → HTML)
- **Markdown basics:** a syntax table with a block quote
- **LaTeX math:** inline ($\alpha + \beta = \gamma$, sample mean) and displayed equations (regression model, standard deviation)
- **Four R code chunks** using the built-in `mtcars` dataset:
  1. Load `ggplot2` and the dataset
  2. Summary statistics and mean MPG by cylinder count
  3. Linear regression of `mpg ~ wt`
  4. `ggplot2` scatter plot with a fitted regression line
- **Inline R code** that inserts calculated values (mean MPG, coefficients, R²) directly into sentences
- **Reflection** on R Markdown vs. writing plain reports

## Source vs. output

![Source vs. rendered output](images/source_vs_output.png)

## How to reproduce

```r
install.packages(c("rmarkdown", "ggplot2"))
rmarkdown::render("My_R_Markdown_Primer.Rmd")
```

Or open the `.Rmd` in RStudio and click **Knit**.
