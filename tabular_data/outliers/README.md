# Outliers

An outlier is any data point that is distinctly different from the rest of your data points. When you’re looking at a variable that is relatively normally distributed, you can think of outliers as anything that falls 3 or more standard deviations from its mean. While this will suffice as a working definition, keep in mind that there’s no golden rule for defining what an outlier is.

In general, outliers belong to one of two categories: a mistake in the data or a true outlier. The first type, a mistake in the data, could be as simple as typing 10000 rather than 100.00 – resulting in a big shift as we’re analyzing the data later on. The second type, a true outlier, would be something like finding Bill Gates in your dataset. His profile probably looks so different from the other people in your list that including him might skew your results. It’s important to distinguish these types because we’ll handle them differently in an analysis. It’s subjective. It’s up to you as the analyst to determine which data points are outliers in any given dataset.

Now, how do we deal with outliers? Here are four approaches:

### 1. Drop the outlier records.

In the case of Bill Gates, or another true outlier, sometimes it’s best to completely remove that record from your dataset to keep that person or event from skewing your analysis.

### 2. Cap your outliers data.

Another way to handle true outliers is to cap them. For example, if you’re using income, you might find that people above a certain income level behave in the same way as those with a lower income. In this case, you can cap the income value at a level that keeps that intact.

### 3. Assign a new value.

If an outlier seems to be due to a mistake in your data, you try imputing a value. Common imputation methods include using the mean of a variable or utilizing a regression model to predict the missing value.

### 4. Try a transformation.

A different approach to true outliers could be to try creating a transformation of the data rather than using the data itself. For example, try creating a percentile version of your original field and working with that new field instead.

Just how much an outlier affects your analysis depends, not surprisingly, on a few factors. One factor is dataset size. In a large dataset, each individual point carries less weight, so an outlier is less worrisome than the same data point would be in a smaller dataset. Another consideration is “how much” of an outlier a point might be – just how far out of line with the rest of your dataset a single point is. A point that is ten times as large as your upper boundary will do more damage than a point that is twice as large.

---

## Sources
[Handling outliers](https://www.rapidinsightinc.com/handle-outliers/)
