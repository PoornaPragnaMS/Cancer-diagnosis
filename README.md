# Cancer-diagnosis
This repository provides data science operations, approaches and algorithms for Personalized cancer diagnosis.

In this project we are going to classify genetic mutations based on clinical evidence (text).

There are nine different classes a genetic mutation can be classified on.

This is not a trivial task since interpreting clinical evidence is very challenging even for human specialists. Therefore, modeling the clinical evidence (text) will be critical for the success of your approach.

Both, training and test, data sets are provided via two different files. One (training/test_variants) provides the information about the genetic mutations, whereas the other (training/test_text) provides the clinical evidence (text) that our human experts used to classify the genetic mutations. Both are linked via the ID field.

Therefore the genetic mutation (row) with ID=15 in the file training_variants, was classified using the clinical evidence (text) from the row with ID=15 in the file training_text


The workflow is as follows

  1: A molecular pathologist selects a list of genetic variations of interest that he/she want to analyze

  2: The molecular pathologist searches for evidence in the medical literature that somehow are relevant to the genetic variations of        interest

  3: Finally this molecular pathologist spends a huge amount of time analyzing the evidence related to each of the variations to     classify them.

Our goal here is to replace step 3 by a machine learning model.
The molecular pathologist will still have to decide which variations are of interest, and also collect the relevant evidence for them. 
But the last step, which is also the most time consuming, will be fully automated.

As a first step we are going to perform Exploratory Data Analysis by Preprocessing of text and following the descriptive statistical approach of Univariate Analysis of Gene Feature, Variation feature and Text Feature available in the dataset.

Once the impact of each feature is analysed using descriptive statistic approach, we use following machine learning model and stacking three types of features:

  1: Base Line Model being Naive Bayes
  
  2: K Nearest Neighbour Classification
  
  3: Logistic Regression
  
  4: Linear Support Vector Machines
  
  Finally stacking the models.


