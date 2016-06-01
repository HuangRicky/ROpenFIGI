![Build Status](https://travis-ci.org/HuangRicky/ROpenFIGI.svg?branch=master "Build Status")

# ROpenFIGI
A convenient interface to OpenFIGI API

# Usage
very simple, see below. You can look at the source code and come up with your own usage.

```R
library(ROpenFIGI)
jsondf <- data.frame(idType=c("ID_ISIN"),idValue=c("US922646AS37"),
                     exchCode=c(NA),currency=NA,micCode=NA,stringsAsFactors = F)

jsonrst <- OpenFIGI(jsondf)
jsonrst

library(dplyr)
finalrst <- OpenFIGI_MappingCreator(jsondf)
```
