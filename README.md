AI project on Multiple disease detection, focused mainly on diabetes detection using CNN model on the dataset. 

Project Process:

Data Loading and Preprocessing:

The dataset is loaded using Pandas from a CSV file (diabetes.csv).
Features are separated from the target variable (Outcome) to prepare the data for modeling.

Data Splitting:

The dataset is divided into training and testing sets to evaluate model performance on unseen data.

Model Building:

1D CNN Model: A Convolutional Neural Network is constructed using the Keras Sequential API, consisting of:
Several convolutional layers (Conv1D) for feature extraction.
Max pooling layers to reduce dimensionality.
Dropout layers for regularization.
Fully connected layers (Dense) for the output.
The model is compiled with the Adam optimizer and binary cross-entropy loss function, suitable for binary classification tasks.

Model Training:

The CNN model is trained on the training dataset using a defined number of epochs and batch size, with validation split to monitor performance on a portion of the training data.

Model Evaluation:

The trained model is evaluated on the testing dataset to determine accuracy and loss using model.evaluate().

Alternative Model - KNN:

A K-Nearest Neighbors (KNN) classifier is also implemented.
Hyperparameter tuning is performed using GridSearchCV to find the optimal number of neighbors (n_neighbors).
The best parameters are printed, and the model is evaluated on the test set, calculating accuracy and log loss.
