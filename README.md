# Using-Word-Frequencies-for-Predicting-Integrative-Complexity-Scores
American presidential speeches have been ranked in terms of integrative complexity (IC), their score for having more than one viewpoint. IC scores will range from 0-4, 4 being aware of many viewpoints. 148 records have been supplied with the most occurring word rates, with corresponding IC scores to match each speech. Each IC score will be attempted to be predicted using word rates from the 148 speeches, using both classification and regression models. 

The goal is not to produce the best accuracies on this given data set, but given any new data set to be able
to confidently predict the IC score. Overfitting to specificities of the training data set is tempting, but will
not yield accurate future test results. Useful words most correlated to the IC score will be determined and
used as attributes, using univariate attribute selection. Certain “structure words” that could objectively
be placed in either a minimum or maximum IC score speech should be removed as attributes to be used
as predictive to generalize future predictions.

The all 3000 words data set will create overfitting models. All measures and insights will be taken to avoid
complex overfitting models, while still producing reasonably improved accuracy results from the original
3000-word data set. Results will be compared using the 3000-word data set and the useful word data set,
to see if the attribution selection process will aid in prediction accuracy. 
