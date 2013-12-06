#need to install RCurl to read the csv from github
library(RCurl)
y = read.csv("https://raw.github.com/tristantao/data-curators/master/250.csv")
z = data.frame(y)

#Magnitude versus Year:
# Magnitude is column 8
# Year is column 12

#turn the relevant columns into vectors:
mag = z[[8]]
year_raw = as.vector(z[[12]])
d <- as.Date(year_raw, format="%Y/%m/%d") 
year = as.numeric(format(d, format = "%Y"))
month = as.numeric(format(d, format = "%m")) 

#make scatterplot:

plot(d,mag, xlab = "Month in 1999", ylab = "Magnitude", main = "Earthquake Magnitude versus Time", cex=0.7)

#counting number of earthquakes in each month
count = list()
for (i in 1:12){
  count[i] = length(which(month == i))
} 
count2= as.numeric(count)

#Makes QQ Plot
qqplot(month, count2, xlab = "Month in 1999", ylab = "Number of Earthquakes", main = "Number of Earthquakes versus Time", xaxt='n')
axis(1, seq(2,12,2), c("February", "April", "June", "August", "October", "December"))
