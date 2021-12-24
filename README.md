# Neural_Network_Charity_Analysis
## Overview of the project
The purpose of this analysis is to show the knowledge gained through machine learning and neural networks. I used the features in the dataset in more than 34,000 organizations that received funding from Alphabet Soup. Armed with this information, I created a binary classifier that can predict whether applicants will receive funding from Alphabet Soup.
### Results
* Data preprocessing
  * Target variable is the "IS_SUCCESSFUL" column.
  * Variables that are considered to be the features are listed below: 'STATUS', 'ASK_AMT', 'IS_SUCCESSFUL', 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT'. I dropped "USE_CASE_Other","AFFILIATION_Other" columns.
  * "EIN" and "NAME" are variables that are neither targets nor features and were removed from the input data.
* Compiling, Training, and Evaluating the Model
  * Layers and activation functions in AlphabetSoupCharity: two hidden layers (the first with Rectified Linear Unit (ReLU), the second with Sigmoid), output layer (with Sigmoid)
  * Optimize the layers and activation functions in the code: Sigmoid is used for the three hidden layers and the output layer.
  * I cannot reach the target model performance.
  * To increase the models performance I changed the number of layers, increased the epochs and remove colomns.
### Result Images
* 1st round

![image](https://github.com/YutaiLee/Neural_Network_Charity_Analysis/blob/main/images/1st_round.PNG)
* 2nd round

![image](https://github.com/YutaiLee/Neural_Network_Charity_Analysis/blob/main/images/2nd_round.PNG)
* 3rd round

![image](https://github.com/YutaiLee/Neural_Network_Charity_Analysis/blob/main/images/3rd_round.PNG)
* Final round

![image](https://github.com/YutaiLee/Neural_Network_Charity_Analysis/blob/main/images/last_round.PNG)

### Summary
The model has an accuracy score of 53% after optimization. The accuracy of the initial neural network is 68%. This loss of accuracy can be explained by the fact that the model is overfitting. In addition, we can further optimize our neural network to improve accuracy by removing more features or simply adding more data to the data set. Since our accuracy score does not particularly meet the criteria of a neural network, we can use a random forest classifier. This is because random forest has a sufficient number of estimators and tree depths, so it is a robust and accurate model. In addition, the performance of the random forest model is faster than that of the neural network and can avoid data overfitting.
