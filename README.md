# Amazon fine food review

This repopsistory contains various data analysis technique and subsequent models based on [Amazon fine food review dataset](https://www.kaggle.com/snap/amazon-fine-food-reviews) 

- [Exploaratory data Analysis](https://github.com/jpnevrones/Amazon-fine-food-review/tree/master/Exploratory%20Data%20Analysis/EDA-Amazon-Fine-Food-Review.ipynb)
- [Recomendation System](https://github.com/jpnevrones/Amazon-fine-food-review/blob/master/Food%20Recommendation%20System/amazonFineFoodRecommendation.ipynb)
- [Review Classification - using Random Forest + word2vec](https://github.com/jpnevrones/Amazon-fine-food-review/blob/master/Classification%20Algorithm/RandomForest-Classifier-using-wordEmbeddingFrom-word2vector-gensim.ipynb)  
  - Trained a word2vec model using Gensim package with the following parameter value ( Word vector dimensionality  = 300, Minimum word count =40, Number of threads to run in parallel  = 3,  Context window size = 10 and downsampling rate for frequent words = 1e-3).
  - Created Feature vector to be used by random forest model by averaging word embeddings of all words in the review.
  - Accuracy : 
  - ROC curve 
  ![ROC CURVE](/result/ROCcurve_RandomForest-Classifier-using-wordEmbeddingFrom-word2vector-gensim.PNG)
  

