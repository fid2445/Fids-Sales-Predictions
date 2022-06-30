Sales Predictions 

Author: Mike Fiddler

Business problem:
Trying to predict item sales based on a variety of categories.

Data: 
Some of our categories included Item Weight, Item Fat Content (Low fat or regular), Item Type (dairy, meat, etc.), Item Visibility and Outlet Size.

Methods
I began by exploring the data, cleaning out any duplicated rows and checking for missing data.
I decided to remove the column Item Weight for two reasons, firstly that was missing over 1500 values and secondly because weight doesnt detur people from buying the food they want. Next I imputed a value of 'Unknown' for missing values in the column Outlet Size as I do belive that store size could end up impacting sales.
Now it was time to clean the data and I found a column (Item Fat Content) with multiple values that meant the same thing (LF, low fat, reg, Regular) so I changed all the data in that column to be more uniform.
Now with clean unifrom data i was able to start vizualizing the data.
Here is a boxplot showing us the spread of item visibility.
![image](https://user-images.githubusercontent.com/105397828/176762506-15ea1ca2-3ce5-4154-8782-c46871b22ee8.png)
Checking on the relative visibility of items against the number of sales we found this.
![image](https://user-images.githubusercontent.com/105397828/176763012-7b0fc5e2-d7e2-42ac-9570-4fcfc44afe41.png)

Next we moved on to recleaning our data for Machine Learning.
I dropped serverl columns right off the start as i did not need any extra noise in my models.
After imputing, transforming and fitting I was able to create a Linear Regression and a Regression Tree.

After looking over serveral metrics of the data I concluded that my Regression Tree model was the best fit for predicting item sales.
With a RMSE of 1082 and 1057 for my trainging and testing data respectivly i am able to infer that this model works very well with this data.


For further information
For any additional questions, please contact Mike Fiddler fid2445@hotmail.com
