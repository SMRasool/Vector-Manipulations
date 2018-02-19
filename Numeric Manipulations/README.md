# Vector-ManipulationsR Markdown
----------

This is an R Markdown document. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

    summary(cars)

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

Including Plots
---------------

You can also embed plots, for example:

![](Vector_Manp_files/figure-markdown_strict/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot. \# Ceating
Object

     marks<-c(86,94,78,56,98,NA)
    marks

    ## [1] 86 94 78 56 98 NA

Accessing Specified vector
==========================

    marks[c(2,3)]

    ## [1] 94 78

    marks

    ## [1] 86 94 78 56 98 NA

Removing vectors
================

\`\`{r} marks\[-c(2,5)\] \`\`\` \#Addition of vectors

    marks<-marks[3]+10
    marks

    ## [1] 88

Finding Length of vectors
=========================

    length(marks)

    ## [1] 1

    #Generating Numbers
    20:30

    ##  [1] 20 21 22 23 24 25 26 27 28 29 30

    seq(20,40)

    ##  [1] 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40

Division Of vector
==================

    marks_3<-marks/24
    marks_3

    ## [1] 3.666667

Creating two vectors
====================

    prev_cost=c(35,56,30,28)
    prev_cost

    ## [1] 35 56 30 28

    present_cost=c(24,45,56,27)
    present_cost

    ## [1] 24 45 56 27

Multiplying Two vectors having Same length
==========================================

    result=prev_cost*present_cost
    result

    ## [1]  840 2520 1680  756

Multiplying two vectors having Different Lengths
================================================

    cost1=c(3,4)
    cost1

    ## [1] 3 4

    cost2=c(3,4,5,6)
    cost2

    ## [1] 3 4 5 6

    total_cost=cost1*cost2
    total_cost

    ## [1]  9 16 15 24

Addition & Substraction of Vect
===============================

    new_cost=cost1-cost2
    new_cost

    ## [1]  0  0 -2 -2

    old_cost=cost1+cost2
    old_cost

    ## [1]  6  8  8 10
