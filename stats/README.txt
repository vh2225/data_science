stats refresher:

variables:
- categorical:
    Nominal (Male/Female/Red/Green ...): names
    Ordinal (small/medium/large/ABC grades): groups
- Numeric:
    Discrete (1,2,3,567): not divisible into smaller unit
    continuous (age/height): inf divisible 

Regression
- linear:
    simple: y = b0 + b1*x (y: dependent var, DV; x: independent var, IV; b1: coef; b0: const)
    multiple: y = b0 + b1*x1 + ... + bn*xn
- logistic
    simple: 
    multiple:
    
Least Square:
- ordinary: a line y^(x) so that sum(y-y^)^2 -> min
- R square:
    SSres = sum(yi-y^)^2
    SStot = sum(yi-yavg)^2
    R^2 = 1 - (SSres/SStot) (0->1 the closer to 1, the better)
- adjusted R square:
    Adj R^2 = 1 - (1-R^2)*(n-1)/(n-p-1) (p: number of regressors; n: sample size)