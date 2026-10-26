# Nairobi--house-deal-finder
Nairobi-house-deal-finder predicts house prices and classifies as a good or bad deal.
#uses 2 ML algorithms in 1 project:

1. *Linear Regression*->predicts the house price in ksh (eg. ksh.230,000)
2. *Logistic Regression*->classifies as good or bad deal (eg. if the price is expensive given the house has few rooms and size, it'll be classified as a bad deal...vice versa)
   
##Data set

Nairobi property prices with columns:
Bedrooms, Bathrooms, House size(m2),land size(acres),location, town property, price.

#source:

Kaggle

#Data Cleaning:

Removed ksh,commas,m2,acres from text.

Handled missing values with df.dropna(),df.fillna().

Changed texts into integers using pd.to_numeric(errors='coerce').

#Models:

Linear Regression:

input-> bedrooms, bathroom, house size

output->price

metrics->r2_score, mean_squared_error

Logistic Rgression:

input->bedrooms,bathroom,house size

output-> 0 or 1

metrics-> accuracy_score

Technologies:

python

pandas

scikit learn
