A sample RMD document
================

This is a single English sentence

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.0 ──

    ## ✓ ggplot2 3.3.3     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.0     ✓ dplyr   1.0.5
    ## ✓ tidyr   1.1.3     ✓ stringr 1.4.0
    ## ✓ readr   1.4.0     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
cars %>% 
  ggplot(aes(x=speed, y=dist)) +
  geom_point(col = "CadetBlue4")
```

![](Sample_RMD_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

Playing with the diamonds dataset

``` r
diamonds %>% 
  ggplot(aes(x = carat, y = price, col = clarity)) +
  geom_point() +
  facet_wrap(~cut)
```

![](Sample_RMD_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->
