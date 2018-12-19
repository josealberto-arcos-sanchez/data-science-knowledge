# Working with R and Python

## Abstract
There has been a passionate discussion in the past few years about which is the best tool for data science: R or Python. Today, this discussion is meaningless. It is completely possible to use the best tools from both worlds. And I will explain how to do it here.

## Using R and Python together

### R notebooks
The easiest way to use R and Python together is through RStudio Notebooks, where it is possible to use R and Python code together, sharing data between them. A minimal notebook example can be found [here](R_notebooks/r_and_python.Rmd) (and the result of its execution can be found [here](https://htmlpreview.github.io/?https://raw.githubusercontent.com/josealberto-arcos-sanchez/data-science-knowledge/master/tools/r_and_python/R_notebooks/r_and_python.html)).

The problem with this approach is that it is only available when using R notebooks in the last version of RStudio.

### Reticulate
Another great way is to use the great [reticulate](https://github.com/rstudio/reticulate) package to use Python from R. This approach is more flexible, as you can use it is any script or tool. You don't need to use an R notebook over RStudio as before. 

A great example that shows how to use Scikit-Learn from R can be found [here](R_Scikit_Learn).
