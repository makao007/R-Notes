# Data Mining with R
#### the Book resource : http://www.dcc.fc.up.pt/~ltorgo/DataMiningWithR/

    install.packages("DMwR")
    library("DMwR")

## clean all the variable in the current environment
    rm(list=ls())

## load the data set into env
### method 1 , load from the Library
    library("DMwR")
### method 2 , load from the RData file
    load("algae.RData")
### method 3 , load form the text file
    algae <- read.table('Analysis.txt', header=FALSE, dec='.',
	col.names=c('season','size','speed','mxPH','mnO2','Cl','NO3','NH4','oPO4','PO4','Chla','a1','a2','a3','a4','a5','a6','a7'),
                      na.strings = c("XXXXXXX"))

## show the data set overview
    str(algae)
    nrow(algae)
    ncol(algae)
    head(algae)
    summary(algae)


