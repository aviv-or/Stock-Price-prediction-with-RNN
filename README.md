# Stock-Price-prediction-with-RNN

> **If you’d like to know more, I've written [an article](https://nicolasracchi.com/projects/stock-prediction) on my blog about this project!**

This web app is built with Flask in Python. It consists of a recurrent neural network application for stock price prediction. It’s been instrumental in learning how to train neural networks in the cloud and use a remotely trained network to produce results.

## Example of prediction output:

<div align=center><img src=nvda_prediction.png></img></div>

## Instructions to run

```bash
git clone https://github.com/nicolas-racchi/Stock-Price-prediction-with-RNN
cd Stock-Price-prediction-with-RNN

# If you're on MacOS/Linux:
export FLASK_APP=app.py

# If you're on Windows:
set FLASK_APP=app.py

# (Optional): Set up your python virtual environment
virtualenv venv

# Install requirements
pip install -r requirements.txt

# Start the app:
flask run
```

## How it works:

- Stock historical data is gathered from the Alpha Vantage API
- An LSTM RNN is trained with your choice of stock symbol, with the API data
- The network is used to predict prices from 1/1/2019 on forward.
- When the prediction has been completed, you'll see a graph of the ACTUAL vs PREDICTED stock price.

### Disclaimer:

_This is not meant to be an investment guide. Take this material as useful for learning about neural networks and stock price prediction._
