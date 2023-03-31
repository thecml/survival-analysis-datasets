# survival-datasets

A simple data loader for the most common datasets in Survival Analysis. Currently the following are included: 
* Veterans Lung Cancer (https://scikit-survival.readthedocs.io/en/stable/api/generated/sksurv.datasets.load_veterans_lung_cancer.html)
* German Breast Cancer Study Group (GBSG2) (https://scikit-survival.readthedocs.io/en/stable/api/generated/sksurv.datasets.load_gbsg2.html)
* AIDS dataset (https://scikit-survival.readthedocs.io/en/stable/api/generated/sksurv.datasets.load_aids.html)
* NHANES (https://shap.readthedocs.io/en/latest/generated/shap.datasets.nhanesi.html)
* SUPPORT Study to Understand Prognoses Preferences Outcomes and Risks of Treatment (from DeepSurv paper, https://arxiv.org/abs/1606.00931)
* METABRIC The Molecular Taxonomy of Breast Cancer International Consortium (from DeepSurv paper, https://arxiv.org/abs/1606.00931)
* WHAS500 Worcester Heart Attack Study (https://scikit-survival.readthedocs.io/en/stable/api/datasets.html)
* FLCHAIN (https://scikit-survival.readthedocs.io/en/stable/api/datasets.html)
* SEER (from Kaggle, https://www.kaggle.com/code/jnegrini/breast-cancer-dataset)

## Requirements

* Python 3.8 or later
* scikit-survival 0.17.2 or later
* pandas 1.4.3 or later
* numpy 1.22.4 or later
* shap 0.41 or later
* pyarrow 11.0 or later

## Installation

Simply install via pip:
```
pip install survival-datasets
```

## Examples

Import the datasets module from the package and load your dataset of choice:
```
from survdata import datasets

if __name__ == "__main__":
    X, y = datasets.load_seer_dataset()
```
