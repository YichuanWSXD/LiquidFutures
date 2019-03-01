# LiquidFutures
*This repository is build for an interview project*

## Instruction
*Strategy.ipynb* - code in jupyter notebook

*Strategy.pdf* - pdf version of the code and results

*Returns.png* - Visualization on Performance


## Dependent variable: Previous T-bill monthly return, Libor (3 month) and S&P 500 index
Rational: Libor and S&P 500 can well expain the macroeconomic factor, while the past performance of T-bill is a technical factor. 
## Model: Four different machine learning models
Logistic regression, support vector regression, support vector classification and random forest.
Three of those are simple classfication tools and I want to test whether they work in this case.

## Period:
2001-2006: train set for machine learning model
2007-2010: test set for machine learning model
2011-present: test set for backtest

## Visualization
![alt text](https://github.com/YichuanWSXD/LiquidFutures/blob/master/Returns.png)


It illustrate that the models do well in the train set period, but the performance fades off quickly into the test. Especially after 2008 financial crisis, all models fail to predict the market, and this may imply a change in the financial environment after the crisis or simply a disappointing performance in the long term.

## Reflection
Since overfitting is a huge issue in real-world investing, I try to show how to improve the real-world performance by using multiple validation set.
The performance is disappointing, in my opinion, mostly due to the poor choice of dependent variables. I believe the performance would improve if I put more effort into feature selection. Another reason is that I didn't optimaze the parameters.

The difficulty in the project is the objectives of the project, which are maximized returns and sortino ratio, and minimized drawdowns. I am still trying to figure out how to include those objectives into the model. It may require to build a comprehensive model that computes those metrics during training, and surely the training process would take much longer time.
Another difficult is the mid-frequency strategy. It takes some time to figure out how to use the daily date as the dependent variable to form a mid-frequency strategy.

Neural-network and deep learning could take more dependent variable (more layers) and improve the performance. Continuing traing the model would improve the performance as well. Learned from class, I know that PCA performs well in the bond market by decomposing the yield curves. However I didn't do those because it requires extra research and may take longer than required.

## Takeaway
I enjoy doing the project and am exicted about the stuff learned during the project. 


