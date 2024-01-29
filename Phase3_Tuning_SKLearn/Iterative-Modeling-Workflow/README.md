# Classification Workflow 1

## Learning Goals

- formulate and implement an iterative modeling workflow

## Lecture Materials

[Jupyter Notebook: Classification Workflow](classification_workflow.ipynb)

## Lesson Plan

Caution! The notebook for this lecture is very long and you will probably not get through it all. It once, in fact, was spread out over two lectures. The second "half" was revamped into a demo of workflow that includes pipelines and other modeling types, but we didn't want to get rid of the content that was in the original notebook. Students should be able to get a hang of the iterative nature of modeling even if you don't get through it all.

### Introduction (5 Mins)

This is a long notebook! You may not get through it all, but the point is to illustrate the iterative workflow of building / assessing  models, so students shouldn't in any case miss out on new concepts.

### Prepping Data (5 Mins)

For the first model we'll just use the numeric  columns and drop 'Age' since it has nulls.

### Dummy Model (10 Mins)

Use the `DummyClassifier` and build a class for easy model evaluation.

### Try `LogisticRegression` (5 Mins)

This model will make some predictions of "Survived".

### Impute Values for Nulls and One-Hot Encode for Categories (20 Mins)

We build a function for imputing. It will use the mean for numerical variables and the most-frequent value for categorical variables. The initial one-hot encoding applies to *all* categorical variables, including the name and ticket-number columns.

### Adjust Hyperparameters (5 Mins)

We can adjust the regularization, the number of iterations, the tolerance, the solver itself.

### Choose a Final Model and Evaluate it (5 Mins)

Bring in the test data and plot confusion matrices.

### Conclusion (5 Mins)

We want to do the same kind of demo lecture when we've added other models and pipelines to our repertoire.
