# Backtesting_using_OOP

## Development setup

Tensorflow and Keras frameworks are adopted for the implementation.

> pip install tensorflow

The historical data can be accessed by installing yfinance library (https://pypi.org/project/yfinance/).

> pip install yfinance

Libraries used to create visualizations

> pip install matplotlib
> pip install seaborn

## The Model

With the help of an LSTM network, we previously estimated a model the predictis the future price of BTC for the day after. We created the class Data that downloads the historical data available for BTC and splits the dataset and imports the estimated model mentioned before to obtain the predicted prices fot BTC. We can see below the results of running the model with new data.

<img width="873" alt="Screen Shot 2021-05-02 at 1 48 29 PM" src="https://user-images.githubusercontent.com/34326154/116821299-b73e1f80-ab4f-11eb-8749-076239e69570.png">

## Results

After extracting the predicted prices, we passed onto defining the trading rule. Instead of looking at the actual price predicted we decided to identify as a buying opportunity (1) each time the predicted price is higher than the previous closing price. Otherwise, the trading rule will output the number zero, which indicates the investor should sell. After rulling this loop we plotted the results the investor would have had if he had followed this trading rule.

<img width="857" alt="Screen Shot 2021-05-02 at 1 48 39 PM" src="https://user-images.githubusercontent.com/34326154/116821312-c45b0e80-ab4f-11eb-8f37-b5ba45eade6a.png">


## Articles

- "Python Trading Toolbox: a gentle introduction to backtesting", Stefano Basurto, shorturl.at/bzGO5
- https://www.investopedia.com/articles/trading/05/030205.asp
- https://realpython.com/python3-object-oriented-programming/
- "Time Series Forecasting with LSTMs and Prophet", Maximilian Strauß  https://tinyurl.com/62vbrx3m
- Chapter 6, "Deep Learning with Python",Francois Chollet
- Chapter 15, "Hands-on Machine Learning with Sciki-Learn & TensorFlow", Aurélien Géron, O'Reilly 2019

## Contributing

- Fork this project
- Create your feature branch
- Commit your changes
- Push to the branch
- Create a new Pull Request

