# Prediction-of-Cell-Count
This work aims to predict counts of different cell types from images of human body tissues. Data used for this project was sourced from the CoNIC: Colon Nuclei Identification and Counting Challenge. Please see https://github.com/TissueImageAnalytics/CoNIC and https://arxiv.org/abs/2111.14485 for more information regarding this challenge.

The different cell types in focus are listed below:

T1: neutrophil
T2: epithelial
T3: lymphocyte
T4: plasma
T5: eosinophil
T6: connective

Comprehensive EDA is carried out to identify features that correlate with the target variable and model around them. This includes mapping the images to Haematoxylin-Eosin-DAB(HED) space as the H-channel 'stains' the image to highlight the cells we are interested in. Gray Level Co-occurence Matrix features were also found to add value to the predictor.

Different approaches are analysed, from classic Ordinary Least Squares(OLS) regression to a pre-trained ResNet18 model to see what works best for this task.

Multiple evaluation metrics such as R2 score, RMSE, Pearson Correlation Coefficient and Spearman Correlation Coefficient are considered to capture a robust picture of how the models perform.
