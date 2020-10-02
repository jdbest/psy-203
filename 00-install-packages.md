# PSY 203 Labs: Installing packages and programs

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This contains instructions for installing R and RStudio, and installing the packages used for most tutorials in this course. [The list of labs is here](../../.).

The github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, you'll do the same thing there, with a few minor changes.

## Install R and RStudio

1. Install R from https://cran.r-project.org/—it is available for Mac OS, Windows, and Linux. Choose the appropriate link, download, and install.

2. Install RStudio from https://www.rstudio.com/products/rstudio/download/—choose the free “RStudio Desktop” (all the way to the left). You can run R without RStudio, but I strongly recommend using RStudio (since that is what you’ll be seeing for all examples).

### Alternatively, set up an account with RStudio.Cloud

If you do not have access to a personal computer that will allow you to install this software, you may choose to make a (free) account on https://rstudio.cloud/, which is a website that runs this software. You can save files, install packages, and download your work.

## Download packages

Run the following commands in the Console in RStudio to download the correct packages. (Copy and paste the code _one line at a time_ into the R Studio console, hitting enter after each line.) Note that occasionally R will ask things like "These packages have more recent versions available. It is recommended to update all of them. Which would you like to update?" And you will need to select a response (e.g., type 1 and hit enter to download all updates)---if you've just installed R, hit enter (or a number for no and then enter) to not update. You may also get requests about whether or not to "compile from source"; you may hit "n" without the quotation marks, and then return/enter (don't do so), or allow it to compile by hitting "y" (without quotes) and then return/enter. On a PC, this question may appear as a pop-up dialog.

```
install.packages("usethis")
install.packages("remotes")
remotes::install_github("rstudio/learnr")
remotes::install_github("rstudio-education/gradethis")
install.packages("flair")
install.packages("rmarkdown")
install.packages("tidyverse")
```

## Errors and Problems

If you run into any errors, consider looking to the [wiki page on troubleshooting](../../wiki/Installation-Errors-and-Problems) for solutions. (You can also scroll up and click "Wiki".)

## What next? 

Begin with [lab 1](01-lab-instructions.md).