# Deep-learning-challenge

### Overview
Alphabet Soup, a nonprofit foundation, seeks to optimize its funding allocation process by identifying the most promising applicants for successful ventures. With the assistance of a data scientist knowledgeable in machine learning and neural networks, they plan to leverage a dataset comprising information on over 34,000 previously funded organizations. The project involves using this dataset to create a predictive model that acts as a binary classifier. This model will assess and predict the probability of success for future applicants if they were to receive funding from Alphabet Soup. The ultimate objective is to enhance the foundation's decision-making process in selecting potential funding recipients, improving the likelihood of supporting successful endeavors.

### Aim 
The aim of the project is to develop a machine learning-based tool, specifically a binary classifier using neural networks, to predict the success of funding applicants for the nonprofit foundation Alphabet Soup. The goal is to effectively select potential funding recipients by analyzing a dataset of over 34,000 previously funded organizations to determine their likelihood of success based on certain features.

### Results

#### Step 1: Preprocessing the data

* Feature columns that capture metadata about each organization, such as:
	* APPLICATION_TYPE—Alphabet Soup application type
	* AFFILIATION—Affiliated sector of industry
	* CLASSIFICATION—Government organization classification
	* USE_CASE—Use case for funding
	* ORGANIZATION—Organization type
	* STATUS—Active status
	* INCOME_AMT—Income classification
	* SPECIAL_CONSIDERATIONS—Special considerations for application
	* ASK_AMT—Funding amount requested

* Target column:
	* IS_SUCCESSFUL—Was the money used effectively

![Screenshot 2023-11-01 at 10 40 07 PM](https://github.com/ShipraGupta16/deep-learning-challenge/assets/25715747/65a43900-3ea7-4a3a-8954-e10c964063c3)


* For columns that have more than 10 unique values, determine the number of data points for each unique value.

* Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

* The train_test_split function was used to create a split into the data into training and testing datasets.
  
![Screenshot 2023-11-01 at 10 41 56 PM](https://github.com/ShipraGupta16/deep-learning-challenge/assets/25715747/22e2b6bd-2f8b-441c-8631-7e190359c42d)


#### Step 2: Compile, Train, and Evaluate the Model

After designing the network, the next steps involve compiling, training, and evaluating the model. This evaluation includes calculating the model's loss and accuracy to ensure its predictive performance in determining the success of Alphabet Soup-funded organizations. Total 3 attempts were made using machine learning and neural networks to achieve the target model performance at predictive accuracy > 75%. The results are:

Attempt 1
![Attempt1 2023-11-01 at 10 42 25 PM](https://github.com/ShipraGupta16/deep-learning-challenge/assets/25715747/2f1506a3-9122-487e-a274-b974552df901)

* Accuracy score is 67.7%
* No of hidden layers = 2
* First layer: 90 neurons : activation function = ‘relu’
* Second layer: 30 neurons : activation function = ‘relu’
* Output layer: activation function = ‘sigmoid’
* epochs = 100

Attempt 2
![Attempt2 2023-11-01 at 10 43 09 PM](https://github.com/ShipraGupta16/deep-learning-challenge/assets/25715747/90d37197-b064-4377-a256-1b0db7449aa5)

* Accuracy score is 60.2%
* No of hidden layers = 3
* First layer: 100 neurons : activation function = ‘relu’
* Second layer: 35 neurons : activation function = ‘relu’
* Third layer: 25 neurons : activation function = ‘tanh’
* Output layer: activation function = ‘sigmoid’
* epochs = 100

Attempt 3
![Attempt3 2023-11-01 at 10 43 20 PM](https://github.com/ShipraGupta16/deep-learning-challenge/assets/25715747/e12b06cf-f59d-4682-b3b1-f09830a2dc0a)

* Accuracy score is 80.7%
* No of hidden layers = 3
* First layer: 10 neurons : activation function = ‘relu’
* Second layer: 50 neurons : activation function = ‘relu’
* Third layer: 30 neurons : activation function = ‘tanh’
* Output layer: activation function = ‘sigmoid’
* epochs = 100
  
### Summary
After all the attempts were made, the model was able to achieve a target performance of 80% on full data. It could be better performance and hence we should explore other methods and better ways to tune the model. 
