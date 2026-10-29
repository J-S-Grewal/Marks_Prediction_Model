# IDC409 Data Science Project: Student Performance Prediction

This repository contains the code, analysis figures, derived data, and
model prediction results for the IDC409 Data Science project on
predicting student performance.

## Project overview

The project studies student final-grade prediction for two subjects:

-   **Mathematics**
-   **Portuguese language**

It compares models trained with and without the earlier-period grades
**G1** and **G2**, and evaluates how their inclusion affects prediction
performance.

## Repository structure

``` text
IDC409_Project/
├── Codes/
│   ├── 01_data_audit_Mat.ipynb
│   ├── 01_data_audit_Por.ipynb
│   ├── 02_models_mat.ipynb
│   ├── 02_models_por.ipynb
│   └── Data.ipynb
├── Data_Analysis_and_Results/
│   ├── Mathematics_Initial_Data_Analysis/
│   ├── Mathematics_Machine_Learning_Data_Analysis/
│   ├── Portuguese_Initial_Data_Analysis/
│   └── Portuguese_Machine_Learning_Data_Analysis/
├── Data_used_and_Derived/
│   ├── Extra_Files/
│   ├── Results/
│   └── student_data.xlsx
├── README.md
└── requirements.txt
```

## Contents

### `Codes/`

Jupyter notebooks for data inspection, exploratory analysis, model
development, and error analysis.

-   `01_data_audit_Mat.ipynb` --- data audit and initial analysis for
    Mathematics.
-   `01_data_audit_Por.ipynb` --- data audit and initial analysis for
    Portuguese.
-   `02_models_mat.ipynb` --- Mathematics prediction models and error
    analysis.
-   `02_models_por.ipynb` --- Portuguese prediction models and error
    analysis.
-   `Data.ipynb` --- additional data-related notebook.

### `Data_Analysis_and_Results/`

Figures and outputs from initial data analysis and machine-learning
analysis for both subjects.

### `Data_used_and_Derived/`

The dataset, supporting files, and model prediction results.

-   `student_data.xlsx` --- dataset used by the project.
-   `Extra_Files/` --- additional source or supporting files.
-   `Results/` --- model prediction spreadsheets, including results for
    models trained with and without G1 and G2.

## Models evaluated

The notebooks compare the following model types:

-   Linear Regression
-   Ridge Regression
-   Decision Tree
-   Random Forest
-   Gradient Boosting
-   XGBoost
-   Multilayer Perceptron (MLP)
-   Mixture of Experts (MoE)
-   Radial Basis Function Neural Network (RBFNN)
-   Residual MLP (ResMLP)

The exact preprocessing, training procedure, and evaluation are
documented in the relevant notebooks.

## Evaluation

Prediction performance is assessed using:

-   **Root Mean Squared Error (RMSE)**
-   **Mean Absolute Error (MAE)**
-   **Coefficient of determination (R²)**

The analysis also examines prediction errors and residual distributions,
and compares performance with and without G1 and G2.

## Setup

Use Python with the packages listed in `requirements.txt`.

From the repository directory, create and activate a virtual
environment, then install the dependencies:

``` bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

On Windows, activate the environment with:

``` powershell
.venv\Scripts\Activate.ps1
```

## Running the project

1.  Open the repository in VS Code or Jupyter.
2.  Select the Python environment in which the dependencies are
    installed.
3.  Run the notebooks in `Codes/`.
4.  Review saved figures in `Data_Analysis_and_Results/` and prediction
    spreadsheets in `Data_used_and_Derived/Results/`.

Run notebooks from the project directory and check file paths if your
working directory differs.

## Notes

-   The saved prediction spreadsheets contain model outputs; the
    notebooks document how those outputs are generated and evaluated.
-   Virtual environments, cache files, and other machine-specific
    temporary files should not be committed.
