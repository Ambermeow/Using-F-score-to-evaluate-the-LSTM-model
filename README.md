# Using-F-score-to-evaluate-the-LSTM-model
It seems that one can plot the beautiful predicting curves in lookback testing using LSTM. However, the most important thing for individual clients, is whether the price would move up or down, instead of the absolute deviation. So, here I used F score to evaluate that performance of LSTM in lookback testing. 

The LSTM part is based on : https://www.kaggle.com/benjibb/lstm-stock-prediction-20170507.

Here the epochs=20, windows=7, and batch_size=32. Changing the epochs=400 would make the predicting plot more "beautiful", yet the F score would only be lifted to 0.59.

You can also test many other LSTM models published in "Kernals".

For example, the F score of the model published by TusharGupta : https://www.kaggle.com/bunny01/predict-stock-price-of-apple-inc-with-lstm, is 0.48, with batch_size=32, windows=7, and epochs=900. (F=0.52 with batch_size=512 and windows=22)
