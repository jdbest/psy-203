# PSY 203 Solo Project (Lab 8)

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for the solo project. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer or RStudio.Cloud installation, and run them there. 

## Objectives

This lab asks you to practice the skills you have learned about running *t*-tests and visualizing the results, as well as reporting them. It also expects you to practice using `filter()` and otherwise subsetting data. 

## Make sure you're in the right working directory

Set your working directory if necessary. Check that you're in the directory you expect by running `getwd()` in the Console. If you need more help, [look at the wiki page on setting a working directory](../../wiki/setting-a-working-directory). 

## The solo project

To download the project and the data it relies on, run the following command. **Please note: only run the `usethis::usezip()` line once! Running it again will result in your overwriting the files on your computer---potentially losing your work.**

Additionally, please make sure to copy the *whole thing*, all the way to the closing parenthesis.

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab08.zip", cleanup = TRUE)
```

For most users, a window will pop up with the solo project. Double click on it to open it, or select it from the Files pane in RStudio. 