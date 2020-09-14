# PSY 203 Lab 3

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for Lab 3. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, the same instructions should work today. 

## Previous labs

* [Find Lab 1 here](./01-lab-instructions.md)
* [Find Lab 2 here](./02-lab-instructions.md)

Below are instructions for Lab 3.

## Make sure you're in the right working directory

In the first lab, we set the working directory to a specific folder where every lab for this class will live. If you don't remember, [look at the wiki page I've created on setting a working directory](../../wiki/setting-a-working-directory). 

Check that you're in the directory you expect by running `getwd()` (the parentheses should have nothing in them). 

## Today's tutorial

<<<<<<< HEAD
Today's tutorial builds on the skills you learned in Labs 1 and 2; it uses the packages you installed earlier. (Haven't installed them? [Do so here](https://github.com/jdbest/psy-203/blob/master/00-install-packages.md))
=======
Today's tutorial builds on the skills you learned in Labs 1 and 2; it uses the packages you installed earlier. (Haven't installed them? [Do so here](./00-install-packages.md))
>>>>>>> 72c54308e50d1bc5fa8be631b8a37552f94cbb8e

To download and then run the tutorial, run the following two commands:

```
usethis::use_zip("https://github.com/jdbest/psy-203/raw/master/lab03.zip", cleanup = TRUE)
rmarkdown::run("lab03/visualizing-data.Rmd")
```

Once you've completed the tutorial, return for the exercise that you will turn in at the end of the lab. You may need to close the tutorial window. You may also be able to run code in the Console while the tutorial is open by *clicking on the Console tab*. See what works for you. However, you cannot knit a document while a tutorial is running.

If you would like to refer to the tutorial while also working on this document, open the HTML version of the tutorial (after closing it in RStudio) in a web browser to refer to the code. (In RStudio.Cloud, browse to the file in the Files pane, click on it, and click "View in Web Browser".)

## Exercise

This exercise gives you the opportunity to do the following: 

1. Practice filtering and subsetting
2. Practice creating histograms
3. Use `ggplot2` to create basic plots including boxplots and scatterplots.

You've downloaded the exercises along with the tutorial. Double click on the file called `visualizing-data-exercises.Rmd` to open it, and follow the instructions. 