# House Price Analysis and Prediction

## Table of Contents
- [House Price Analysis and Prediction](#house-price-analysis-and-prediction)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Dataset](#dataset)
    - [Dataset Attributes](#dataset-attributes)
  - [Data Preprocessing](#data-preprocessing)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Modeling](#modeling)
    - [Model Evaluation](#model-evaluation)
  - [Future Price Prediction](#future-price-prediction)
  - [Conclusion](#conclusion)
  - [Requirements](#requirements)
  - [Acknowledgements](#acknowledgements)

## Introduction
This project aims to analyze and predict house prices using various machine learning models. The main objectives include data cleaning, exploratory data analysis, feature engineering, model training, and future price prediction based on hypothetical scenarios.

## Dataset
The dataset contains information about various properties listed on a real estate platform. It includes details on property attributes, location, and pricing.

### Dataset Attributes
- **property_id**: Unique identifier for each property.
- **location_id**: Identifier for the property's location.
- **page_url**: URL link to the property details.
- **property_type**: Type of property (e.g., house, apartment).
- **price**: Price of the property.
- **location**: Specific location of the property (e.g., neighborhood).
- **city**: City where the property is located.
- **province_name**: Name of the province where the property is located.
- **latitude**: Geographic latitude coordinate of the property.
- **longitude**: Geographic longitude coordinate of the property.
- **baths**: Number of bathrooms in the property.
- **area**: Total area size of the property.
- **purpose**: Purpose of the property listing (e.g., sale, rent).
- **bedrooms**: Number of bedrooms in the property.
- **date_added**: Date when the property listing was added.
- **agency**: Real estate agency handling the property (may contain missing values).
- **agent**: Agent responsible for the property (may contain missing values).
- **Area Type**: Type of area measurement (e.g., Marla, Kanal).
- **Area Size**: Size of the area.
- **Area Category**: Category of the area size.

## Data Preprocessing
The data preprocessing steps included:
- Handling missing values and inconsistencies.
- Converting area measurements to a consistent unit (square feet).
- Encoding categorical features for modeling.

## Exploratory Data Analysis
Exploratory data analysis (EDA) was conducted to understand the distribution and relationships in the dataset. Various visualizations and statistical methods were used to gain insights into the data.

## Modeling
Three machine learning models were trained and evaluated:
- **Linear Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

### Model Evaluation
The performance of the models was evaluated using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²). Visualizations of predicted vs. actual prices were also created.

## Future Price Prediction
The trained models were used to predict house prices for hypothetical scenarios with specific characteristics:

```python
hypothetical_data = {
    'area': [3000, 1800, 2200],  # in square feet
    'bedrooms': [5, 3, 4],
    'baths': [4, 2, 3],
    'house_age': [12, 7, 9],
    'latitude': [31.5504, 33.7004, 31.4404],
    'longitude': [74.3707, 73.0604, 73.1004]
}
```


## Conclusion
The project successfully analyzed and predicted house prices using machine learning models. The models provided valuable insights and reasonably accurate predictions, demonstrating the potential for using data science in real estate price forecasting.

## Requirements
- Python 3.6+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn


## Acknowledgements
- Thanks to the [InternnCraft](linkedin.com/company/internncraft) platform for giving this oppertunity.
- Special thanks to the data science community for their valuable resources and support.

---