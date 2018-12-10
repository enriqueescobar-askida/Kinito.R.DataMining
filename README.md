# Kinito.R.DataMining
Kinito R Data Mining Description

## Prerequisits

Regression-https://en.wikipedia.org/wiki/Regression_analysis

Classification-https://en.wikipedia.org/wiki/Statistical_classification

Data clustering-https://en.wikipedia.org/wiki/Cluster_analysis

Association rules-https://en.wikipedia.org/wiki/Association_rule_learning

Text mining-https://en.wikipedia.org/wiki/Text_mining

Time series analysis-https://en.wikipedia.org/wiki/Time_series

Social network analysis-https://en.wikipedia.org/wiki/Social_network_analysis

## Requirements

You will need to bring your own laptop. Please install the required software and R packages and download the datasets, slides and scripts below before coming to the course.

### Software and Packages

R-http://www.r-project.org/

RStudio (desktop edition)-http://www.rstudio.com/products/rstudio/download/

#### R packages (please run the R script to install required R packages)

http://www.rdatamining.com/books/rdm/code/Install-R-packages.R

1. Package which is only available in source form, and may need compilation of C/C++/Fortran: ‘RODBC’
   Do you want to attempt to install these from sources? y/n:" 
   Choose "y".
2. The downloaded binary packages are in ... 
   Old packages: ...
   Update all/some/none? [a/s/n]:"
   Choose "a" to update all old packages, or "n" to update none.
3. Installing RODBC on Mac or Linux
   A: Run steps below:
     1) ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
     2) brew update
     3) brew install unixODBC
     4) install.packages("RODBC") and choose "y" when asked whether to install it from sources.
4. Installing rgl on Mac or Linux
  A: Download and install XQuartz https://www.xquartz.org and then install the rgl package.
```
## what's already included in R base:
## rpart, parallel, data.table
## install R packages from CRAN
pkgs <- c("arules", "arulesSequences", "arulesViz", "caret", "cluster", 
          "data.table", "dplyr", "dtw", "e1071",
          "ff", "fpc", "foreign", "ggplot2", "glmnet", 
          "Hmisc", "igraph", "knitr", "lattice", "lda",
          "magrittr", "MASS", "party", 
          "randomForest", "RColorBrewer", "rgl", "rJava", "rmarkdown", "ROAuth", "ROCR", "RODBC", 
          "scatterplot3d", "sna", "SnowballC", "snowfall", "stringi", "stringr",
          "TH.data", "topicmodels", "tm", "twitteR", "ROAuth",
          "visNetwork", "wavelets", "wordcloud", "openxlsx")
## exclude packages already installed
pkgs.installed <- installed.packages()
pkgs.to.install <- setdiff(pkgs, pkgs.installed[, 1])
print("Packages to install:")
print(pkgs.to.install)
install.packages(pkgs.to.install)
## install R packages from Bioconductor
source("http://bioconductor.org/biocLite.R")
biocLite("graph")
biocLite("Rgraphviz")
## install R packages from GitHub
install.packages("devtools")
library(devtools)
install_github("okugami79/sentiment140")
```

### RStudio project archive

Which contains all datasets, slides and scripts below. Alternatively, you may download individual files separately at links below.
http://www.rdatamining.com/training/course/RDM-course.zip

### Data

Titanic dataset-http://www.rdatamining.com/data/titanic.raw.rdata

Twitter dataset-http://www.rdatamining.com/data/RDataMining-Tweets-20160212.rds

Graph dataset-http://www.rdatamining.com/data/graph.rdata

### Slides

R Programming [PDF]-http://www.rdatamining.com/training/course/RDM-slides-r-programming.pdf

Data Exploration and Visualisation with R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-data-exploration-visualisation.pdf

Regression and Classification with R  [PDF]-http://www.rdatamining.com/training/course/RDM-slides-regression-classification.pdf

Data Clustering with R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-clustering-with-r.pdf

Association Rule Mining with R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-association-rule-mining-with-r.pdf

Text Mining with R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-text-mining-with-r.pdf

Time Series Analysis with R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-time-series-analysis.pdf

Network Analysis and Graph Mining with R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-social-network-analysis-with-r.pdf

Hadoop, Spark and R [PDF]-http://www.rdatamining.com/training/course/RDM-slides-hadoop-spark.pdf

R Reference Card for Data Mining [PDF]-http://www.rdatamining.com/docs/RDataMining-reference-card.pdf

### Scripts

http://www.rdatamining.com/training/course/RDM-course-scripts.zip

## Outline

This is an 8-hour course on data mining with R, consisting of 8 sessions below. Each session will be one hour, composed of a 40-minute tutorial and a 20-minute exercise.

### Part I: Monday 1-5pm

R Programming 
basics of R language and programming, parallel computing, and data import and export
Data Exploration and Visualisation
summary, stats and various charts
Regression and Classification
linear regression and logistic regression, decision trees and random forest
Data Clustering
k-means clustering, k-medoids clustering, hierarchical clustering and density-based clustering

### Part II: Thursday 1-5pm

Time Series Analysis
time series decomposition, forecasting, classification and clustering
Association Rule Mining 
mining and selecting interesting association rules, redundancy removal, and rule visualisation
Text Mining
text mining, word cloud, topic modelling, and sentiment analysis,
Network Analysis and Graph Mining
graph construction, graph query, centrality measures, and graph visualisation
Big Data
Hadoop, Spark and R
