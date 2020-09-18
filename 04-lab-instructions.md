# PSY 203 Lab 4

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for Lab 4. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer or RStudio.Cloud installation, and run them there. 

## Previous labs

* [Find Lab 1 here](./01-lab-instructions.md)
* [Find Lab 2 here](./02-lab-instructions.md)
* [Find Lab 3 here](./03-lab-instructions.md)

Below are instructions for Lab 4.

## Objectives

The following lab explores the ideas of hypothesis-testing as explored in the initial classes, using examples from *z*-scores to continue experimenting with visualizations and continue exploring real data. You should have completed the initial three labs, have a base-level understanding of the **goals** and **procedures** of hypothesis-testing, and be ready to practice using R. 

## Make sure you're in the right working directory

Set your working directory if necessary. Check that you're in the directory you expect by running `getwd()` in the Console. If you need more help, [look at the wiki page on setting a working directory](../../wiki/setting-a-working-directory). 

## Finishing up with visualizations

If you didn't complete the exercises on creating visualizations in R and RStudio, complete those first in [Lab 3](./03-lab-instructions.md). Don't forget that you can upload the knitted output HTML file from the exercises to Brightspace for feedback. 

Want some additional information on using `ggplot2` in R? I recommend completing [this primer from RStudio](https://rstudio.cloud/learn/primers/1.1). 

## Today's tutorial

To download and then run the tutorial, run the following two commands. **Please note: only run the `usethis::usezip()` line once! Running it again will result in your overwriting the files on your computer---potentially losing your work.**

Additionally, please make sure to copy the *whole lines*, all the way to the closing parenthesis.

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab04.zip", cleanup = TRUE)
rmarkdown::run("lab04/hypothesis-testing.Rmd")
```

Once you've completed the tutorial, close it and double click on the `hypothesis-testing-exercises.Rmd` file in the folder you downloaded. (You may need to close the tutorial window.) To work on the exercises with the tutorial running, refer to [the instructions on the wiki](../../wiki/Run-a-tutorial-and-exercise-simultaneously).

## Exercise

This exercise explores the commands you learned and lets you continue practicing the steps of hypothesis testing. 

Double click on the file called `hypothesis-testing-exercises.Rmd` to open it, and follow the instructions. 