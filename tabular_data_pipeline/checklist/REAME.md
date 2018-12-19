# Checklist for Data Science Projects with Tabular Data

---

### Before Starting the Project (before touching the data)

<br>

**QUESTION / ANSWER**  

- What question are you asking/answering and for whom?
- Why is your client interested in the answer? Understand the context for the question and the scientific or business application.
- Determine the type of data analytic question (e.g. exploration, association causality).

<br>

**DATA**  

- What data are you going to need to answer the question?
- Where are you going to get the data?
- Consider whether the question can be answered with the available data.
- What is the potential size of the data?
- What data cleaning, munging, scraping, massaging, etc will I need to do to this data?
- Understand how the data was collected, or how the experiment was designed.

<br>

**METHODS**  

- What methods/techniques are you going to try?
- Why do I think these are the correct methods/techniques to use for this type of problem and data set?
- Are there similar projects / papers that have already done this that I can learn from before I get started?
- Are these techniques ones that I would want to use/do in a data science job?

<br>

**DEFINITION OF SUCCESS**

- How will I know I did the analysis and project correctly?
- What are key parts of the project that will tell me that I am doing things incorrectly?
- What numbers / results / insights will I sense check?
- What are simple logical chronological checkpoints I can put into my project to ensure I check to see if what I am doing is working?
- If possible at this point, define the objective metric for success.

<br>

**EXPECTED RESULT**

- What do I expect the result to be?
- Why do I expect the result to be this?
- Does this result match the results / experiences other people have had with similar methods and techniques on similar data?
- What do I expect the results to be at the simple chronological checkpoints I put into my project?

---

### Checking the Data
- Did you plot univariate and multivariate summaries of the data?
- Did you check for outliers?
- Did you identify the missing data code?

---

### Tidying the Data
- Is each variable one column?
- Is each observation one row?
- Do different data types appear in each table?
- Did you record the recipe for moving from raw to tidy data?
- Did you create a document explaining each column?
- Did you record all parameters, units, and functions applied to the data?

---

### Exploratory Analysis
- Did you identify missing values?
- Did you make univariate plots (histograms, density plots, boxplots)?
- Did you consider correlations between variables (scatterplots, correlation matrix)?
- Did you check the units of all data points to make sure they are in the right range?
- Did you try to identify any errors or miscoding of variables?
- Did you consider plotting on a log scale (or other alternative scale)?

---

### Inference
- Did you identify what large population you are trying to describe?
- Did you clearly identify the quantities of interest in your model?
- Did you consider potential confounders?
- Did you identify and model potential sources of correlation such as measurements over time or space?
- Did you calculate a measure of uncertainty for each estimate?

---

### Training and prediction
- Did you set in advance your error measure?
- Did you immediately split your data into training and test?
- Did you use cross validation, resampling, or bootstrapping only on the training data?
- Did you create features using only the training data?
- Did you estimate parameters only on the training data?
- Did you fix all features, parameters, and models before applying to the test data?
- Did you apply **only** one final model to the test data and report the error rate?
- Did you include the preprocessing step into your cross-validation process?

---

### Causality
- Did you identify whether your study was randomized?
- Did you identify potential reasons that causality may not be appropriate such as confounders, missing data, non-ignorable dropout, or unblinded experiments?
- If not, did you **avoid using language that would imply cause and effect**?

---

### Written analyses / documentation
- Did you describe the question of interest?
- Did you describe the data set, experimental design (origin of the data), and question you are answering?
- Did you specify the type of data analytic question you are answering?
- Did you specify in clear notation the exact model you are fitting?
- Did you create a [model card](https://arxiv.org/pdf/1810.03993.pdf) for each model?
- Did you explain on the scale of interest what each estimate and measure of uncertainty means?
- Did you report a measure of uncertainty for each estimate?

---

### Figures
- Does each figure communicate an important piece of information or address a question of interest?
- Do all your figures include plain language axis labels?
- Is the font size large enough to read?
- Does every figure have a detailed caption that explains all axes, legends, and trends in the figure?
- Did you use the corporative colors?

---

### Presentations
- Did you lead with a brief, understandable to everyone statement of your problem?
- Did you explain the data, measurement technology, and experimental design before you explained your model?
- Did you explain the features you will use to model data before you explain the model?
- Did you explain your model so that everyone in the room understands what is happening?
- Did you make sure all legends and axes were legible from the back of the room?

---

### Reproducibility
- Did you avoid doing calculations manually?
- Did you create a script that reproduces all your analyses?
- Did you save the raw and processed versions of your data?
- Did you record all versions of the software you used to process the data?
- Did you try to have someone else run your analysis code to confirm they got the same answers?

---

### Code
- Is your code modular?
- Did you write unit tests for your functions?
- Is your code well commented?
- Have you eliminated all errors and warnings?

---
  
### Code Packages
- Did you make your package name "Googleable"
- Did you write help files for all functions?
- Did you write a vignette?
- Did you try to reduce dependencies to actively maintained packages? 
- Did you save the version of each package (dependency) in your code?
 
---

### Sources
- [Essential Checklist for any Data Analysis project](https://blog.k2datascience.com/essential+checklist+for+any+data+analysis+or+science+project+7c4fa924e563)
- [Data Science Project Checklist To Use Before You Start A Project](https://www.datascienceweekly.org/articles/data-science-project-checklist-to-use-before-you-start-a-project-to-convey-you-can-actually-get-work-done)
