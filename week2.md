install.packages("readx1")
library(readxl)
data1<-read_excel("COVID_19_Tracker_for_India_")
head(COVID_19_Tracker_for_India_)
# A tibble: 6 × 1,324
#Covid-19 Cases in India…¹ ...2   ...3
#<chr>                     <chr> <dbl>
# 1 How it works              By @… 43900
#32 Total Cases In India      NA       47
#3 Andaman and Nicobar Isla… NA        0
#4 Andhra Pradesh            NA        0
#5 Arunachal Pradesh         NA        0
#6 Assam                     NA        0
tail(COVID_19_Tracker_for_India_)
# A tibble: 6 × 1,324
#Covid-19 Cases in India…¹ ...2   ...3
#<chr>                     <chr> <dbl>
# 1 Tamil Nadu                NA        1
#2 Telangana                 NA        1
#3 Tripura                   NA        0
#4 Uttar Pradesh             NA        9
#5 Uttarakhand               NA        0
#6 West Bengal               NA  

data1$Pclass <- 0
head(data1)

data1 <- data1[-2]

data1<- data1[-3]


data1
#merge:

data3 <- merge(data1, data2, all.x = TRUE, all.y = TRUE)
head(data3)
install.packages("writexl")
library(writexl)
write_xlsx(data1, "New_Data1.xlsx")
write_xlsx(data2, "New_Data2.xlsx")
csv_data <- read.csv(file = 'sample.csv') 
tomato<- read.table(file ="http://www.jaredlander.com/data/Tomato%20First.csv",header=TRUE, sep=",")
head(tomato)
ncol(tomato)
nrow(tomato)
s<-min(tomato$projects)
s

tomato <- read.csv(file ='http://www.jaredlander.com/data/Tomato%20First.csv') 


print(names(tomato))

new_csv <- subset(tomato, Avg.of.Totals < 10) 


print(new_csv) scv


