Multiple linear reg:
- since the data need number and state is not -> using dummy var (work as switches)
(beware of the dummy var trap: including vars that can be inferred from other vars will polute the dataset)
- only keep important vars

5 methods of building models:
- all-in
- backward elimination (stepwise)
- forward selection (stepwise)
- bidirectional elimination (stepwise)
- score comparison

Backward elimination:
- select a significance level (eg. SL = 0.05)
- fit the full model with all possible predictors
- while(max(p)>SL):
    + remove the predictor
    + fit model

Forward elimination:
- select a significance level (eg. SL = 0.05)
- fit all simple reg models y~xn, then select the one with lowest P
- while(max(p)<SL):
    + consider predictor with lowest P
    + add to the current one
- move a step back and return the prev model

Bidirectional elimination:
- select a significance level to enter and stay (eg. SLE = SLS = 0.05)
- change = True
- while(change = True):
    + change = False
    + forward add var, change = True
    + backward remove var, change = True

All possible model:
- select a criterion of goodness of fit (eg. Akaike)
- construc all possible reg models: 2^n -1 combinations
- select the one that best fit the criterion

adjusted R^2
- how good the model fit
- since ARS went down in model 4, we choose model 3 as our final
- Akaike is better when it's smaller -> confirm our choice for model 3

Interpreting the result:
- sign of coefficient matter, but not magnitute (changing unit from m to mm will increase the mag 1000x)
- magnitute can be used to quantify the effect per unit
