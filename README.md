# Visualization and Modeling for URL Phishing Attempts
Perform data visualization on Features and Regression Models for predicting when a URL is malicious

**Santos A. Romero**

# Business Problem
Predicting whether a URL is legitimate or a Phishing attempt

# Data
Web Page Phishing Detection Dataset
https://www.kaggle.com/datasets/shashwatwork/web-page-phishing-detection-dataset

# Methods
For Predictive Model
- Checked for duplicates
- Checked for missing values
- Removed URL Column
> The URL column was aready detailed in the rest of the features, making it unnecessary for my predictive model.
For the Visualizations and Presentation
- Checked for duplicates
- Checked for missing values
- Checked for inconsistencies in data.

# Visualizations
I compared multiple features for correlation and patterns with what truly distinguishes
legitimate URLs from malicious URLs, testing assumptions against what was found

![URL Length Multivariate Analysis](https://user-images.githubusercontent.com/112634963/202641593-db969505-4877-4a02-9713-4db262e7ba39.png)

With the above image I set the URL length for the y-axis and compared several features to determine if the assumption that malicious URLs tend to be longer than legitimate ones which proved to be correct.


Other visualizations returned empty graphs. For example, I tested another assumption that malicious URLs try to have the same number of links as authentic URLs, but given their nature most of these hyperlinks would be empty. This assumption was debunked in our data as both legitimate and phishing URLs don't have any empty hyperlinks.


# Model
For the predictive model I recommend a `Random Forest Classifier` model.

As of 11/18/2022:
My reasoning resides on how it performed when compared to a KNN model, as well as a Logistic Regression model on default values. It performed the best out fo the three so I continued fine tuning this model to improve fit and predict time, as well as accuracy. So far, simply tuning a few hyperparameters improved the model while the feature engineering I've tried hasn't improved it.
I currently recommend using my final tuned model of the Random Forest Classifier as the fit and predict times are fast and it had an accuracy score of 96% on the test data, as well as a AUC of 99% with an almost 90 degree Roc Curve.

I will continue to update this section as I try more feature engineering and model tuning:

## Contact information
If there are any more questions or concerns regarding my data, feel free to contact me: saromerg@gmail.com
