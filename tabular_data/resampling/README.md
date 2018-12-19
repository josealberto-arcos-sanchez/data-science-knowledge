# Resampling

Resampling methods help us estimate the performance of our model in new (unseen) data. But we have to be careful when applying these methods, because if done wrongly, they can lead us to overestimate the performance of our models, or to select the wrong hyperparameters.

## Resources

---
**mlr** package documentation is great in general, as it is for this particular subject:  
[mlr package doc on resampling](https://mlr.mlr-org.com/articles/tutorial/resample.html)  

---
Interesting paper explaining advantages and disadvantages of every resampling method. It is applied to genetics, and to data sets with more features than samples, but its conclusions are useful for every project:  

*"In general, 10-fold cross validation seems to be the way to go for most problems. In case you have a small quantity of samples (around 20), Leave One Out Cross Validation (LOOCV) seems to outperform 10-fold cross validation".*  

[Resampling Strategies for Model Assessment and Selection](https://www.researchgate.net/publication/226334863_Resampling_Strategies_for_Model_Assessment_and_Selection)  

---
Not read, but promising:    

*"After introducing  the three  basic  strategies,  cross-validation,  bootstrapping,  and
subsampling, nested resampling is discussed and common pitfalls and design mistakes
are highlighted when using these methods. As a summary recommendation, we suggest
consideration of the efficient leave-one-out cross-validation for fast model tuning, the
.632+  bootstrap  for  small  samples  sizes  with  low  complexity  models,  and  when  no
tuning is required, and subsampling or repeated cross-validation in all other cases (see
Figure 3)"*  

[Resampling Strategies for Model Assessment and Selection](https://www.researchgate.net/publication/226334863_Resampling_Strategies_for_Model_Assessment_and_Selection)
  
---
