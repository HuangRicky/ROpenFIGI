# ROpenFIGI
A convenient interface to OpenFIGI API

# Usage
very simple, see below:

```R
jsondf <- data.frame(idType=c("ID_ISIN"),idValue=c("US922646AS37"),
                     exchCode=c(NA),currency=NA,micCode=NA,stringsAsFactors = F)

jsonrst <- OpenFIGI(jsondf)
jsonrst

library(dplyr)
finalrst <- OpenFIGI_MappingCreator(jsondf)
```
