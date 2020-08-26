# PSY 203 Labs

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, you'll do the same thing there, with a few minor changes.

If you'd like, you can watch a video about setting this up---or just follow the instructions below. (Videos link to Brightspace.)

* <a href="https://bardcollege.brightspace.com/d2l/le/content/6809/viewContent/11977/View" target="_blank">If you have a PC, click here</a>
* <a href="https://bardcollege.brightspace.com/d2l/le/content/6809/viewContent/12005/View" target="_blank">If you have a Mac, click here</a>
* <a href="https://bardcollege.brightspace.com/d2l/le/content/6809/viewContent/11978/View" target="_blank">If you're using RStudio Cloud, click here</a>
* If you're using a lab computer, it *should* have R and R Studio installed already; click on the appropriate link and jump forward to the section covering this document. (Or just read on.)
* If you're using Linux, you probably can get by just reading the instructions below---just download R (and RStudio), and continue to the directions

## Set a working directory

If you are using your own computer, follow the [syllabus details on installing R and RStudio](https://faculty.bard.edu/~jdainerbest/psy-203/syllabus.html#installing-r-and-rstudio-on-your-own-computer), and then open RStudio. If using RStudio Cloud, make an account [on RStudio.Cloud](https://rstudio.cloud/), and then skip to the next section. If using a lab computer in Albee 100, the computer should have R and RStudio installed. (Let me know if it does not.)

You'll need to make a decision about what will be your "working directory". The working directory is the folder on your computer where you'll be storing your files, and where R assumes you're working. (For example, you might use the "Downloads" folder on most computers is located in your user folder/Downloads, e.g., mine might be in /Users/jdbest/Downloads on a Mac or in C:/Users/jdbest/Downloads on a PC.) 

Use the **Session > Set Working Directory** menu. Navigate to whatever folder you'll be using for this class. (You might want to use something like /yourusername/Bard/PSY 203/labs -- but anything is fine so long as you know where it is.) This is the sort of folder that when you go to Finder (*Mac*) or Windows Explorer (*PC*), you can find all of the files associated with this class in one place. (If you're on a shared computer, you may have limited choices. Documents folders are fine!)

Optional: You can permanently set your working directory using the Tools Menu. Go to Tools: Global Options, and then click the "Browse..." under Default working directory. Navigate to the same folder you just set.

If you're familiar with some coding, you can also set your working directory using the `setwd()` command---just be sure to enclose the path in quotation marks, e.g., `setwd("/yourusername/Bard/PSY 203/labs")`. 

([Read more about working directories in R and RStudio](https://support.rstudio.com/hc/en-us/articles/200711843-Working-Directories-and-Workspaces).)

To check that you've got the right working directory set up, run the following code in the RStudio console (just copy and paste it and then hit enter):

```
getwd()
```

Does it say what you expected it to? If not, either ask for help or read through the above again.

### RStudio Cloud

Your files will download to "/home/rstudio-user" -- if when you run `getwd()` you don't get that, run the following code: `setwd("/home/rstudio-user")`. 

If you want to download files from the Cloud to your own computer, [follow these instructions](https://support.rstudio.com/hc/en-us/articles/200713893-Uploading-and-Downloading-Files). I briefly point this out in the video linked above.

## Download packages

Once you're ready with your working directory correctly set, run the following commands in the Console in RStudio to download the correct packages, and then the correct document. (Copy and paste the code _one line at a time_ into the R Studio console, hitting enter after each line.) Note that occasionally R will ask things like "These packages have more recent versions available. It is recommended to update all of them. Which would you like to update?" And you will need to select a response (e.g., type 1 and hit enter to download all updates).

```
install.packages("usethis")
install.packages("remotes")
remotes::install_github("rstudio/learnr")
remotes::install_github("rstudio-education/gradethis")
remotes::install_github("kbodwin/flair")
install.packages("rmarkdown")
install.packages("tidyverse")
```

Once all packages are installed, run the following:

```
usethis::use_course("https://github.com/jdbest/psy-203/raw/master/lab01.zip", destdir = getwd())
```

The lab document will download to your computer in the directory (folder) you defined above---into your working directory. (If you didn't define it, it'll download into whatever working directory was the default.) RStudio will prompt you to confirm that you want to do this---say yes! Once it has finished downloading, copy and paste the following line to run in your RStudio console, which will open the tutorial. 

```
rmarkdown::run("lab01/intro-to-r.Rmd")
```

## Errors and Problems

If you run into any errors, consider looking to the [wiki page](wiki/PSY-203-Wiki) for trouble-shooting, or asking a course assistant or me. (You can also scroll up and click "Wiki".)