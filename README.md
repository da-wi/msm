msm
===

Fork of the [msm](http://cran.r-project.org/package=msm) R package for continuous-time multi-state modelling of panel data implementing a zero-inflated negative binomial model. 


## Installation (development version)
```r
install.packages("devtools") # if devtools not already installed
devtools::install_github('da-wi/msm')
```
## Basic usage

```
model_zeroinflnegbinom <- list(
                 hmmMV(hmmZINBinom(disp = 10, prob = 0.4, bernpi = 0.1),
                       hmmZINBinom(disp = 3, prob = 0.3, bernpi = 0.16),
                       hmmZINBinom(disp = 5, prob = 0.6, bernpi = 0.7),
                       hmmZINBinom(disp = 2, prob = 0.3, bernpi = 0.5)),
                 hmmMV(hmmZINBinom(disp = 7, prob = 0.3, bernpi = 0.1),
                       hmmZINBinom(disp = 3, prob = 0.3, bernpi = 0.16),
                       hmmZINBinom(disp = 5, prob = 0.6, bernpi = 0.2),
                       hmmZINBinom(disp = 4, prob = 0.3, bernpi = 0.1))
)
```

## Original package

https://github.com/chjackson/msm

