# -Predict-Students-Dropout-and-Academic-Success

Project Overview

This project explores student-related data to understand patterns
associated with academic outcomes and develops a machine learning model
to classify students into three outcome categories:

-   **Dropout**
-   **Enrolled**
-   **Graduate**

The project uses the **Predict Students' Dropout and Academic Success**
dataset from the UCI Machine Learning Repository. Python is used for
data inspection, cleaning, exploratory data analysis (EDA), feature
preparation, classification modelling, and evaluation.

The goal is to turn educational data into meaningful insights that may
support academic planning and further investigation. Model predictions
are intended for decision support, not as guaranteed outcomes for
individual students.

 Dataset Information

  Item                   Description
  ---------------------- ------------------------------------------------
  Dataset                Predict Students' Dropout and Academic Success
  Source                 UCI Machine Learning Repository
  Dataset ID             697
  Records                4,424
  Input features         36
  Target variable        `Target`
  Target classes         Dropout, Enrolled, Graduate
  Domain                 Education Analytics and Machine Learning
  Programming language   Python

**Dataset link:**
https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success\
**DOI:** https://doi.org/10.24432/C5MC89

The dataset includes demographic and admission attributes, prior
qualification information, family and socioeconomic variables, first-
and second-semester curricular-unit measures and grades, and selected
macroeconomic indicators. Refer to the UCI documentation for the
official feature definitions and encoded category values.

## Project Objectives

1.  Understand the structure, size, and variables in the dataset.
2.  Identify missing values, duplicate records, inconsistent formats,
    and invalid values.
3.  Analyze the distribution of Dropout, Enrolled, and Graduate
    outcomes.
4.  Explore demographic, admission, socioeconomic, and academic
    characteristics.
5.  Examine first- and second-semester performance in relation to
    student outcomes.
6.  Prepare features for machine learning while preventing data leakage.
7.  Train and compare multiclass classification algorithms.
8.  Evaluate model performance using appropriate metrics for all three
    classes.
9.  Present verified findings, limitations, and recommendations through
    visualizations and documentation.

## Tools and Technologies

-   **Python** -- programming and analysis
-   **Pandas** -- data loading, cleaning, transformation, and analysis
-   **NumPy** -- numerical operations
-   **Matplotlib** -- data visualization
-   **Seaborn** -- statistical visualization
-   **Jupyter Notebook** -- interactive analysis and documentation

## Project Workflow

### 1. Data Collection and Inspection

-   Download the dataset and documentation from the UCI repository.
-   Load the data using Pandas.
-   Inspect the records, columns, data types, and sample values.
-   Review statistical summaries and target-class distribution.
-   Check official feature descriptions, especially for encoded
    categorical values.

### 2. Data Cleaning and Preprocessing

-   Check for missing values and duplicate records.
-   Investigate unusual or implausible values before making changes.
-   Validate numerical and categorical columns.
-   Encode categorical variables and scale numerical variables where
    required.
-   Split the data into training and testing sets, using stratification
    where appropriate.
-   Fit preprocessing transformations on training data only, then apply
    them to test data to avoid data leakage.
-   Document preprocessing decisions.

### 3. Exploratory Data Analysis (EDA)

-   Analyze the number and percentage of records in each target class.
-   Compare outcomes across courses and selected admission categories.
-   Explore demographic, scholarship, tuition-fee, and other available
    attributes.
-   Examine semester grades, units enrolled, units evaluated, and units
    approved.
-   Explore relationships among suitable numerical variables.

### 4. Model Evaluation

Model performance will be evaluated using:

-   Accuracy
-   Precision
-   Recall
-   F1-score
-   Macro F1-score
-   Confusion matrix

Per-class performance will be reviewed, with particular attention to
recall for the Dropout class. Actual performance results will be added
after experiments are completed.

### 5. Data Visualization

Planned visualizations may include:

-   Target-class distribution bar chart
-   Outcome distribution across courses
-   Box plots of semester grades by target class
-   Semester units approved or evaluated by outcome
-   Outcome distribution by scholarship or tuition-fee status
-   Correlation heatmap for selected numerical features
-   Confusion matrix for model predictions

The final visualizations will depend on the available columns and data
quality.


.  Download the dataset from the [UCI Machine Learning
    Repository](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success),
    place it in the appropriate `data/raw/` folder, and run the
    notebooks in order.

## Expected Deliverables

-   A cleaned dataset or reproducible data-cleaning workflow
-   Python Jupyter Notebook(s) for data inspection and preprocessing
-   EDA results and visualizations
-   A documented feature-preparation and modelling workflow
-   Evaluation results for at least one multiclass classification model
-   Model metric comparison and a confusion matrix
-   Summary of verified findings, recommendations, and limitations
-   Final project report and GitHub documentation

## Limitations and Responsible Use

-   The analysis is limited to the records and variables in this
    dataset.
-   The dataset may not represent all higher education institutions or
    student populations.
-   Historical and institutional context may limit generalization to
    other settings.
-   Class imbalance and input-feature quality may affect model
    performance.
-   Semester performance measures mean that models using those fields
    cannot be described as admission-time predictions.
-   The model identifies statistical patterns; it does not establish the
    causes of student dropout.
-   Demographic associations must not be treated as proof of cause or
    used as a basis for unfair treatment.
-   Any real-world use would require further validation, privacy
    safeguards, fairness review, and human oversight.


## Conclusion

This project applies Python-based data analytics and machine learning to
explore student characteristics, academic performance, and recorded
educational outcomes. Through data cleaning, exploratory analysis,
feature preparation, classification modelling, and evaluation, the
project aims to produce useful insights while demonstrating practical
data analytics skills.

Predictions should be treated as support for further investigation, not
as definitive judgements about individual students.
