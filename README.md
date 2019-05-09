# Personalized-Cancer-Diagnosis
Objective: To classify the given genetic variations based on text-based clinical literature.

Description: The dataset was obtained from Kaggle. It contains various features such as Genes, Text, Variation and Label (Type of Cancer). Univariate analysis of each feature was done to check feature importance. These features were converted into their respective vector forms. The task is to minimize the log-loss and determine how well the model performed.

Dataset Link:
https://www.kaggle.com/c/msk-redefining-cancer-treatment/data


Data: Memorial Sloan Kettering Cancer Center (MSKCC)

Download training_variants.zip and training_text.zip from Kaggle.

CaseStudy Flow:
================
1. The objective of the case study was to Classify the given genetic variations/mutations based on evidence from text-based clinical literature.
2. The case study demands very high interpretability and probabilistic outputs
3. Dataset contains ID,Gene,Variation,Class and Text as feature.
4. On EDA on class label it was found that distribution of classes were not balanced. More data pts. was present in classes 1,2,4 and 7 as compared to other.
5. Gene feature found to be most important feature followed by variation and text.
6. Features are encoded as response encode and onehot encoding.
7. Various ML models were tired and tested to obtain the best results.
8. For correctly classified pts. differance in probabilities of classes were high which is as expected.
9. Random Forest with onehot encoding took the longest to run.
10. Random Forest with onehot encoding showed incorrectly classified pt. as correctly classified.
11. As LR with onehot encoding performed best among all the models. So , it was considered during feature engineering.
12. During Feature engineering, argmax of response encoded gene feature was considered along with one hot encoded feature.
13. All the results are summarized in tabular format and observation are noted whenever necessary.
