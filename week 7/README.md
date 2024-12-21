## Read Me for Week 3. Regressions
Learning R:
- changing values of the tail and head 
- changing how to see the matrix of dummies, realized (x, number) gives you that number of rows
- I realized I was having problems to install packages with R (new device) because I was opening the app from Git instead of installing it locally when opening the R in my device. Before it did not happen because of the folder in which I installed Git and R manually.
- Put what the function parts do (noted with #)
- ; to code more things in one line
- You can work uploading two datasets and just calling them!! Oj and email both stay in my data environment and I can just call them when I need them. 
- Hovering the mouse on top of the formulas shows a picture of the formulas


R and Content: 
-  I got the Warning message: glm.fit: fitted probabilities numerically 0 or 1 occurred --> this could be many outliars or too many variables




Going through the content slowly to solve some mind fogs: 
- We are working with GLM not LM therefore when regressing like this, R reports df, null deviance, residual deviance and AIC.This made me focus more on the differences between the kinds of regressions.  
- GLM -->link functions to allow for non-linear relationships, relate predictors to response, allows different error distributions, uses makimum likelihood estimation.
- LM--> normal distribution of errors, Uses least squares method for estimation. (what we did before)
- mybrand was were we stored the releveled variable! you can change this in r to change who you compare to (dummy part)
- exp(coef) tells you how the odds change when the predictor increases by one unit.
- 1/exp(coef) shows how the odds change when the predictor decreases by one unit.
- residual deviance of the model--> how far model is from the data. 
- null deviance --> deviance from null model (only intercept), how well the simplest model fits. 