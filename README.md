# Stock.AI
This project tries to use AI, specifically reinforcement learning, to manage a stock portfolio. The objective is to be practical. So this is not another concept proof of AI in investment.
This project is still at its early days. I will try to complete it in 1 year.

## For performance, not for concept
I am an equity portfolio manager with a few years’ experience. And I have a strong background on quant. I have studied AI for months. I am thinking to apply reinforcement learning to the Financial Markets.
I have checked a few projects, which were initiated by AI experts instead of financial experts. These projects demonstrated AI on financial market, but they are not practical to real financial market.
I will add more color from the financial side to use AI in financial market.

## In Business, why are financial markets hard for AI?
In investment companies, there are a lot of people working to use AI on financial markets.
If someone finds something useful, maybe he will keep it confident and use it to make real money instead to publish it. 
Financial markets are gaming system, everyone gains at cost of others.

## In theory, why are financial markets hard for AI?
In theory, to make money by AI is to challenge EMH (Efficient-market hypothesis) (https://en.wikipedia.org/wiki/Efficient-market_hypothesis ). EMH is the corner stone of modern finance. So that the task is very tough.

## In practice, why are financial markets hard for AI?
1.	Limited data. There is only one copy of data. History doesn’t repeat itself simply.
2.	The information is hard to normalized. The information from the market, the company, the industry and the regulation authorities.
3.	To balance the return and risk. Maybe the predication is 90% accurate. But 1% long tail event can make you bankrupt. In other words, the percent of accuracy is not as important as in other applications.
4.	Regarding microstructure, there are a lot of thing that is hard to digitize, such as shorting, up stick rule and so on.

## How to implement step by step?
1. Don't make a general project for all kinds of finacial products. 
  For me, I will focus on equity (stocks).
  
2. Don't create a tools for all investors. Instead, to solve one problem for 1 kind of investors. For example, for benchmark based portfolio, a tools to solve asset allocation (specifically maybe sector allocation).
  For me, at first I will focus on asset allocation for a benchmark based portfolio.So that I will work on sector level (https://en.wikipedia.org/wiki/Economic_sector) instead of stock level.

3. Don't try to use all kinds of information. The work and cost to use information is very high. 
    Corresponding to EMH (Efficient-market hypothesis), there are 3 Levels of Information:
      Market Data (price, volume and timestamp)
      Other Public Information (such as annoucements from a company, government policies)
      Private Information.
    For a personal project, I will use only market data at first.

## Why reinforcement learning instead of price predicting?
A few projects try to predict price, usually by deep learning. Actually in Github, there is a label #stock-price-prediction. 
But,
1. The accuracy of price predicting is not as important as expected. The accumulated return is the final goal instead of one-time predicting. Actually the accuracy of an experienced investors could be as low as 60%, even lower than 50%. You may be surprised how an investor can gain when his accuracy is below 50%. That is because when he is right he makes a lot of money, when he is wrong he loses a little.
2. The trading cost will make most of your predicting non-profitable. In other words, even when you make a right predictation, you will lose money if you trade following your predication.
3. The portfolio may have some constrains, such as 100% annual turnover restrication. 
4. A portfolio is evaluated by risk adjusted return. Usually Sharpe ration (https://en.wikipedia.org/wiki/Sharpe_ratio) is used. In other words, not only the return, but also the risk, measured by standard deviation (https://en.wikipedia.org/wiki/Standard_deviation)  of the return is considered.

## Why LSTM model?
Most prationer believes the financial history repeats. In other words, the history is meaningful to the future. Technically, the financial price movement is not a Markov Processes (http://www.randomservices.org/random/markov/index.html) .
To use history information, I will use Long short-term memory model(https://en.wikipedia.org/wiki/Long_short-term_memory) as a module of reinforcement learning. 

## What's the architecture?

Not a general algo for investement data, but a investement specific algo.

![Architecture](https://github.com/MRYingLEE/Stock.AI/blob/master/Reinforcement%20Trading.png "Architecture")



I am still in my early days to implement my ideas. If anyone has interest, we may cooperate. You can reach at me by gmail, Mr.Ying.Lee.

