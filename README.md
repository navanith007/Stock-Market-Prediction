# Stock Market Prediction using both stock data and the news data
### Author: Rayavarapu Navanith

## 1. Project overview
* Stock market Prediction offers great profit avenues and is a fundamental stimulus for most researchers in this area. 
* This github repo researched the both fundamental analysis and technical analysis on the stock data to predict the market movement. Technical Analysis refers to using the historical stock data to predict the future market movement. Fundamental Analysis refers to using the financial news related to the stock market to predict the future market movement.
* Engineered features from the text data and stock data to build ML and Deep Learning Models. 
* The project idea is to find whether the sellers are in the control or buyers are in the control of the stock given the past prices and the technical news.
* Researched with different datasets and conculded what to do and what not do in the work of stock market prediction.
* knn, svm and deep learning models are used to predict the class label.

## 2. Code and Resources used
**python**: version 3.7  
**packages**: pandas, numpy, sklearn, matplotlib, TensorFlow, NLTK.  
**Research papers Referred**:
  * (https://www.researchgate.net/publication/318298991_Predicting_Stock_Market_Behavior_using_Data_Mining_Technique_and_News_Sentiment_Analysis)
  * (http://ieeexplore.ieee.org/document/7996306/)
  * (https://www.intechopen.com/online-first/recent-advances-in-stock-market-prediction-using-text-mining-a-survey)  
  
**Github code referred**:
  * (https://github.com/EmielStoelinga/CCMLWI)


## 3. Data sets used  
There are two different data sets are used in this analysis.  
**First data set**: (https://www.kaggle.com/aaron7sun/stocknews) This dataset contains the Dow Jones industrial Average stock data and the Top25 Reddit news published.  
**Second data set**: (https://www.kaggle.com/uciml/news-aggregator-dataset) This dataset contains the technical news, business news of various top companies in the period of five months. And the Microsoft stock data (https://finance.yahoo.com/quote/MSFT/history?p=MSFT).  

## 4. Data pre-processing  
* Stock data contains continuous features which depends on the time. But, my model doesn't depend on the time. So, to get the discrete features fromt this dataset. I generated five features from the stock dataset.  
    1. **move_close**: It's the movement of today's close price compared to yesterday's closing price. This feature values are either **increased** or **decreased**.  
    2. **move_open**: It's the movement of today's open price compared to yesterday's open price. This feature values are either **increased** or **decreased**.  
    3. **move_high**: It's the movement of today's high price compared to yesterday's high price. This feature values are either **increased** or **decreased**.  
    4. **move_low**:  It's the movement of today's low price compared to yesterday's low price. This feature values are either **increased** or **decreased**.  
    5. **move_close_open**: It's the movement of today's close price compared to today's opening price. This is the target feature. This feature values are either **Buyers are control** or **sellers or control**. 

* In both datasets the news data is messy, The news data set is cleaned by removing stopwords.  

* the cleaned dataset looks like this.  

 
 

## Notebooks folder
In the notebooks folder, the stock_matrket_prediction.ipynb file contains the total analysis and the prediction on these two datasets are there. Final.ipynb contains the prediction using the best model.

You can look more about the analysis in this medium article (https://medium.com/@navaneethrayavarapu/stock-market-prediction-using-artificial-intelligence-ai-d5f4e86055be).
