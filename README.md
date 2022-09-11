# IS6812_Assignment1
print "Hello World"

import library(tidyverse)

cloud_wd <-getwd()
setwd(cloud_wd)
balance <- read.csv(file = "CD_additional_balanced.csv", stringsAsFactors = TRUE)
str(balance)
