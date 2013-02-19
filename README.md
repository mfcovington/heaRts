# Random Heart Generator

I made the Random Heart Generator for Valentine's Day as part of a weekly class I help teach on R and ggplot.

## Defaults

The default parameters of The Random Heart Generator are:


```r
hearts(n = 5, up = TRUE, free.love = FALSE)
```


## Usage

The Random Heart Generator plots five hearts of random size, position, and color (of the rainbow):


```r
source("random_heart_generator.R")
hearts()
```

![plot of chunk default_hearts](figure/default_hearts.png) 


By changing `n`, you can plot any number of hearts:


```r
hearts(n = 10)
```

![plot of chunk ten_hearts](figure/ten_hearts.png) 


However, if you try to plot too many (100+), you will get a warning to help prevent R from becoming non-responsive:


```r
hearts(n = 150)
```

```
## [1] "That's way too many hearts for you to handle."
```


This safeguard can be bypassed with the `free.love` option:


```r
hearts(n = 150, free.love = TRUE)
```

![plot of chunk lots_of_hearts](figure/lots_of_hearts.png) 


Since love can be messy, you can make your plot a bit more chaotic by changing to `up` option:


```r
hearts(up = FALSE)
```

![plot of chunk up+down_hearts](figure/up+down_hearts.png) 

