# Fairness-Transparency Trade-Off: How does increasing fairness in an interpretable model influence accuracy?
Hello and welcome to my project. The dataset required for the code demonstration is "survey_lung_cancer.csv" however I did not add the underscores when loading the dataset into the .ipynb file so be aware of that.

The code demonstration includes the following:
1. Importation of Libraries
2. Loading the Dataset
3. The Exploratory Analysis
    - this is where I look if there are any missing values, and check what the class/gender/cancer by gender distribution looks like. Following the simple commands, I then graph the distributions using bar plots.
4. Data Pre-Processing
    - in this step I create a copy of the original dataset before then encoding the non-numerical variables: boolean LUNG_CANCER variable, and categorical GENDER variable. Following the encoding, I then train the calssifier and use the imported libraries to look at the classification report, as well as teh confusion matrix for the TP, TN, FP, FN values of whether the patients have cancer.
5. Creation of Helper Function: compute_group_metric
    - this function computes the fairness metrics seperately for each demographic group before then adding them to the results dictionary containing all relevant information regarding the metrics found within the dataset.
6. First Fairness Metric: Equalized Odds
    - get the TPR and FPR for male patients and female patients, calculate the difference between demographic groups, then plot them as bar plots.
7. Second Fairness Metric
    - get the PPV for male patients and female patients then calculate the difference between demographic groups, before plotting them as bar plots.
8. Side-by-side comparison of the two fairness metrics, seen illustrated through bar plots, with the difference between the demographic groups added above the respective bars.

The analysis of the code is not discussed within the .ipynb file, but briefly within the report that can be found within this repository. 
