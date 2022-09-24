Simple document
================
Mike Liu
September 2022

I’m an R Markdown document!

# Section 1

Here’s a **code chunk** that samples from a *normal distribution*:

``` r
samp = rnorm(100)
length(samp)
```

    ## [1] 100

# Section 2

I can take the mean of the sample, too! The mean is 0.1815003.

# Section 3

### Data frame and plot

the code chunk below creates a data frome and generates a plot

``` r
library(tidyverse)
plot_df=tibble(
  x=rnorm(500, mean=2,sd=4),
  y=3-4.2*x+rnorm(500)
)
ggplot(plot_df, aes(x = x,y = y)) + geom_point()
```

![](template_files/figure-gfm/plot%20example-1.png)<!-- -->

This plot is great!

The data frame has 500 rows

Here is a list:

- This is my first list item
- lists need at least two items
  - This list has a sub item
- Third list item

### Table

| Col 1 | Col2 |
|-------|------|
| a     | b    |
| c     | d    |

> This is a block quote
