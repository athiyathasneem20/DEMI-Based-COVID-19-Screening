COVIDCARE DEMI: Home-Based COVID-19 Screening
This project develops an interpretable AI-based screening prototype for COVID-19 using information that can be reported at home before clinical evaluation.
The project uses the COVIDCARE MIT Phase II observational dataset and applies a DEMI evidence-weighting approach to binary pre-test features. The system constructs feature-level evidence weights from 2×2 contingency tables and combines these weights to produce an individualized screening probability.
Key results
•	Analytic cohort: 559 participants
•	PCR positive: 58
•	PCR negative: 501
•	Binary pre-test features: 75
•	Train/test split: 75/25
•	ROC-AUC: 0.824
•	Accuracy: 68.6%
•	Sensitivity: 80.0%
•	Specificity: 67.2%
•	Precision: 22.6%
•	F1 score: 35.3%
Technology
•	Python
•	Jupyter Notebook
•	pandas / NumPy
•	scikit-learn
•	matplotlib
•	ipywidgets
•	DEMI evidence-weighting methodology
How to run
1.	Clone or download the repository.
2.	Open COVIDCARE_DEMI_Final_Project.ipynb in Jupyter Notebook or JupyterLab.
3.	Ensure the dataset, survey dictionary, and DEMI knowledgebase are in the expected project directory.
4.	Run the notebook cells in sequence.
5.	Review the preprocessing, DEMI knowledgebase, model evaluation, ROC curve, and interactive screening section.
6.	In the interactive section, enter patient responses and select Calculate Screening Risk to obtain the estimated screening probability.
Important: This project is a research prototype for screening and does not diagnose COVID-19. A positive or high-risk result should be followed by appropriate testing or clinical evaluation. The reported model has not undergone external clinical validation.
Causal interpretation
The project includes a directed acyclic graph (DAG) to identify potential confounding, mediation, and selection issues. DEMI weights are interpreted as predictive evidence, not causal effects. No ATE or ACE was estimated because the observational dataset does not define a single treatment intervention suitable for causal effect estimation.
Repository purpose
The repository is intended to provide a reproducible record of the course research project, including the data-processing workflow, DEMI analysis, model evaluation, and interactive Jupyter implementation.

