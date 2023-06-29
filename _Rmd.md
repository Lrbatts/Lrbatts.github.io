2023-06-29-Blog3-R
================
Landon Batts
2023-06-29

## R Recap

Now that we’ve learned how to program in R, I think my favorite thing I
learned was learning how to actually visualize data graphically and use
them to actually analyze trends in data. More specifically, the ggplot
function was my favorite to learn because it makes it easy to customize
and create graphs that are easy to analyize data. For example, I will
produce a scatter plot with the built in iris flower data.

``` r
library(tidyverse)
g <- ggplot(iris, aes(x=Sepal.Length,y=Sepal.Width))
g + geom_point(aes(col=Species)) +
  labs(main="Sepal Lenth vs Sepal Width")
```

![](_Rmd_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

``` r
#This graph shows a scatter plot of the sepal length of flowers against the sepal width with the colors representing the species of flower.
#We can see that each species grows at a different rate and there appears to be a positive relationship between length and width
```
