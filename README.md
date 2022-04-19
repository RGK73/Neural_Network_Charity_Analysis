# Neural_Network_Charity_Analysis

Neural Networks and Deep Learning Models , Machine Learning classification, TensorFlow, Deep Neural Networks.

### Overview of the analysis:

- Compare the differences between the traditional machine learning classification and regression models and the neural network models.
- Describe the perceptron model and its components.
- Implement neural network models using TensorFlow.
- Explain how different neural network structures change algorithm performance.
- Preprocess and construct datasets for neural network models.
- Compare the differences between neural network models and deep neural networks.
- Implement deep neural network models using TensorFlow.
- Save trained TensorFlow models for later use.

The purpose of this analysis:
A foundation, Alphabet Soup, wants to predict where to make investments. The goal is to use machine learning and neural networks to apply features on a provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The initial file has 34,000 organizations and a number of columns that capture metadata about each organization from past successful fundings.

Results:

Data Preprocessing:

What variable(s) are considered the target(s) for your model?
Checking to see if the target is marked as successful in the DataFrame, indicating that it has been successfully funded by AlphabetSoup.

What variable(s) are considered to be the features for your model?
The IS_SUCCESSFUL column is the feature chosen for this dataset.

What variable(s) are neither targets nor features, and should be removed from the input data?
The EIN and NAME columns will not increase the accuracy of the model and can be removed to improve code efficiency.

Compiling, Training, and Evaluating the Model:

How many neurons, layers, and activation functions did you select for your neural network model, and why?

![Alt_text]()

![Alt_text]()

Were you able to achieve the target model performance?
The target was 75% and we could achieve 74.16%.

![Alt_text]()

What steps did you take to try and increase model performance?
We tried more hidden layers and increased epochs to 100 to increase model performance.Columns were reviewed and the STATUS and SPECIAL_CONSIDERATIONS columns were dropped as well as increasing the number of neurons and layers. Other activations were tried such as tanh.Linear activation produced the worst accuracy, around 28%. The relu activation at the early layers , tanh activation in the middle and sigmoid activation at the latter layers gave the best results.

Summary: 

The relu, tanh and sigmoid activations yielded a 74.12% accuracy, which is the best the model could produce using various number of neurons and layers. The next step should be to try the random forest classifier as it is less influenced by outliers.
