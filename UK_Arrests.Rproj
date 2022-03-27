
## UKArrests


knitr::opts_chunk$set(echo = TRUE)

library(tidyverse)
library(cowplot)
library(gridExtra)
library(patchwork)
library(ggfortify)
library(visdat)
library(naniar)
library(GGally)
library(VIM)




data <-read_csv("https://www.ethnicity-facts-figures.service.gov.uk/crime-justice-and-the-law/policing/number-of-arrests/latest/downloads/arrests-data-march-2013-to-march-2019.csv",show_col_types = FALSE)

skimr::skim(data)
names(data)




df <-cbind("Ethnicity" = data$Ethnicity,"Gender" = data$Gender, "Age" = data$Age_Group , "Region" = data$Geography ,"Arrests" = data$`Number of arrests`,"Year" = substring(data$Time,1,4) )

df<-data.frame(df)
df


write.csv(df,"UKArrests.csv",row.names=FALSE)



