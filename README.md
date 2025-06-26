# Credit-card-fraud-detection
Credir card fraud detection using machine learning.

DATASET OVERVIEW:
●	Source: European cardholders’ transactions from September 2013.
●	Duration: Records transactions over a span of 2 days.
●	Total Transactions: 284,807
●	Fraudulent Transactions: 492 (approx. 0.172%) ie highly skewed dataset.


DATA PREPROCESSING
•	HANDLING MISSING VALUES: this dataset had zero null values
•	REMOVING DUPLICATES: No duplicates, as no two transactions can have similar ids.
•	SCALING: robust scaling was applied on amount and time feature
•	SAMPLING: a technique used to handle imbalanced datasets in machine learning. It involves reducing the number of samples from the majority class to balance the               dataset and improve the performance of the model, particularly for the minority class.

PRIMARY MODEL(NEURAL NETWORK)
●	INPUT LAYER: Accepts the 30 features (including PCA components, Time, and Amount).
●	HIDDEN LAYER: A single dense layer with 2 neurons and ReLU activation.
●	BATCH NORMALIZATION: Normalizes outputs for stable learning.
●	OUTPUT LAYER: A single neuron with sigmoid activation for binary classification.
F1 SCORE OF .81

SECONDARY MODEL
1. Logistic regression
2. Random forest
3. Support vector machine
4. Isolation forest(anomaly detection)
These model have a poor f1 score generally less than .5
