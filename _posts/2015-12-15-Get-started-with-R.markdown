---
layout: post
title:  "Get started with R"
date:   2015-12-15 14:24:44 -0800
categories: R 
---
R is a free software environment for statistical computing and graphing. It's very useful if you work with data that are too large to load into Excel or other graphical interface tools and that you want to do things faster and neater than clicking and dragging things around. 

There is a huge hype about data science these days. If you are just getting your feet wet with data science, learning how to program with R is a good start (glad you're reading this!) It's also an easy language to learn.
<!--more-->

However, googling "getting started with R" will get you numerous links to A LOT of things, and that could be overwhelming... That's the last thing you want someone to feel when you want to help them to learn something! 

Here I'm going to be very brief to the point on how you start from ground zero and the steps to take to learn R. 

## Download R (and RStudio)

First [install R through CRAN](https://cran.rstudio.com/) and then [install R Studio](https://www.rstudio.com/products/rstudio/download/). RStudio makes it easy for you to write a script, run a script, look at files, look at manuals all at the same time with the split windows. It's also nice if you're new to Git and also want an easy way to generate a markdown report (we'll discuss this later). If you're a purist and don't need RStudio, that's cool, too. 

## Go through Swirl

Probably the best and most efficient way to learn R: actually writing R codes in the console and see things happening. Go to the [Swirl](http://swirlstats.com/students.html) page and follow the steps. There are [many interactive courses](https://github.com/swirldev/swirl_courses) with the swirl R package, from beginner things like setting a variable to a value to advanced topics like statistical models. Follow the instruction on that Github README page to download those courses. Sit down and do them. And then ... that's really it. You're done learning the essentials with R and ready to analyze whatever real dataset you're working with. Congrats!

 
## Take a Coursera course (optional)

With the hype about data science and related career, there are many, many MOOC courses on statistics, machine learning, etc, and many of them use R. If you just want to know R in general and basic data analysis, you don't need to go to this step. 

If you want to be better at your subfield, such as genomic data science, data mining, [Coursera](https://www.coursera.org/) and maybe some university's MOOC sites such as [Standford Online](http://online.stanford.edu/courses) have excellent resources. Coursera specifically has several specializations, or series of courses, that focus on different aspects of data science. 

Once you enroll in a course, Coursera will keep recommending you to pay to get the signature track. It's basically a more sophisticated way to track your performance and keep you on track so you can get a more valid certificate upon the course completion. If you don't want to pay money but like the idea of having a certificate, you can apply for a financial aid (like a fee waiver). If you're a student and/or your income is below a certain threshold, you can easily get one. 


## Now let's review some essential functions

Here are some lists of functions that are very useful and you will use them a lot. By going through the Swirl tutorials, you will have already learned most of these functions. If not, Google the function name or simply type ?function-name() in the R console to get more information on how to use the function and other function attributes you can use. 

Most of these functions are in base R, but some very useful ones are in packages you need to install yourself. Some of the must-have packages include _plyr_, _dplyr_, _ggplot2_, ... 

### 1. Facts and tips

- Always refer to an R package as a "package", not a "library", even though you load them using the `library()` function
- Useful fast keys
    - the assignment symbol `->`  :  `alt` + `-`
    - The pipe symbol `%>%`: `command` + `shift` + `M` 
    - The include symbol `%in%` : (not sure if there's one or I forgot)
- Always set up your work directory first: 
    - `getwd()`, `setwd()`

### 2. Read in a table 
- `read.table()` 
- `read.csv()`

If R complains about not having the right number of objects, it's either that you have null values in some rows/cols or that you have a string with quotes or weird symbols in them. use `quote=""` to resolve the former case. Use `?function-name()` to learn more about how to use function attributes. 

### 3. Data inspection and fixing
- `nrow()`, `ncol()`, `head()`, `tail()`, `dim()`, `length()`
- `str()`, `summary()`, `table()`
- `as.string()`, `as.factor()`, `colnames()`
- `unique()`, `which()`, `is.na()`

These are useful functions if you want to quickly inspect the data frame and the diversity of the variables in the data. It's important to do a sanity check before you proceed to more complicated analysis. 

### 4. Basic statistics
- `sum()`, `mean()`, `min()`, `max()`, `median()`
- `sd()`, `range()`, `mode()`
- `sort()`
- `quantile()`, `IQR()`

Again, a sanity check and some quick inspections. 

### 5. Data frame manipulation
- `rbind()`, `cbind()` 
- `melt()`, `stack()`, `map()`
- `factor()`
- `subset()`, `mutate()` 
- `aggregate()` <- one of my favorites
- several join functions from the plyr package, check out [my Rmarkdown report](https://github.com/santina/STAT-545/blob/master/HW7/hw7_data_wrangling.md) on these functions to learn more. 

You would often need to change how your data is structured or combine data from different resources in order to get a desirable plot or ease some analysis process. These functions often come in handy. 

### 6. Plot things 
- `plot()` , `barplot()` , `boxplot()`

Also, go learn about _ggplot2_ and _lattice_, you can check out [my R markdown report](https://github.com/santina/STAT-540/blob/master/Seminar3/Seminar3.md) as a start. 

Choose your graph and labels wisely. Avoid pie chart because areas aren't as perceivable as lengths. Use [a good color palatte](http://www.cookbook-r.com/Graphs/Colors_(ggplot2)/) in your graph. Data visualization is a whole field of study itself. Go learn more on the internet. 

### 8. Others 
- You can [write your own functions](http://www.statmethods.net/management/userfunctions.html) or even create your packages in R. 
    - This is a [simple NHL R package](https://github.com/santina/gameplay) that I wrote. It pulls NHL data from the web and summarizes them. 
    
- You can build a Shiny app, an interactive graph that let you easily explore the dataset. 
    - This [gapminder Shiny app](https://santinalin.shinyapps.io/Gapminder_App/) is something I have created as an assignment by following [this tutorial](http://stat545-ubc.github.io/shiny00_index.html). 
    - A friend of mine who TA-ed that course has written a [few blog posts](http://deanattali.com/) on many applications of Shiny app. 

- You can use R to interact with web API to [get data from the web](http://stat545-ubc.github.io/webdata03_activity.html). 

- For some additional resources, here is the course page for the two courses on R, offered at University of British Columbia 
    - [STAT545](http://stat545-ubc.github.io)


Last but not least, thanks for reading and happy learning ~ :) 