Task1: Estimate whether a particular item would be reviewed

In this task, I combine two ways to predict whether customer will buy the products.

First, I rank items by popularity in the data. If a test item ranks among the specific percent of most popular items, return True else return False. 

Second, I define a function to compute the Jaccard similarity between item’s categories that the customer has previously bought and a test item’s categories. I save these similarities into a list. If the length of the list equal to one and the value is larger than one specific value, return True else return False. If the length of the list larger than one and the sum of tow maximum similarities is bigger than a specific value, return True else return False. 

During the prediction progress, I combine the popularity and Jaccard similarity classification. If a test item is among the specific percent of most popular items in the data or the function I defined return True, I write 1 in the prediction dataset else write 0. After testing, I verify these specific values to predict whether customer will buy item in the test dataset.
