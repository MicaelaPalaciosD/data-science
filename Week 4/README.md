## Read Me for Week 4. Regularization
Learning R:
- The data I uploaded before is still in my R environment!! I can just call on it, do not need to "upload" it everytime
- learned to use cv.gamlr, cross validates for you, you first need to create a sparse matrix
- you can use that to take the lambda with minimum CV error

R and Content: 
- my plots look different than the slides --> randomization -->data points included in each fold may be different
- to allow repetitions we can set a seed. I learned how to set a seed and that it cannot be negative.
- making more folds really takes up more time
- if i make too many folds I get NaN as average of Rsq, this could be because od insufficient data. Also, lowering folds too much makes the negative (Rsq) bigger. 



Going through the content slowly to solve some mind fogs: 
- We are working with binary data! the regression is on binary data. 
- I add some comments on the slides (from notes from class)
- We compute deviance differently depending on whether the model is Gaussian or Binomial.
- Gaussian --> linear
- Binomial --> logistic
- Forward stepwise regression: adds covariates on each step, the deviance increases and flattens. 
- CV picks model with less error, R can show you its coefficients

Random (question "hidden" in the data): 
- Household 4 visited:   atdmt.com          yahoo.com 
       13.54780245        18.50928863 
           msn.com         google.com 
        0.29451744         1.11010421 
           aol.com questionmarket.com 
        0.06796556         3.19438151 
- Household 1:      
atdmt.com      yahoo.com      whenu.com 
     4.0520260     11.8559280      0.0000000 
weatherbug.com        msn.com     google.com 
     0.0000000      0.2501251      6.5282641 