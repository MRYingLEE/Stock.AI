I have nearly gone through all reinforcement learning based trading repos. I have some findings:

1. Most failed, few may be successfully.

So far, I found the following 2 repos could be practical:

https://github.com/ZhengyaoJiang/PGPortfolio

https://github.com/liangzp/Reinforcement-learning-in-portfolio-management-

But, these 2 are for relative investment. They are for portfolio management, instead of for a single name. 
They adjust weights for different names, instead of make decisions of buy/sell for a name.

This is consitent with my thoughts. The information for absolute buy/sell decision is needed massively. But the information for relative investment (adjust weights) is needed at a reasonable level.

2. Most repos have nothing to do with investment. They just use code to deal with investment data.

As an investment based solution, the code should be reflect the characteriscs of investment.

A good solution should have some investment related components:

  Portfolio: To management the positions and calculate P/L.

  Metrics: To calculate Sharpe ratio and so on. These ratios can be used in the reward function, and also can be used to evaluate the model.
