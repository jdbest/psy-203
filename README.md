# PSY 203

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This github repository contains R lab code for labs in Bard College's for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, you'll do the same thing there.

Assuming you're downloading to your own computer, you should open RStudio (follow the syllabus details on installing R and RStudio) and use the Files pane (bottom right) to navigate to whatever folder you'll be using for the labs in this class. (e.g., "yourname/Bard/PSY 203/Labs/"). Click the gear that says "More", and click "Set as Working Directory". 

[See the image for an example](set-working-directory.png)

Once you've set your working directory (and you can also use the command `setwd()` with the directory inside the parentheses), run the following commands in the Console in RStudio to download the correct folders and data. (Copy and paste the code into the R Studio console..)

```
install.packages("usethis")
install.packages("remotes")
remotes::install_github("rstudio/learnr")
remotes::install_github("rstudio-education/gradethis")
devtools::install_github("kbodwin/flair")
install.packages("rmarkdown")
install.packages("tidyverse")
```

Once that is finished, run the following:

```
# usethis::use_course("https://github.com/jdbest/psy-203/archive/intro-to-r.zip") # need to update with correct URL
```

The file will download to your computer in the directory (folder) you defined above. Once it has finished downloading, copy and paste the following line to run in your RStudio console. 

```
rmarkdown::run("Intro-to-R.Rmd")
```
