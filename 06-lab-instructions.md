# PSY 203 Lab 6

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for Lab 6. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer or RStudio.Cloud installation, and run them there. 

## Objectives

Today's lab explores some ideas about missing data, helps you identify common errors, and then introduces error bars in {ggplot2}. 

## Make sure you're in the right working directory

Set your working directory if necessary. Check that you're in the directory you expect by running `getwd()` in the Console. If you need more help, [look at the wiki page on setting a working directory](../../wiki/setting-a-working-directory). 

## Today's lab

To download and then run the tutorial, run the following two commands. **Please note: only run the `usethis::usezip()` line once! Running it again will result in your overwriting the files on your computer---potentially losing your work.**

Additionally, please make sure to copy the *whole lines*, all the way to the closing parenthesis.

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab06.zip", cleanup = TRUE)
rmarkdown::run("lab06/visualizing-data-ii.Rmd")
```

Once you've completed the tutorial, close it and double click on the `visualizing-data-ii-exercises.Rmd` file in the folder you downloaded. (You may need to close the tutorial window.) To work on the exercises with the tutorial running, refer to [the instructions on the wiki](../../wiki/Run-a-tutorial-and-exercise-simultaneously).