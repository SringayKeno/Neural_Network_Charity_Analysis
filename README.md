# Neural_Network_Charity_Analysis

### Create a deep robust neural network capable of interpreting large complext datasets

Neural networks (also known as artificial neural networks, or ANN) are a set of algorithms that are modeled after the human brain. They are an advanced form of machine learning that recognizes patterns and features in input data and provides a clear quantitative output. In its simplest form, a neural network contains layers of neurons, which perform individual computations. These computations are connected and weighed against one another until the neurons reach the final layer, which returns a numerical result, or an encoded categorical result.

## Overview of Analysis

The nonprofit organization, Alphabet Soup, is a philanthropic foundation dedicated to helping organizations protect the environment, improve peoples well being and unify the world. Alphabet Soup has raised and donated over 10 Billion dollars in the last 20 years. This money has been used in life saving technologies and organizing reforestation groups. 

Beks, a data analyst is in charge of data collection and analyzation for Alphabet Soup. Beks job is to analye the impact of each donation and vet potential recepients. This insures the foundations dollars are being spent effectivatly. Unfortunatly not ever donation Alaphabet Soup makes is impactful. Some organizations receive money only to disappear. 

Senior leadership at Alaphabet Soup has asked Beks to predict which organizations are worth donating too and which are high risk. Alphabet Soup's leadership has asked Bek and her analytics team to produce a mathmatical data driven solution that can do this accurately. Beks has decided this problem is to complex for statistical and machine learning models she has used in the past. Instead Beks will design and train a deep learning neural network. This model will evalutate all types of input data and produce a clear decision making result. 

I will assist Beks in learning about neural networks and how to design and train these models using the Python tensorflow library. I will rely on my past statistics and machine learning experience to help test and opptimize the our models.

With knowledge of machine learning and neural networks, I will use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.


## Results

### Data Preprocessing

* What variable(s) are considered the target(s) for your model?
The target variable of a dataset is the feature of a dataset about which you want to gain a deeper understanding. A supervised machine learning algorithm uses historical data to learn patterns and uncover relationships between other features of your dataset and the target. The target in our dataset was "Is Successful". THe successful target denoted campaigns where alphabet Soup donated where monies were deemed as effectively used.

* What variable(s) are considered to be the features for your model?
Features are nothing but the independent variables in machine learning models. The features in this model are show in image below

<img width="224" alt="Screenshot (440)" src="https://user-images.githubusercontent.com/102890151/184015878-d4e0e107-b27a-470e-ae12-c0963c5efde5.png">

* What variable(s) are neither targets nor features, and should be removed from the input data?
During first model and several attempts at optimiation I eliminated the columns 'Name and 'Ein'. Later in furth optimization attempts I added the 'Name' column back to the dataframe.

elimiated 'EIN' column shown below 

<img width="348" alt="Screenshot (441)" src="https://user-images.githubusercontent.com/102890151/184016509-ef163468-fb91-4534-9768-91b78178dd8d.png">

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?


* Were you able to achieve the target model performance? Yes. In order to do so I didn't remove the 'Names' column as I had done in with previous iterations of this model. I used the 'Name column to separate the organizations into yet another bucket.
Once this was done I was able to rerun the model and achieve the > 75 threshold. Accuracy below

<img width="601" alt="Screenshot (442)" src="https://user-images.githubusercontent.com/102890151/184026546-efe48eea-3fef-4753-be40-b915a9ab939d.png">


* What steps did you take to try and increase model performance?

I did the following for optimazation with this model;
1- Creating more bins for rare occurrences in columns
2- Increasing or decreasing the number of values for each bin
3- Adding more neurons to a hidden layer
4- Adding more hidden layers

## Summary

Summarize the overall results of the deep learning model. Include a recommendation 
for how a different model could solve this classification problem, and explain your recommendation.
