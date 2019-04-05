## Main question:
A Survey of:

_Does the first programming language learned influence whether someone prefers Python or R when it comes to data analysis?_

## Other questions & Justifications:
1. What is the first computing language you learned?
  - This survey question explores the influence of specific languages for the preference of Python or R.
  - Choices: C/C++/C#, HTML/XML/CSS, Java/JavaScript, Python, R, SQL, Visual Basic/VBA, and Other
2. What was your undergraduate degree in?  
  - Educational background might influence what programming language one prefers to learn first.
  - Choices: Business, Computer Science, Engineering, Math/Statistics, Other Science, and Other
3. What is the typical size of your analysis projects? Small(10K rows), Medium(10-1M Rows), or large (1m+ rows) ?
  - The size of a data analysis project might influence the language a person tends to use because of difference in speed and ease of setup/use.  
  - Choices: Small(0 - 10k rows), Medium (10k - 1m rows), and Large (1M+ rows)
4. Which language do you think has better documentation when it comes to its data analysis packages?
  - Having clear and concise documentation aids in the ease of wrangling data and decreases the learning curve of the language. If clear examples of analysis using the languages of R or Python are not given, the user might tend to prefer to choose the one they believe has better documentation that helps them through the process.  
  - Choices: Python or R

## Plan of Survey Analysis.

We plan to use logistic regression to analysis how someone's preference to use R or Python for a data analysis task is influenced by the first programming language learned they have learned, while also controlling for confounding effects. We chose a logistic regression because we have a binary response variable, either R or Python, and will the other survey question answers as explanatory variables.

## Discuss the aspects of the UBC Office of Research Ethics document on Using Online Surveys that are relevant to your proposed survey.
- We will not be collecting any names in our surveys
- Our survey will be anonymous
- Our Survey will not include any IP address that could be used to identify a person
