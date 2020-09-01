# Amazon Instrument Reviews
The data used for this project was downloaded from the Kaggle dataset found
[here](https://www.kaggle.com/eswarchandt/amazon-music-reviews).  
The purpose of this project to perform sentiment analysis to help the organization understand their customer 
feedback so they can concentrate their focus on addressing customer issues with their products. 
Here we build the model which has highest accuracy in classifying the feedback as positive, neutral, or negative.  Where a 
rating of 4 or 5 is positive, 3 is neutral, and 2 or 1 is negative.  This will enable to company to 
have a better grasp of the customers feedback in order to improve their service and thus create loyal customers, 
increase business, fame, brand value, and profits.

Task 1 <br>
Categorize opinions expressed in feedback forums
<br>
Task 2 <br>
Classify individual comments/reviews and determine overall rating based on individual
comments/reviews.

**Columns**
* `reviewerID` - ID of the reviewer, e.g. A2SUAM1J3GNN3B
* `asin` - ID of the product, e.g. 0000013714
* `reviewerName` - name of the reviewer
* `helpful` - helpfulness rating of the review, e.g. 2/3
* `reviewText` - text of the review
* `overall` - rating of the product
* `summary` - summary of the review
* `unixReviewTime` - time of the review (unix time)
* `reviewTime` - time of the review (raw)

Overall there were very few negative reviews totalling less than 5%.  The majority of reviews were 4 or 5 
stars.  A few models were trained and tested.  XGBClassifier consistently yielded the higher accuracy up to
89.3%.