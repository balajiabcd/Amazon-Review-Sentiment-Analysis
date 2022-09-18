# Amazon-Review-Sentiment-Analysis
Using Sentiment Intensity Analyzer


## Libraries Used:  
  
1. Numpy  
2. Pandas  
3. Matplotlib  
4. Seaborn  
5. SciKit Learn
6. nltk





## Data Set:  
  
You can Download the data set used in this project here at this link.  
"https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews?datasetId=18&sortBy=dateRun&tab=profile"  






## Flatform:  
  
For this project I used Kaggle. Which you can found here: https://www.kaggle.com/  







## About data:  

Dataset consists of 568454 entries. Each review was rated from 1 star to 5 star.  
![Reviews](https://github.com/balajiabcd/Amazon-Review-Sentiment-Analysis/blob/main/Imges-repo/reviews-per-star.png)

In data one column is summary of reveiw, and the next column is review itself. Hence these two columns are merged togather as one full_review column.  
![data](https://github.com/balajiabcd/Amazon-Review-Sentiment-Analysis/blob/main/Imges-repo/data.png)

This full review column is tested for polarity, then the results are stored in a dataframe.  
![polarity_dataframe](https://github.com/balajiabcd/Amazon-Review-Sentiment-Analysis/blob/main/Imges-repo/compound-score-dataframe.png)

Then different columns are created and added this dataframe. One of these columns are "good" which considers 4,5 star reviews as positive and remaining columns as negative.  
![addition](https://github.com/balajiabcd/Amazon-Review-Sentiment-Analysis/blob/main/Imges-repo/review-analysis-columns-addition.png)

Here 3 star reviews are hard to classify as positive or negative, hence the 3 star reviews were removed.    








## Note:  
Here to get the accuracy was calculated in the code itself, rather than using any other library.  







## Model Result:  

Model is trained with the columns that are obtained from polarity dataframe and the newly created column "good".  
After trining and Deploying the different classification models:  
Random Forest model with n_estimators = 10, criterion = "gini", gave best results with 91.59% accuracy of classification.  
![Result](https://github.com/balajiabcd/Amazon-Review-Sentiment-Analysis/blob/main/Imges-repo/Result.png)








