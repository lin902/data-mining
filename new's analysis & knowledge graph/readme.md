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

The first method involved directly connecting to a database in Colab, but it resulted in an infinite loop. 

The second method was to download the community edition and create a database using the command line, followed by importing the data.

**Q4**：
Two methods were attempted. 

1.Querying and setting rules for Implicit_Positive_Company and Implicit_Negative_Company in Neo4j knowledge graph，which needs more than 7146.63s.

2.Directly searching in the list, first find the corresponding company ID, then check if :START_ID and :END_ID are present, and then perform rule-based evaluation. This process needs 4670.64s which is quicker than query in the knowdge graph.
