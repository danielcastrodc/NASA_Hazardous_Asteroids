# NASA_Hazardous_Asteroids

## ***Goal:*** 
Classify asteroids as hazardous based on the provided data. No target leakeage within the existing feature space.

## ***Initial subject matter understanding:***
Asteroids vary in size from 'minor planets' to 'planetoids'. The larger the asteroids, the more dangerous it is. The closer or faster the asteroids comes to hitting earth, the more dangerous it is.

## ***Initial thoughts on dataset before preprocessing:***
Various numeric values that need to be normalized. 

## ***Approach:***
Please note that after determining the best model via PyCaret. I later redo the work with sci-kit learn to demonstrate my understanding of these techniques. PyCaret is an open source low-code machine learning library that makes it extremely easy to test out popular algorithms to see which are the best. PyCaret will also handle one hot encoding, train and test splits, hyperparameter tuning, cross validation, and more.

## ***Results:***
I recreated the best model that I identified with PyCaret by using Sci-kit learn (sklearn). The resulting recall was approximately 98.6% thereby netting a great score that minimized false negatives. This was nearly equivalent to the 99% recall that was netted in PyCaret with logistic regression.

Please note: When considering performance metrics, a false positive would indicate an asteroid predicted as hazardous when it isn't. A false negative would indicate an asteroid predicted as non-hazardous when it is. Therefore, priority should be given to performance metrics that minimize false negatives (eg. Recall, F1 Score).

## ***Technology used:***
Google Colab, PyCaret, Pandas, Numpy, Seaborn, Sklearn
