# Project Overview

In this project we will predict Bitcoin prices using Historical Data and Sentiment Analysis. Sentiment Analysis is performed on the Wikipeda edits using mwclient which is a lightweight Python client library to the MediaWiki API which provides access to most API functionality. Sentiment Analysis is performed using transformers package. USD/BTC data was obtained through Yahoo Finance API.

# File Overview

* `Prediction.ipynb` - a Jupyter notebook that contains the code to predict Bitcoin prices
* `Sentiment_Analysis.ipynb` - a Jupyter notebook that creates our wikipedia edit dataset.

# Installation

Install the following locally:

* JupyerLab
* Python 3.8+
* Python packages:
    * pandas
    * yfinance
    * scikit-learn
    * xgboost
    * mwclient
    * transformers
    
 # Running

First, run the code in `Sentiment_Analysis.ipynb` to generate a new Wikipedia edits dataset.  The dataset committed in the repo is old, and this will get the edits up to the present day.

Second, run the code in `prediction.ipynb`.  By default, this will load data from an existing `BTC.csv` file.  Removing that code will ensure that it downloads the newest data from Yahoo Finance.
    
