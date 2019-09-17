# RHOASo
RIASC Hyper-Optimization Automatic Software. An algorithm for optimization of discrete hyperparameters.

# Example usage
```Python
import sklearn.ensemble
from seleccion_nueva import selection_n
import numpy as np
import sklearn.datasets

data, labels = sklearn.datasets.load_breast_cancer(return_X_y=True)
params, acc, evaluations, num_evals = selection_n(
    sklearn.ensemble.RandomForestClassifier, data, labels, {'max_depth': 10, 'n_estimators': 50}
)
```
