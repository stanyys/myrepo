A sample RMD document
================

Loading my libraries nicely

``` r
suppressMessages(library(tidyverse))
```

This is a single English sentence

``` r
cars %>% 
  ggplot(aes(x=speed, y=dist)) +
  geom_point(col = "CadetBlue4")
```

![](Sample_RMD_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

Playing with the diamonds dataset

``` r
diamonds %>% 
  ggplot(aes(x = carat, y = price, col = clarity)) +
  geom_point() +
  facet_wrap(~cut)
```

![](Sample_RMD_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->
