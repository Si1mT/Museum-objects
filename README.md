# Museum Object types

<p>Predict the <strong>type</strong> of a museum object based on its descriptive variables. Data taken from a Kaggle competition[1].
<br><br>Links:
<br>[1] https://www.kaggle.com/competitions/caps-in-museums-data-part-2/data
</p>
<h2>How to run the code</h2>
Our code uses a DecisionTreeClassifier to train using given data and predict the types of museum objects. To do that, we have cleaned up our training and testing data by removing unnecessary columns, filling any NaN values with an empty string (because we are working on a dataset with a lot of string variables) and then encoding the string data using OneHotEncoder. The encoded data is fed into the DecisionTreeClassifier, which does the rest of the work. Our algorithm has about a 0.77 accuracy for predicting types.
<br>
<br>
<strong>To run the algorithm on new data, you must:</strong> <br> <br>
<strong>1.</strong> Assure the new data is in the correct format (as given in the repository)<br>
<strong>2.</strong> Give the desired file path for the data your wish to predict types of and/or training data<br>
<strong>3.</strong> Assuming the data is in the same format as the original training data then by running all cells the needed changes are made (i.e. deleting columns, encoding, training the data)<br>
<strong>4.</strong> The first DTF algorithm is used to print an estimate to it's accuracy using the training data to split it into both testing/training<br>
<strong>5.</strong> The second DTF algorithm uses the whole training dataset to train and then gives a prediction based on the given testing data<br>
<strong>6.</strong> The predictions are placed into a Pandas DataFrame (id and predicted type) for easy viewing of the results.
