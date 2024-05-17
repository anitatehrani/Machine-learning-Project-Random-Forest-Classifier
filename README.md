# Machine Learning Project - Random Forest Regressor Optimization

This project focuses on optimizing a Random Forest Regressor model using GridSearchCV from the sklearn library. The goal is to find the best hyperparameters that will yield the highest accuracy for the model.

## Project Structure

The project consists of a single Jupyter notebook file, `MachinLearning_project-2.ipynb`.

## Code Overview

The code begins by importing necessary libraries, including `GridSearchCV` and `RandomForestRegressor` from sklearn, and `numpy`.

A grid of hyperparameters is defined for the Random Forest Regressor model. This includes:

- `n_estimators`: The number of trees in the forest. The grid searches from 100 to 1000 in steps of 100.
- `max_depth`: The maximum depth of the tree. The grid searches from 15 to 20.
- `max_features`: The number of features to consider when looking for the best split. The grid considers 1 or 'sqrt'.

`GridSearchCV` is then initialized with the `RandomForestRegressor` as the estimator, the defined grid as the parameter grid, and accuracy as the scoring method. The cross-validation fold is set to 5, and all processors are used (`n_jobs=-1`).

The `GridSearchCV` is fitted to the data (`x`, `y`), and the best parameters are extracted and stored in `best_params`.

## Usage

To use this project, you will need to provide your own data (`x`, `y`) to fit the `GridSearchCV`. After running the code, you can check the `best_params` variable to see the best parameters found by the grid search.

## Dependencies

- Python
- sklearn
- numpy

## Report
#### -[Canva File](https://www.canva.com/design/DAF_gFQy9cU/QWdyZUKmBciXM0MElTQTUg/view?utm_content=DAF_gFQy9cU&utm_campaign=designshare&utm_medium=link&utm_source=editor)

### Contributors

#### -[@mohiabd99](https://github.com/Mohiabd99)
#### -[@anitatehrani](https://github.com/anitatehrani)
