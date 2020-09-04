# PSY 203 Labs

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, the same instructions should work today. 

## Previous labs

* [Find Lab 1 here](./01-lab-instructions.md)

Below are instructions for Lab 2.

## Make sure you're in the right working directory

In the first lab, we set the working directory to a specific folder where every lab for this class will live. If you don't remember, [look at the wiki page I've created on setting a working directory](../../wiki/setting-a-working-directory). 

Check that you're in the directory you expect by running `getwd()` (the parentheses should have nothing in them). Just copy and paste that into the console and hit return/enter.

## Today's lab

Today's lab mostly focuses on completing the first tutorial---followed by an exercise. 

If you haven't already downloaded the relevant packages and the tutorial, do so in [Lab 1](./01-lab-instructions.md). 

If you haven't already completed the tutorial, you can open it up by pasting the following line to run in your RStudio console, which will open the tutorial. 

```
rmarkdown::run("lab01/intro-to-r.Rmd")
```

Once you've completed the tutorial, return here for an exercise that you will turn in at the end of the lab. Make sure that you *close the tutorial window*. 

## Exercise

This exercise gives you the opportunity to do the following: 

1. Practice selecting subsets of data.
2. Understand how to load a package.
3. Practice writing your own code in an R Markdown document. 

You can download the lab exercise like this:

### Run this code in the RStudio console to download the exercise directly into your working directory

(No link yet.)

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab02.zip", cleanup = TRUE)
```

After running this, a folder should open with the exercise. You can double click on the file called `intro-to-r-exercises.Rmd` to open it in RStudio. (If you'd prefer, you should be able to find it in the Files pane: open the folder "lab02" and click on the name of the exercise.)