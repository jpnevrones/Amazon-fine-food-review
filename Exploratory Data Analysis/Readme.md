
# Exploratory Data Analysis on Amazon Fine Food Review 

## Summary

- **Datset Source**  
https://www.kaggle.com/snap/amazon-fine-food-reviews


- **Dataset Context**  
Dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

- **Dataset Contents**  
Reviews.csv: Pulled from the corresponding SQLite table named Reviews in database.sqlite
database.sqlite: Contains the table 'Reviews'

- **Data includes**  
    - Reviews from Oct 1999 - Oct 2012
    - 568,454 reviews
    - 256,059 users
    - 74,258 products
    - 260 users with > 50 reviews
    
- **Acknowledgements**  
See this SQLite query for a quick sample of the dataset.  

If you publish articles based on this dataset, please cite the following paper:  

J. McAuley and J. Leskovec. From amateurs to connoisseurs: modeling the evolution of user expertise through online reviews. WWW, 2013.  


## About the Dataset 

### Field Name 
- Id - Unique Identifier
- ProductId - unique identifier for the product
- UserId - unqiue identifier for the user
- ProfileName
- HelpfulnessNumerator - number of users who found the review helpful
- HelpfulnessDenominator - number of users who indicated whether they found the review helpful
- Score - rating in the range 1 and 5, with 1 being the worse and 5 being the best
- Time - timestamp 
- Summary - summary of the review
- Text - Content of the review

### Observed facts till now   
- Missing value for column with id "Summary" and "ProfileName"
- Orginal datset contain 5-star reviews (64%) of all reviews. Followed by 4-stars(14%),  1-star (9%), 3-star (8%), and finally 2-star reviews (5%).
- We have skewed dataset
- 75% of data is belonging to positive class(Score=4,5) - **Imbalanced dataset**
- positive reviews 
    - are way more than the negative reviews.
    - are shorter
    - are found more helpful (speaks of human cognitive processing)
- Frequent reviewers
    - write longer reviews
    - more help review 
