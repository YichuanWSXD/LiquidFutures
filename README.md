# LiquidFutures
*This repository is build for an interview project*

## Instruction
*Strategy.ipynb* - code in jupyter notebook

*Strategy.pdf* - pdf version of the code and results

*Returns.png* - Visualization on Performance


## Dependent variable: Previous T-bill growth, Libor (3 month) and S&P 500 index
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
It shows that the model does well in the train set period, but performance fades off.

## Reflection
Since overfitting is a huge issue in real world investing, I try to show how to improve the real-world performance by using multiple validation set.
The performance is disappointing, in my opinion, due to the poor choice of dependent variables. I believe the performance would improve if I put more time on feature selection. Another reason is that I could've put more time into optimazation.

The difficulty is that the objectives of the project is maximize returns and sortino ratio while minimize drawdowns. I am still trying to figure out how to include those numbers into the model. It may require to build a comprehensive model that computes those metrics during training, and surely the training process would take a long time.
Another difficult is the mid-frequency strategy. I think it takes some time to figure out how to use the daily date as the training set to form a mid-frequency strategy.

Neural-network and deep learning could take more dependent variable (more layers) and improve the performance. Continuing traing the model would improve the performance as well. Learned from class, I know that PCA performs well in the bond market by decomposing the yield curves. However I didn't do those because it requires extra research and may take longer than required.

## Takeaway
I enjoy doing the project and am exicted about the stuff learned during the project. 


