---
output:
  html_document: default
---
# PSY 203

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This github repository contains R lab code for labs in Bard College's for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, you'll do the same thing there.

Assuming you're downloading to your own computer, you should open RStudio (follow the syllabus details on installing R and RStudio) and use the Files pane (bottom right) to navigate to whatever folder you'll be using for the labs in this class. (e.g., "yourname/Bard/PSY 203/Labs/"). Click the gear that says "More", and click "Set as Working Directory". 

[See the image for an example](set-working-directory.png)

Once you've set your working directory (and you can also use the code `setwd()` with the directory inside the parentheses), run the following commands in the Console in RStudio to download the correct folders and data. 

```
install.packages("usethis")
```

Once that is finished, run the following:

```
usethis::use_course("https://github.com/jdbest/psy-203/archive/intro-to-r.zip")
```