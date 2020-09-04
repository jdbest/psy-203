# PSY 203 Labs

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer, and run them there. If you're using https://rstudio.cloud/ instead of running things locally, the same instructions should work today. 

[Find Lab 1 here](./01-lab-instructions.md). These are instructions for Lab 2.

## Make sure you're in the right working directory

In the first lab, we set the working directory to a specific folder where every lab for this class will live. If you don't remember, [look at the wiki page on setting a working directory](../../wiki/setting-a-working-directory). 

Check that you're in the directory you expect by running `getwd()` (the parentheses should have nothing in them). Just copy and paste that into the console and hit return/enter.

## Today's lab







```
usethis::use_course("https://github.com/jdbest/psy-203/raw/master/lab01.zip", destdir = getwd())
```

The lab document will download to your computer in the directory (folder) you defined above---into your working directory. (If you didn't define it, it'll download into whatever working directory was the default.) RStudio will prompt you to confirm that you want to do this---say yes! Once it has finished downloading, copy and paste the following line to run in your RStudio console, which will open the tutorial. 

```
rmarkdown::run("lab01/intro-to-r.Rmd")
```

## Errors and Problems

If you run into any errors, consider looking to the [wiki page on troubleshooting] for solutions, or asking a course assistant or me. (You can also scroll up and click "Wiki".)