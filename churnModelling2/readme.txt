geo-demographic

- create dummy vars for geography and gender
- run dependent logit model with variables
- backward ellimination => model 4 is currently the best (due to R^2)

transformation of independent variable:
sqrt(x), x^2, ln(x)

log10 is good for balance, since 1 unit increase -> 10x
Balance/Age is a good measure of how successful a person is
Analysis -> collinearity
=> model 6 is currently the best
multicollinearity is bad for the model => use correlation matrix to illiminate things that > 0.3