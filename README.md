# sensim
Given two sentences returns the similarity score between them as a value between 0 and 1

Implemented the paper  [UdL at SemEval-2017 Task 1: Semantic Textual Similarity Estimation of English Sentence Pairs Using Regression Model over 
Pairwise Features](https://www.aclweb.org/anthology/S17-2013)


Input  : 2 sentences

Output :  Similarity Score

Developed in python3

## Approach

To compute the similarity we use 5 features which are

 1) Average of w2v Cosine Similarity of all the PoS tag pairs
 2) Average of w2v Cosine Similarity of all the NE tag pairs
 3) Cosine similarity of the sentence BoW vector pair
 4) Absolute difference of the number summation
 5) Absolute difference of the number of characters
 
 This figure shows the importance of each feature in predicting a similarity score
 
 ![alt text](https://github.com/Sanjithae/sensim/blob/master/Figure1.PNG)
 
 After obtaining the features we apply Random Forest Ensemble Learning to predict the final similarity score.
 
 ## To run the program
 
 python main.py
 
 
 ## Evaluation Metrics
 
 Pearson Correlation Coefficient.
 
 ## Benchmark Datasets 
 
 1) SICK 2014
 2) SemEval 2017
 3) SemEval 2014

## Results




## Jupyter Notebook

You can see the execution of each function [here.](https://github.com/Sanjithae/sensim/blob/master/sentence_similarity.ipynb)

## Youtube Video

Explanation of the code [here.]()



## Citation
Al-Natsheh, Hussein T.  and  Martinet, Lucie  and  Muhlenbach, Fabrice  and  ZIGHED, Djamel Abdelkader,
UdL at SemEval-2017 Task 1: Semantic Textual Similarity Estimation of English Sentence Pairs Using Regression Model over 
Pairwise Features,Proceedings of the 11th International Workshop on Semantic Evaluation (SemEval-2017),August,2017,Vancouver, Canada,Association for Computational Linguistics,115--119.
(http://www.aclweb.org/anthology/S17-2013)
