# unit-14_Deep_Learning

#### For this homework I created 2 notebooks to see which between fear & greed index and closing price is best reference the for price predictions.
##### Those are all of the steps:

* Prepared the data joining together Historical prices and Fear & Greed scores.
* Used the window data function to chunk the data up with a rolling window of Xt-n to predict Xt and getting in return a numpy array of X any y.
* Setted the window size and target for our prediction.
* Splitted the data (70% training, 30% testing).
* Used MinMaxScaler to scale the data and then fit.
* Reshaped the features for the model.
* Builded the LSTM model setting the number of units to 30 and dropout to 0.6.
* Compiled the model using "Adam" optimizer.
* Printed the model summary.
* Trained the model using 10 epochs and batch size 1.
* Evaluated the test and made predictions.
* Created a dataframe with predicted and real prices then plotted it.

#### Results

There are no doubts about which model performs better, the model that uses closing prices as feature column shows a much lower loss from the evaluation result. 
I tested both models with different windows sizes between 1 and 10 and smaller windows seems to give the best results.
Also over time the the closing price model tracks the values better compared to FnG.
