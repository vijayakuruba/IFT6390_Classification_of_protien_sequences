# IFT6390_Text-Generation

Final year project for IFT 6390- Fundamentals of Machine learning
Team Members: \
Kuruba Vijaya Lakshmi \
Saadaoui Houda \
Binulal Narayanan

In this project, we use different Data cleaning strategies, Imputation techniques and Machine Learning models to classify protein sequences as AMP or non-AMP.

# Approach



1.   Exploratory data analysis 
2.   Based on data analysis we found 2 challenges:
*   Imbalanced dataset: No of non-AMPs are more way higher than AMP. 
*   the distribution of the sequence lengths varies a lot between the two classes.

3.   We have Tried 4 different options with dataset to address Imbalance in sequence lengths
*   Original dataset

*   Dataset 1: We reconstructed Non Amp sequences such that we ignored the samples whose sequence legths are not in AMP sequences. 
*   Dataset 2: Dataset in which sequence lengths >125 is ignored, based on fact that 95 percentile of AMP sequence length is 125.
*   Dataset 3 :   Considered only Amplify dataset since the samples and sequence lengths are balanced
4.   For Data samples imbalance , Tried Oversampling and Undersampling Techniques.
5.   Models :
*   1. Random forest classifier + Oversampling + Dataset1
*   2. Random forest classifier + Oversampling + Dataset2
*   3. Random forest classifier + Undersampling + Dataset1
*   4. SVM Classifier + No Sampling +Cost penalised+ Original dataset 
*   5. Neural networks + Dataset 3 
6.   Results

This repositary has 2 colab files. 
1. IFT_6390_Final_Project_1_.ipynb  - It contains Models option1 - option 5
2. IFT_6390_Final_Project_1_supp.ipynb  - It contains different data strategy (data split on different ratios) modelled with Random forest
