# Skills_Challenge
2024-09-25
# Load dataset 
Flower <- read.csv("C:\\Users\\ADMIN\\Desktop\\pollinators\\pollinators.csv") 
library(ggplot2) 
library(dplyr) 

## 
## Attaching package: 'dplyr' 
## The following objects are masked from 'package:stats': 
## 
## 
filter, lag 

## The following objects are masked from 'package: base': 
## 
## 
intersect, setdiff, setequal, union 

View(Flower) 

# Visualising data 
ggplot(data = Flower, aes(x = Species, y = NumberofPollinator, fill = Species)) + geom_boxplot() + labs (title = "A boxplot of No of pollinators vs species", x = "Species", y = "No of pollinator s") + theme_minimal() 

# Scatter plot 
Scatter_plot <- ggplot(data 
= 
Flower, aes(x = NumberofPollinator, y = NumberofFlowers, colour = Species)) + geom_point() + labs (title = "A scatterplot of No of Flowers Vs No of pollinator", x = "No of pollinator", y = "No of Flowers") + theme_minimal() print(Scatter_plot) 

# Fitting a Linear model 
Model <- 1m (NumberofPollinator print (Model) 

## 
## Call: 
## 1m (formula = NumberofPollinator ~ NumberofFlowers, data = Flower)
## 

# Adding the model to a scatter plot 
Scatter_plot <- Scatter_plot + 
geom_smooth (method = "1m", se = FALSE, color = "Black") + theme_minimal() 
