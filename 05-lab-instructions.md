# PSY 203 Lab 5

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for Lab 5. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer or RStudio.Cloud installation, and run them there. 

## Objectives

The following lab *builds* on your skills with `ggplot2`, using `filter()`, and helps you practice using *z*-scores and *t*-scores to test simple sample means. This lab anticipates that you have read Chapter 7 of the course textbook, listened to the initial lecture on *t*-tests, or have a background on *t*-tests; however, most of the lab reviews material you have already covered in [previous labs](../../.). 

## Make sure you're in the right working directory

Set your working directory if necessary. Check that you're in the directory you expect by running `getwd()` in the Console. If you need more help, [look at the wiki page on setting a working directory](../../wiki/setting-a-working-directory). 

## Today's lab

There is no tutorial today; you'll be focusing on an R Markdown file. 

To download it, run the following single command. **Please note: only run the `usethis::usezip()` line once! Running it again will result in your overwriting the files on your computer---potentially losing your work.**

Additionally, please make sure to copy the *whole lines*, all the way to the closing parenthesis.

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab05.zip", cleanup = TRUE)
```

This exercise explores the commands you learned and lets you continue practicing the steps of hypothesis testing. 

Double click on the file called `one-sample-t.Rmd` to open it, and follow the instructions. 