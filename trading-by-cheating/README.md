
# Why I tried to trade by cheating?
I have nearly gone through all reinforcement learning based trading repos in Github. And few have positive results.

So I am thinking to use a new method to use mechine learning to assist trading. 

Firstly I use the future 20 days price data to decide an optimal strategy (LONG, NETUAL, SHORT) for today. This is a kind of cheating. BTW, I have taken the transaction cost into consideration.

Secondly I use the past 20 days price data to predict the optimal strategy, instead of the forethcoming price, which is usually done by existing models.

In other words, I turn the trading decision problem into a multiclass classification problem.

# The cheating is helpful to the performance, but not always



# The multiclass multification by deep learning and XGBoost failed

At the beginning, I wondered I would meet overfitting.

To my surprise, the accuracy is always below 50% for 2 kinds of models.

Maybe it is because the state (only 20 past prices, actually 20 past returns) is not enough to make a decision on trading.

# All related files have been put in this folder

# The excel files are for pre-processing 

# The notebook is for multi-classification

