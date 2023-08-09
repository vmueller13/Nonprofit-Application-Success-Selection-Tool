# Module 21 Challenge: Deep Learning

<ins>Project Overview</ins>
------
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The steps to this project are to preprocess the dataset and prepare it for step two which will compile, train and evaluate the neural network model.


<ins>Processes and Technologies</ins>
------

**Step 1: Preproccess the Data**


After opening the notebook in Google Colab, clean up the data by dropping uncessesary columns and determining the unique values for each column and choose a cutoff point for binning. Next, use `pd.get_dummies` to encode categorical variables, split the data into Split the preprocessed data into a features array, `X`, and a target array, `y`. Use these arrays and the train_test_split function to split the data into training and testing datasets. Scale the training and testing features datasets by creating a `StandardScaler` instance, fitting it to the training data, then using the `transform` function.

**Step 2: Compile, Train and Evaluate the Model**


Using your knowledge of TensorFlow, you’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. You’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once you’ve completed that step, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

* Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.
* Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.
* Create the first hidden layer and choose an appropriate activation function.
* If necessary, add a second hidden layer with an appropriate activation function.
* Create an output layer with an appropriate activation function.
* Check the structure of the model.
* Compile and train the model.
* Create a callback that saves the model's weights every five epochs.
* Evaluate the model using the test data to determine the loss and accuracy.
* Save and export your results to an HDF5 file. Name the file `AlphabetSoupCharity.h5`.

**Step 3: Optimize the Model**

Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

Use any or all of the following methods to optimize your model:

* Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
* Dropping more or fewer columns.
* Creating more bins for rare occurrences in columns.
* Increasing or decreasing the number of values for each bin.
* Add more neurons to a hidden layer.
* Add more hidden layers.
* Use different activation functions for the hidden layers.
* Add or reduce the number of epochs to the training regimen.

<ins>Challenges</ins>
------


The biggest challenge I faced in this project was to optimize the data for more than 75% accuracy. I ran ten optimization tests where I changed the coumns that were dropped, increased and decreased the number of epochs and added a third hidden layer. None of these tests were successful.
