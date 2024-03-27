# House Price Prediction

## Overview
This project aims to predict house prices using machine learning algorithms. The dataset used for this project is from the -Kc_house_data Sales dataset.

## Dataset
The dataset contains the following columns:
- id: Unique identifier for each house
- date: Date of the sale
- price: Price of the house in USD
- bedrooms: Number of bedrooms in the house
- bathrooms: Number of bathrooms in the house
- sqft_living: Square footage of the living area
- sqft_lot: Square footage of the lot
- floors: Number of floors in the house
- waterfront: Indicates if the house has a waterfront (1 for yes, 0 for no)
- view: Number of views the house has received
- yr_built: Year the house was built
- yr_renovated: Year the house was last renovated
- zipcode: Zip code of the house location
- lat: Latitude coordinate of the house location
- long: Longitude coordinate of the house location
- sqft_living15: Square footage of the living area for the nearest 15 neighbors
- sqft_lot15: Square footage of the lot for the nearest 15 neighbors
   
## Data Preprocessing
- Handled missing values
- Removed duplicates
- Normalized numerical features using StandardScaler

## Models Evaluated
The following regression models were evaluated:
- Linear Regression
- SGD Regressor
- Ridge Regression
- Random Forest Regressor
- AdaBoost Regressor
- Extra Trees Regressor
- Decision Tree Regressor

## Results
The performance of each model was evaluated based on the following metrics:
- Error: Mean Squared Error
- Score: R-squared score
- Train Score: Cross-validated R-squared score on the training set
- Test Score: Cross-validated R-squared score on the test set

Here are the results:

| Model                   | Error           | Score  | Train Score | Test Score |
|-------------------------|-----------------|--------|-------------|------------|
| Linear Regression       | 4.818655e+10    | 0.6415 | 0.6269      | 0.6372     |
| SGD Regressor           | 4.837797e+10    | 0.6401 | 0.6250      | 0.6352     |
| Ridge Regression        | 4.818655e+10    | 0.6415 | 0.6269      | 0.6372     |
| Random Forest Regressor | 1.911153e+10    | 0.8578 | 0.8362      | 0.8344     |
| AdaBoost Regressor      | 9.408283e+10    | 0.3001 | 0.2322      | 0.5362     |
| Extra Trees Regressor   | 2.048825e+10    | 0.8476 | 0.8278      | 0.8329     |
| Decision Tree Regressor | 3.697265e+10    | 0.7249 | 0.6781      | 0.6875     |

## Conclusion
Based on the evaluation, the Random Forest Regressor performed the best with the lowest error and highest score.

## Usage
1. Clone the repository.
2. Install the required dependencies.
3. Run the main script to train and evaluate the models.

## Contributors
- [Samiullah](https://github.com/Sami606713)

