# ml-linear factor models (LFMs)
machine learning methods for LFMs

1. Part 1: Factor model setup and run OLS regression
   there are over 50 factors that have displayed patterns in return, and there is much attention to observing the state of these factors by firms such as MSCI and other providers of analytical services. We have seen the shift into alternative investment categories by university endowments and more recently by large institutional investors including global pension plans and sovereign wealth funds. 
   The study of macro-factors has led to new methods in an asset allocation or Asset Liability Modeling (ALM). Here, we follow the work of Harvard University's endowment and their use of five factors: a) global equity, b) long term U.S. government bonds, c) high yield bonds, d) inflation hedging, and e) currency hedging.
   We will discuss a more systematic approach to estimating the factor loading and employing these loading when forecasting future expected returns for the assets within our portfolio model.
   
  Explaining the asset returns with a five-factor model:
World Equities: MSCI All World market capitalization weighted index.
10 Year US Treasury: Return of 10 year US Treasury Bond
High Yield: BOFA Merrill Lynch Global High Yield Index
Inflation Protection: This is a "style" factor that considers the difference between real and nominal returns, thus balances the need for both. It's the return of the TIPS bond minus the a weighted average of Treasury Bonds.
Currency Protection: This is also an exchange rate factor, capturing the value of the dollar versus a basket of foreign currencies.


   
3. Part 2: Use LASSO regression, and LASSO with cross validation
  Apply a regularized regression with a penalty term to shrink the loadings. This shrinkage is motivated by the Stein result (paradox) since we are estimating the return for more than 2 asset categories. The best penalty value will be determined by cross validation which useses training and validation to estimate the penalty.



4. Part 3: Forecasting 5 factor for multiple assets
