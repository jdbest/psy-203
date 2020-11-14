# PSY 203 Lab 12

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for Lab 12. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer or RStudio.Cloud installation, and run them there. 

## Objectives

This lab will walk you through how to plot and run chi-squared ($\chi^2$) tests in R, as well as how to plot and run basic factorial ANOVAs. You'll use the `lm()` and `anova()` functions for the latter, much as you did with one-way ANOVAs in [lab 9](./09-lab-instructions.md). You'll use the `table()` function to create contingency tables and then the `chisq.test()` function to run chi-squared tests for independence and goodness of fit. You'll also practice using the **{ggplot2}** package to create a variety of plots.

## Make sure you're in the right working directory

Set your working directory if necessary. Check that you're in the directory you expect by running `getwd()` in the Console. If you need more help, [look at the wiki page on setting a working directory](../../wiki/setting-a-working-directory). 

## Today's lab 

To download and then run the tutorial, run the following two commands. **Please note: only run the `usethis::usezip()` line once! Running it again will result in your overwriting the files on your computer---potentially losing your work.**

Additionally, please make sure to copy the *whole lines*, all the way to the closing parenthesis.

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab12.zip", cleanup = TRUE)
rmarkdown::run("lab12/chisq-and-ANOVA.Rmd")
```

Once you've completed the tutorial, close it and double click on the `correg-exercises.Rmd` file in the folder you downloaded. (You may need to close the tutorial window.) To work on the exercises with the tutorial running, refer to [the instructions on the wiki](../../wiki/Run-a-tutorial-and-exercise-simultaneously).