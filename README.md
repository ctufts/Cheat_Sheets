# Cheat_Sheets
Cheat sheets for stats/ML/SP/DM
This repo contains cheat sheets for common statistics, machine learning, signal processing, and data mining terms. 

* Model Description Terms
  * Bias: Error Introduced by approximating real-life problem by using a simple method
  * Variance: The amount the model output will change if the model was trained using a different data
    * Generalized concept:
      * Flexible Methods: higher variance, low bias
        * Examples KNN (k = 1)
      * Inflexible Methods: low variance, high bias
        * Example: Linear regression
  * Parametric: 
    * Model has a function shape and form
    * Model is trained/fit using training data to determine parameter values
      * reduces the problem of training a model down to training a set of parameter values 
      * common approach: ordinary least squares
    * Examples: linear regression
  * Non-Parametric:
    * No assumption about model form is made
    * Example: KNN
* Learning
  * Supervised: Model is trained using historical data to relate the input values to the response
    * Examples: linear regression, svm, decision trees
  * Unsupervised: Try to identify relationship based strictly on input data as no response values are available
    * Examples: clustering (k-means, hierarchical, etc.)
