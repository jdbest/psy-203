# PSY 203 Lab 13: Final project

The primary website for this course is <https://faculty.bard.edu/~jdainerbest/psy-203>

These are all of the instructions for Lab 13. [The list of labs is here](../../.).

This github repository contains R lab code for labs in Bard College's Fall 2020 for Statistics for Psychology, taught by Prof. Justin Dainer-Best. 

For each lab, you should expect to download the lab's files locally to your computer or RStudio.Cloud installation, and run them there. 

## Objectives

The project is described in the syllabus as follows: In your group project, you will perform a data analysis on real data, using the skills you've developed in the labs. This group project is a semester-summarizing version of the solo project---you will develop research questions, create visualizations, carry out analyses, and produce a final document that reports all of them. 

The project is worth 40 points; completing all requirements and turning the project in on-time will result in the receipt of at least 32.

You may use any resources you choose in this (e.g., textbook, web searches, stats study rooms), although of course the work must be your own groups' work. Adapting others' code (e.g., from a StackOverflow post) is great!

## Objectives

As with the solo project, the goals are:

* To help you to practice the skills learned in lab
* To help you understand what happens in the data analysis and reporting sections of a research project
* To give you functional skills from the use of R and RStudio

Don't forget to (a) save and (b) knit the document frequently, so you'll keep track of your work and also know where you run into errors. 

## Deadlines <i class="fa fa-calendar-check-o" aria-hidden="true"></i>

**The final project is due December 14, 2020**

You should plan to also meet the following deadlines (more info below):

* You should read this document, in full, as soon as possible
* By **11/30**, I should know _who_ is in your group, and which dataset (below) your group is using.
* By **12/7**, you should have asked me any major questions---e.g., "is this analysis appropriate?"---and submitted a **preregistration**.
* Again, the final document is due **12/14**

## Requirements

### The data

You get to choose your dataset! You must choose one of the following datasets (or another one you let me know about), and read about it. (If you'd like to find your own, you might try looking at <https://www.icpsr.umich.edu/web/pages/ICPSR/index.html> or <https://dataverse.harvard.edu/> to find them.)

Here are the datasets I suggest:

* Climate Change in the American Mind: National Survey Data on Public Opinion (2008-2017): https://osf.io/w36gn/ 
* Correlates of War: https://correlatesofwar.org/data-sets
* World Values Survey: http://www.worldvaluessurvey.org/WVSContents.jsp
* Pro Publica data on criminal justice: https://www.propublica.org/datastore/datasets/criminal-justice
* Pro Publica data on health: https://www.propublica.org/datastore/datasets/health
* FBI Hate Crime Reports: https://github.com/emorisse/FBI-Hate-Crime-Statistics/tree/master/2013

Whichever data you decide to use, you should (a) read about it in detail, (b) plan to cite the data in APA style, and (c) make sure that you can read the data into R. You can ask me with questions on that topic.

You may need to do some data processing. Any processing that you do before importing it into R (e.g., opening it up in Google Sheets or Excel and renaming columns) should be reported in your final document. 

### Your group

Your group should be 3--4 members of the class, ideally all in your same lab section

### Hypotheses, Preregistration, and Introduction

You should plan to frame _testable_ hypotheses which involve some of the variables described in your dataset. Those should include both a research hypothesis ($H_1$) and a null hypothesis ($H_0$). 

Your statistical framing of the hypotheses (involving means) should assume two-tailed tests. However, your preregistration should also suggest the direction you anticipate. For example, will a correlation be positive or negative? Which group will have higher scores? Will the chi-squared test find independence? All tests (described further immediately below this section) should have a preregistered hypothesis. 

Please refer to the bottom of this document for an [abbreviated preregistration template](#preregistration-template).

In the final document, you should also include a brief introduction which describes the data and cites it, reports your directional hypotheses, and explains why you've made those hypotheses.

### Analyses

#### Statistical tests

You should use **multiple statistical tests** that provide evidence for or against your hypotheses. At minimum, you must conduct tests that fall into three of the following groups: (1) regression or correlation, (2) one-way or factorial ANOVA, (3) independent-samples or decedent-samples *t*-tests, (4) chi-squared test. 

If you're assigning the results of a test to a variable (e.g., `model <- lm(DV ~ IV1 * IV2, data = data)`), then you must also print the model (so that I can see what it looks like):

```
model <- lm(DV ~ IV1 * IV2, data = data)
model
anova(model)
```

All tests must be interpreted immediately (in the document) after the code, with the results printed in the final document. Your interpretation should always include whether the test is significant or not. It frequently will be useful to include the group means. As always, you should generally round to two significant digits after the decimal. 

#### Plots

You should create at least four plots (figures). At least two of those should involve some sort of comparison between variables---i.e., not simply be histograms or boxplots. Several plots should help you interpret the results of the tests. The plots should be "in-line," meaning that they follow the relevant section. For example, a bar graph might be useful immediately following your running a factorial ANOVA.

### Brief discussion

After all tests, you should include a "discussion section" which explains what your tests found and why it matters (or does not). Null results are absolutely fine! 

### Group contributions

At the bottom of your document, you should list all group members. Next to each member's name, detail which of the following roles they played, out of the following:

1. Chose dataset
2. Developed hypotheses
3. Wrote preregistration
4. Wrote introduction
5. Wrote code for analyses
6. Created graphs
7. Reported results of analyses
8. Wrote discussion
9. Edited code
10. Edited document

For example (although more overlap may be better!):

* Faux Auteur: Chose dataset, Developed hypotheses, Wrote preregistration, Wrote introduction, Wrote discussion, Edited document
* Ersatz Autor: Chose dataset, Developed hypotheses, Created graphs, Edited code
* Falso Autor: Wrote code for analyses, Reported results of analyses, Wrote discussion, Edited document

## The documents

For both the preregistration and the final document, you should plan to create a new R Markdown document for your final project. (Yes, you have to use R Markdown; you may not do this in a Word doc---I want to be able to see the code and the image it produces.) Your document should include the following "code" at the top (replacing what is automatically generated), with your title after "title" and your names under the - marks following "author". You should knit that document.

```
---
title: 
author: 
  - First name here
  - Second name here
  - etc.
date: 
output: 
  html_document:
    self_contained: yes
---
```

## Grading

The project is worth 40 points; completing all requirements and turning the project in on-time will result in the receipt of at least 32.

### What does "all requirements" entail? 

* Turning in the preregistration on-time with three or more hypotheses
* Turning in a logical and readable knitted R Markdown document (you won't lose many points for turning in an Rmd file with the data, but you will lose some)
* Including the following (complete) sections of the final document: introduction, analyses, and brief discussion
* Including 3+ tests (based on the hypotheses, and from different "families" of tests)
* Including 4+ plots with labeled axes
* Properly citing the data (and any relevant external sources)
* Including the group members' contributions at the bottom

Missing any of these will result in *fewer* points. However, doing something wrong (e.g., misinterpreting the results of a test) will not necessarily result in lost points.

### How do we get the rest of the points?

More writing does not mean better---a good project can be brief.

1. Complete the self-grading rubric
2. Make sure that your code "works" and is correctly interpreted
3. Work together---look over one another's work, and make sure that everything makes sense
4. Make plots that look good, have thoroughly labeled axes and titles, and clearly show the results of the test in question
5. Thoughtfully reflect on the tests and their results in the discussion

The remaining points will be awarded as follows:

| Points|Topic                                                                                  |
|------:|:--------------------------------------------------------------------------------------|
|      2|Clever question and tests                                                              |
|      2|Excellent interpretation of results                                                    |
|      2|Plots are complete and explain information                                             |
|      2|There is a clear 'message' to the project: hypotheses link to one another and to tests |

# Preregistration template

Use the following for your preregistration in a new R Markdown document. Note that the language under the headers (i.e., the bits that *don't* start with a #) should be deleted---they're just explaining the section.

```
# Variables

## Independent Variables
What are your independent / grouping / predictor variables (including mediators and moderators) ? Explain how you operationalize each variable

## Dependent Variables
What are your dependent / outcome variables? Explain how you operationalize each variable.


# Hypotheses
What are your primary study hypotheses / research questions?


# Sampling
What is the sample size? 

## Sample characteristics
Who is the sample representing?


# Analysis plan

## Significance threshold
What will be your criterion for determining statistical significance?

## Exclusion criteria
Will you exclude participants from data analysis based on any of the reasons listed below? Failed attention check; Failed manipulation check; Missing data

## Outliers
What criterion (if any) will you use to determine whether a participant is an outlier?


## Statistical tests
Which statistical tests will you use to conduct your data analyses? ANOVA; Correlation; t-test; Chi-square; Regression; Other/Additional

If relevant, describe what types of follow-up tests will you perform (e.g., post-hoc; simple main effects). If you will conduct planned comparisons, explain the nature of those comparisons
```