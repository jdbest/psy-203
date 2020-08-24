# PSY 203 Labs

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, you'll do the same thing there, with a few minor changes.

[Watch a video about setting this up on Brightspace](https://bardcollege.brightspace.com/).

## Set a working directory

If using your own computer, follow the [syllabus details on installing R and RStudio](https://faculty.bard.edu/~jdainerbest/psy-203/syllabus.html#installing-r-and-rstudio-on-your-own-computer), and then open RStudio. If using RStudio Cloud, make an account [on RStudio.Cloud](https://rstudio.cloud/), and then skip to the next section.

You'll need to know what the "working directory" is. This is the folder on your computer where you'll be storing your files. (For example, the "Downloads" folder on most computers is located in your user folder/Downloads, e.g., mine might be in /Users/jdbest/Downloads on a Mac or in C:/Users/jdbest/Downloads on a PC.) 

Use the *PC* **Tools > Change Working Directory** menu (*Mac* **Session > Set Working Directory > Choose Directory**). Navigate to whatever folder you'll be using for this class. (You might want to use something like /yourusername/Bard/PSY 203/labs.) 

Optional: You can permanently set your working directory using the Tools Menu. Go to Tools: Global Options, and then click the "Browse..." under Default working director. Navigate to the same folder you just set.

If you're familiar with some coding, you can also set your working directory using the `setwd()` command---just be sure to enclose the path in quotation marks, e.g., `setwd("/yourusername/Bard/PSY 203/labs")`. 

([Read more about working directories in R](https://support.rstudio.com/hc/en-us/articles/200711843-Working-Directories-and-Workspaces).)

To check that you've got the right working directory setup, run the following code in the RStudio console (just copy and paste it and then hit enter):

```
getwd()
```

Does it say what you expected it to?

### RStudio Cloud

Your files will download to "/home/rstudio-user" -- if when you run `getwd()` you don't get that, run the following code: `setwd("/home/rstudio-user")`. 

If you want to download files from the Cloud to your own computer, [follow these instructions](https://support.rstudio.com/hc/en-us/articles/200713893-Uploading-and-Downloading-Files). 

## Download packages

Once you're set with your working directory, run the following commands in the Console in RStudio to download the correct folders and data. (Copy and paste the code one line at a time into the R Studio console, hitting enter after each one.) Note that occasionally R will ask things like "These packages have more recent versions available. It is recommended to update all of them. Which would you like to update?" And you will need to select the number (e.g., type 1 and hit enter to download all updates).

```
install.packages("usethis")
install.packages("remotes")
remotes::install_github("rstudio/learnr")
remotes::install_github("rstudio-education/gradethis")
remotes::install_github("kbodwin/flair")
install.packages("rmarkdown")
install.packages("tidyverse")
```

Once that is finished, run the following:

```
usethis::use_course("https://github.com/jdbest/psy-203/raw/master/lab01.zip")
```

The file will download to your computer in the directory (folder) you defined above; it will prompt you to confirm that you want to do this---say yes! Once it has finished downloading, copy and paste the following line to run in your RStudio console, which will open the tutorial. 

```
rmarkdown::run("lab01/intro-to-r.Rmd")
```

## Errors and Problems

You may get a few types of errors as you run this code. You can ask me or your course assistants with questions! Additionally, you may try to troubleshoot yourself in a few ways:

### General errors

1. If you run into errors like "Error in library(gradethis) : there is no package called 'gradethis'", make sure you've run each line of the above code individually. Run them all again if needed.

2. If you run into an error like "Error in rmarkdown::run("lab01/intro-to-r.Rmd") : The directory 'lab01' does not exist", this means that the directory you downloaded to is not your working directory. 

### In RStudio.Cloud

1. Your working directory might be different from where the files downloaded. They will likely download to "/home/rstudio-user" -- if when you run `getwd()` you don't get that, run the following code: `setwd("/home/rstudio-user")`. Then try running `rmarkdown::run("lab01/intro-to-r.Rmd")`. 

2. If you get a warning on running the last line about not being able to open a popup, enable popups! 

3. Some folks may get an error like "Couldn't normalize path in `addResourcePath`, with arguments: `prefix` = 'mathjax-local'; `directoryPath` = '/usr/lib/rstudio-server/resources/mathjax-26'". If you get that error, run the following code:

```
renv::install("rstudio/renv")
```