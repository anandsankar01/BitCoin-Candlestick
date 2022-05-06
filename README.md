# BitCoin-Candlestick
This python project will show how to use an API to get live bitcoin data and plot candlestick chart using plotly.

Introduction - 
An API lets two pieces of software talk to each other. Just like a function, you don’t have to know how the API works only its inputs and outputs. An essential type of API is a REST API that allows you to access resources via the internet. In thiscode, I will use a basic REST API.

REST APIs - 
Rest API’s function by sending a request, the request is communicated via HTTP message. The HTTP message usually contains a JSON file. This contains instructions for what operation I would like the service or resource to perform. In a similar manner, API returns a response, via an HTTP message, this response is usually contained within a JSON.

In cryptocurrency a popular method to display the movements of the price of a currency.

In this code, I will be using the CoinGecko API to create one of these candlestick graphs for Bitcoin. We will use the API to get the price data for 30 days with 24 observation per day, 1 per hour. I will find the max, min, open, and close price per day meaning we will have 30 candlesticks and use that to generate the candlestick graph. Although we are using the CoinGecko API we will use a Python client/wrapper for the API called PyCoinGecko. PyCoinGecko will make performing the requests easy and it will deal with the enpoint targeting.
The response we get is in the form of a JSON which includes the price, market caps, and total volumes along with timestamps for each observation. We are focused on the prices so we will select that data.

After doing some data preprocessing, I used plotly to create the Candlestick Chart.
