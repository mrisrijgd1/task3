# Introduction
This is a task from Google Code-In.
Here is how to make a scatter plot with three variables and the split them with another variable.
# Requirements

- R

- RStudio

- Lattice

# Code Description
```
#Task 3

#Data Visualization in R with Lattice Graphics
library("lattice")
#Create a simple data set with 4 different variable (W,X,Y,Z) 
#where W,X,Y are numeric and Z is character with different group character (a, b ,c)
data_lattice=data.frame(W=c(1,2,3,4), X=c(4,3,2,1), Y=c(1,3,0,5), Z=c("a","b","c","c"))
#Show your data frame
View(data_lattice)
#Plot a scatter plot -make a plot from data shown above in two different panels, 
#split by variable z -Make two data series on the same plot.
cloud(W ~ X*Y, groups=data_lattice$Z, data_lattice)
```
# Screen Cast
![Record](http://g.recordit.co/UDHOc17Jbo.gif)

# Authors
- Mridul
