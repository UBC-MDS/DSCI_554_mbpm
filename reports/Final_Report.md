Python vs. R
================
April 13, 2019

### Analysis Question

Python and R are the two dominate Data Science programming languages, we
set out determine how people’s background influenced their choice. In
particular we wanted to answer the following question:

> *Does the first programming language learned influence whether someone
> prefers Python or R when it comes to data analysis?*

### Potentinal Confounders

We identified the following potential counfounding variables:

1.  What was your undergraduate degree in?
      - Someone’s educational background could have a large influence on
        their preferred programming language.
2.  What is the typical size of your analysis projects? Small(10Krows),
    Medium(10-1M rows), or large (1m+ rows)?
      - The size of a data analysis project might influence the language
        a person tends to use because of differences in speed and
        efficiency.
3.  Which language do you think has better documentation when it comes
    to its data analysis packages?
      - Having clear and concise documentation aids in the ease of
        wrangling data and decreases the learning curve of the language.
        The user might tend to prefer the language they believe has
        better
    documentation.

### Exploratory Data Analysis

##### Summary of survey results:

    ##       Q1                    Q2                    Q3          Q4    
    ##  Python:36   C/C++/C#        :11   Business        : 7   Large : 6  
    ##  R     :19   Other           :11   Computer Science: 4   Medium:20  
    ##              Python          :11   Engineering     :12   Small :29  
    ##              Java/JavaScript :10   Math/Statistics :14              
    ##              R               : 5   Other           : 4              
    ##              Visual Basic/VBA: 3   Other Science   :14              
    ##              (Other)         : 4                                    
    ##       Q5    
    ##  Python:35  
    ##  R     :20  
    ##             
    ##             
    ##             
    ##             
    ## 

![](Final_Report_files/figure-gfm/preferredLang-1.png)<!-- -->

65% of respondents preferred using Python vs R for data analysis. More
people prefer python.

![](Final_Report_files/figure-gfm/firstLang-1.png)<!-- -->

Those that learned a `dev_lang` (contains C/C++/C\#/Java/Javascript)
seem to almost always prefer python over R. Majority of the survey
respondents were split between those that learned Python and
`web_dev_lang` languages first first. As this heatmap was faceted with
which language people believe have vetter documentation, this seems to
show that more people prefer the language they believe have better
documentation (the majority in this case, is Python).

![](Final_Report_files/figure-gfm/undergrad-1.png)<!-- -->

Those with a Business, Math/Statistics/ or Computer Science background
always prefer Python, those with Sciences/Other degrees seem to prefer R
over Python.

![](Final_Report_files/figure-gfm/size-1.png)<!-- -->

It seems more people prefer python no matter the size of the data set

![](Final_Report_files/figure-gfm/docs-1.png)<!-- -->

It seems highly correlated that people prefer to choose the language
that they believe has better documentation. Over half of the respondents
had experience with small analysis projects.

### Analysis

    ## # A tibble: 6 x 5
    ##   term           estimate std.error statistic p.value
    ##   <chr>             <dbl>     <dbl>     <dbl>   <dbl>
    ## 1 (Intercept)      -2.21      0.689    -3.20  0.00136
    ## 2 Q2Other           1.26      0.925     1.36  0.173  
    ## 3 Q2Python          1.25      0.923     1.35  0.176  
    ## 4 Q2R               0.865     1.21      0.716 0.474  
    ## 5 Q2web_dev_lang    0.138     1.12      0.123 0.902  
    ## 6 Q5R               2.14      0.682     3.13  0.00173

### Discussion of Results

**TODO**

### Discussion of Survey

**TODO**
