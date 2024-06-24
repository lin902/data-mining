# data-mining
two projects about data mining strategies and some ML methods
# final project
# General Instructions
The final project has 7 questions. Each question has 1 readme file. The question requirement are in the word.
# Problem Tasks
## Q1: Supervised Outlier Detection (15 pts)
**Background**: 
Detecting falls in pets using a wearable device that records signals corresponding to various variables.

**Requirements**:
Handle data imbalance and prioritize recall rate for class 1 (falls).

**Solving Approach**:

Data exploration to understand the variables and the distribution.
Use of outlier detection algorithms, potentially Isolation Forest or One-Class SVM, considering the imbalance.
## Q2: Weather Recognition (15 pts)
**Background**: 

Developing an image classifier for different weather conditions based on raw image data.

**Requirements**:

Design a dataloader and train a deep learning model for at least 50 epochs.

**Solving Approach**:

Image preprocessing including resizing and one-hot encoding of labels.
Selection of a CNN architecture and training with early stopping and checkpointing.
## Q3: Short Video Classification (15 pts)
**Background**: 

Classifying short videos into categories using an automatic algorithm.

**Requirements**:

Implement a classification algorithm without using pre-trained models directly.

**Solving Approach**:

Feature extraction from video frames using techniques like CNN.
Training a machine learning model with extracted features and categorical labels.
## Q4: Recommendation and Business Analysis (15 pts)
**Background**: 

Analyzing retail transaction records to provide business insights and sales suggestions.

**Requirements**:

Create visual methods for insights and use association rule analysis for recommendations.

**Solving Approach**:

Data visualization for trends and patterns.
Implementation of association rule mining using algorithms like Apriori or FP-Growth.
## Q5: Smoke Status Recognition (15 pts)
**Background**: 

Predicting a patient's smoking status from biometric information.

**Requirements**:

Implement a binary classification algorithm.

**Solving Approach**:

Exploratory data analysis and preprocessing.
Application of classification algorithms, such as logistic regression or random forest.
## Q6: Bank Customer Clustering (10 pts)
**Background**: 

Clustering bank customers for operational efficiency and tailored services.

**Requirements**:

Use at least three different clustering algorithms.

**Solving Approach**:

Data exploration and visualization to understand customer attributes.
Application of clustering algorithms like K-Means, DBSCAN, and Hierarchical Clustering.
## Q7: Social Media Network Analysis (15 pts)
**Background**: 

Analyzing social network data to understand social relationships.

**Requirements**:

Conduct various graph analyses and community detection.

**Solving Approach**:

Use of network analysis techniques and community detection algorithms.
Visualization of network properties and community structures.
# code:
	
	Q1:code in dsaa5002_project\Q1\Q1.ipynb
 
	Q2:code in dsaa5002_project\Q2\Q2.ipynb
 
	Q3:code in dsaa5002_project\Q3\Q3_locally.ipynb & Q3_colab.ipynb
 
	Q4:code in dsaa5002_project\Q4\Q4_locally.ipynb & Q4_colab.ipynb
# subsubmission:
	
 excel in dsaa5002_project\submission\Task1.xlsx & Task2.xlsx（by list）& Task2_2.xlsx (by knowledge graph)
**Q1**:
Three methods were used for similarity matching and keyword extraction after preprocessing the text by removing numbers, symbols, and tokenizing nouns.

 The first method utilized the bert-base-chinese model to calculate similarity using cosine_similarity, but it did not yield satisfactory results. 

The second method involved direct keyword matching, resulting in an extraction rate of 45.07%. 

The third method replaced bert-base-chinese with bert-wwm, which improved the extraction rate to 55.68%.

**Q2**: 
Three methods were used for sentiment analysis on the data. 

The first method involved comparing the count of positive and negative words using a sentiment analysis lexicon. However, this method sometimes resulted in an equal count of neutral words. 

The second method utilized the results from the first method to train a model. The pipeline of the model included preprocessing, tokenization, and a classification step with L2 regularization. However, the accuracy of this model was very low, only 0.47, as it couldn't learn effective features.

The third method involved using the pre-trained sentiment analysis dictionary FinBERT 1.0, specifically trained for financial news. The positive-to-negative word ratio achieved was 11.01.

**Q3**：
Two methods were attempted. 

- The first method involved directly connecting to a database in Colab, but it resulted in an infinite loop. 

- The second method was to download the community edition and create a database using the command line, followed by importing the data.

**Q4**：
Two methods were attempted. 

1.Querying and setting rules for Implicit_Positive_Company and Implicit_Negative_Company in Neo4j knowledge graph，which needs more than 7146.63s.

2.Directly searching in the list, first find the corresponding company ID, then check if :START_ID and :END_ID are present, and then perform rule-based evaluation. This process needs 4670.64s which is quicker than query in the knowdge graph.

