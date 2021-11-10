# Learning-R-Studio
Coding through data analysis to unerstand errors.

#Seting the working directory


setwd("")

#List files
list.files(recursive = TRUE)

#Install packages
install.packages("genepop")
install.packages("adegenet")
install.packages("pegas")
install.packages("hierfstat")

#read packages
library(genepop)
library(adegenet)
library(pegas)
library(hierfstat)

#Configuring the data
test_LD(
  inputFile = ("two_populations.txt"),
  outputFile = ("two_LD.txt"),
  dememorization = 10000,
  batches = 100,
  iterations = 5000,
  verbose = interactive()
)

#I have encountered an error
Error in .check_gp_file_name(inputFile) : 'inputFile' not found 
