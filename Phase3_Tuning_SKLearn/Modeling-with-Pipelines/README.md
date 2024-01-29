# Classification Workflow 2

## Learning Goals

- formulate and implement an iterative modeling workflow

## Lecture Materials

[Jupyter Notebook: Workflow with Pipelines](workflow_with_pipelines.ipynb)

## Lesson Plan

### Introduction (5 Mins)

Let's do another workflow demo now that we have more tools!

### Pipelines with `FunctionTransformer` (5 Mins)

The `FunctionTransformer` will turn functions into transformers so that they can be used in pipelines.

### Pipelines with `ColumnTransformer` (10 Mins)

The use of the `ColumnTransformer` requires the user to specify which columns should be transformed! Note the `remainder='passthrough'` setting which leaves unnamed columns (untransformed but) ready for use after the named columns are transformed.

### Trying Different Models at the End of the Pipeline (5 Mins)

All `sklearn` models can be used in a pipeline! 

### GridSearching the Pipeline (10 Mins)

Note the double-underscore syntax for specifying the hyperparameters associated with a particular transformer in the pipline.

### `imblearn`'s Pipeline for Imbalanced Datasets (10 Mins)

If you want to use `imblearn` tools like `SMOTE`, you'll need to use this library's proprietary pipelines rather than `sklearn`'s.

### Exercise (10 Mins)

Practice with pipelines and transformers.

### Conclusion (5 Mins)

Good to remind that pipelines are great for streamlining code and for cross-validating properly. But they are also very hard to debug! So good to work out the preprocessing and modeling kinks BEFORE bringing in pipelines!