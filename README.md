# IS6812_Assignment1
print "Hello World"

import library(tidyverse)

cloud_wd <-getwd()
setwd(cloud_wd)
balance <- read.csv(file = "CD_additional_balanced.csv", stringsAsFactors = TRUE)
str(balance)

job <- factor(c("ADMIN",  "UNKNOWN", "UNEMPLOYED", "MANAGEMENT", "HOUSEMAID", "ENTREPRENEUR", "STUDENT", "BLUE-COLLAR", "SELF-EMPLOYED", "RETIRED", "TECHNICIAN", "SERVICES"))
marriage <- factor(c("DIVORCED", "MARRIED", "SINGLE", "UNKNOWN"))
education <- factor(c("BASIC.4Y", "BASIC.6Y", "BASIC.9Y", "HIGHSCHOOL", "ILLITERATE", "PROFESSIONALCOURSE", "UNIVERSITYDEGREE", "UNKNOWN"))
contact <- factor(c("UNKNOWN", "TELEPHONE", "CELLULAR"))
month <- factor (c("JAN", "FEB", "MAR", "APR", "MAY", "JUN", "JUL", "AUG", "SEP", "OCT", "NOV", "DEC"), levels = c("JAN", "FEB", "MAR", "APR", "MAY", "JUN", "JUL", "AUG", "SEP", "OCT", "NOV", "DEC"), ordered = TRUE)
day_of_week <- factor(c("MON", "TUE", "WED", "THU", "FRI"), levels = c("MON", "TUE", "WED", "THU", "FRI"), ordered = TRUE)
poutcome <- factor(c("NONEXISTENT", "FAILURE", "SUCCESS"))

str(balance)
summary(balance)
