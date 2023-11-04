# Housing Price Predictor

This project is a machine learning model designed to predict housing prices based on a dataset of California housing information. The dataset includes features like geographical coordinates, total rooms, population, household income, proximity to the ocean, and more.

## Dataset

The dataset contains 20640 entries with 10 attributes each. After cleaning, it comes down to 20433 non-null entries. The attributes are as follows:

- `longitude`: A float representing the longitude of the location of the house.
- `latitude`: A float representing the latitude of the location of the house.
- `housing_median_age`: A float indicating the median age of a house within a block.
- `total_rooms`: A float indicating the total number of rooms in a house.
- `total_bedrooms`: A float representing the total number of bedrooms in a house.
- `population`: A float representing the population in the area.
- `households`: A float indicating the number of households.
- `median_income`: A float representing the median income of the households in the area.
- `median_house_value`: A float representing the median house value for households within a block.
- `ocean_proximity`: A categorical variable indicating the house's proximity to the ocean.

## Preprocessing

The dataset preprocessing includes:

- Handling missing values by dropping any rows with null entries.
- Splitting the dataset into training and test sets.
- Applying feature engineering by converting certain features to logarithmic scale for better distribution and normalization.
- Creating dummy variables for the categorical variable `ocean_proximity`.
- Adding new features such as `bedroom_ratio` and `household_rooms` based on existing features.

## Exploratory Data Analysis (EDA)

Several exploratory data analyses were performed on the training dataset:

- Histograms of all the features to understand the distributions.
- Heatmap of correlation matrix to understand the relationships between different features.
- Scatter plot for geographical data colored by median house value.

## Getting Started

### Prerequisites

Before running the model, ensure you have the following packages installed:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install these packages using `pip`:

```sh
pip install pandas numpy matplotlib seaborn scikit-learn

Installation
Clone the repository to your local machine:

git clone https://github.com/your-username/housing-price-predictor.git

Navigate to the cloned directory:

cd housing-price-predictor

Usage
Run the Jupyter Notebook or Python script provided to train and test the model:

python housing_price_predictor.py

Or open the Jupyter Notebook if provided:

jupyter notebook housing_price_predictor.ipynb
