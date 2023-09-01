# hART-heart-failure-Attentive-Risk-Trajectory

This repo provides a sample code to experiment with the hART model. The notebook is best run on Google Colab. 

The notebook titled 'hART.ipynb' is divided into section to ease the interpretability and usage. 
Here's a short description of each section:

1. Imports
     a) Contains all Imports needed to run the notebook
     b) Upload the data needed to run the notebook, Note: Synthetic data is provided in the GitHub             repo ('synthetic.csv')
     c) Apply the specific exclusion criterions for our study

2. Preprocessing
    a) Contains helper functions to turn event-based data into sequential input and HF labels
    b) Data split

3. Attention Helper Functions
    a) Custom function used in the Models

4. MODELS
    a) Contains the novel hART model and previously developed DHTM model
       (https://github.com/li-lab-mcgill/recurrent-disease-progression-networks)
    b) Allows you to train and evaluate the performance of the models

5. Patient Population Trajectory Sample
    a) Provides the ability to experiment with the hART-predicted trajectory at a population level
    b) Choose a subgroup to test (severe CHD vs. Non Severe CHD)
    c) Output is HF Trajectory + Attention Matrix (Heatmap) + Actual Distribution of HF for population

6. Individualized Trajectory Sample
    a) Provides the ability to experiment with the hART-predicted trajectory at an individualized level
    b) Choose a baseline to test (non-severe CHD patients) and a specific individual (patient = ) 
    c) Output is HF Trajectory + Patient's Medical Event History + Attention Matrix (Heatmap)


NOTES:

1. The synthetic is NOT the real data used in the study. It is a representation of the actual data
2. Use the 'sample' data frame to help run the code faster (the whole data takes hours to preprocess)
3. The synthetic data is in a zip file due to size (please unzip to use)
    
