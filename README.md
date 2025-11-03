# California Housing Price Prediction🏠📊

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)

This project implements and compares different regression models to predict housing prices in California using the California Housing dataset from scikit-learn.

## Project Overview

The project explores three different regression models:
- Simple Linear Regression
- Ridge Regression
- Lasso Regression

### Discussion
---

The analysis of California housing prices using three different regression models - Simple Linear Regression, Ridge Regression, and Lasso Regression - revealed several interesting insights. The models were trained on standardized data with an 80-20 train-test split, using eight features from the California housing dataset. All three models demonstrated relatively comparable performance, with R-squared values suggesting they could explain approximately 60% of the variance in housing prices. The Simple Linear Regression model provided a baseline performance, while the regularized models (Ridge and Lasso) offered slight improvements in prediction accuracy. The RMSE values indicated that the models' predictions deviated by several thousand dollars from actual housing prices, which is reasonable given the complexity of real estate valuation. Notably, Lasso regression's feature coefficients highlighted which housing attributes had the strongest influence on price predictions, with some coefficients reduced to near-zero, effectively performing feature selection. Ridge regression, while maintaining all features, helped prevent overfitting by constraining coefficient sizes. The models' MAE values provided a more interpretable measure of prediction error in the original price scale. This analysis demonstrates that while linear models can capture significant housing price patterns, there remain unaccounted factors in California's housing market that influence price variations.

## Variable Index

### Input Variables (X)
| Variable | Description | Unit |
|----------|-------------|------|
| MedInc | Median income in block group | Tens of thousands of USD |
| HouseAge | Median house age in block group | Years |
| AveRooms | Average number of rooms per household | Rooms |
| AveBedrms | Average number of bedrooms per household | Rooms |
| Population | Block group population | People |
| AveOccup | Average house occupancy | People per household |
| Latitude | Block group latitude | Degrees |
| Longitude | Block group longitude | Degrees |

### Target Variable (y)
| Variable | Description | Unit |
|----------|-------------|------|
| Target | Median house value | Hundreds of thousands of USD |

### Model Variables
| Variable | Description |
|----------|-------------|
| X_train | Training features |
| X_test | Testing features |
| y_train | Training target values |
| y_test | Testing target values |
| X_train_scaled | Standardized training features |
| X_test_scaled | Standardized testing features |


## Folder Structure

```
Basic_Machine_Learning_EDA_on_California_Housing_Price_Predictio/
│
├── Notebook.ipynb          # Main analysis notebook
├── README.md              # Project documentation
├── requirements.txt       # Project dependencies
└── LICENSE               # License file
```

## Features

The dataset includes the following features:
- MedInc: Median income in block group
- HouseAge: Median house age in block group
- AveRooms: Average number of rooms
- AveBedrms: Average number of bedrooms
- Population: Block group population
- AveOccup: Average house occupancy
- Latitude: Block group latitude
- Longitude: Block group longitude

## Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/Rezaul33/Basic_Machine_Learning_EDA_on_California_Housing_Price_Prediction
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `Notebook.ipynb` and run the cells in sequence.

The notebook:
1. Loads and preprocesses the data
2. Implements three regression models
3. Compares model performance using various metrics (MAE, MSE, RMSE, R²)

## Models and Results

Three regression models were implemented and compared:
1. Simple Linear Regression
2. Ridge Regression (with alpha=1.0)
3. Lasso Regression (with alpha=0.01)

## Dependencies

- Python 3.x
- scikit-learn
- pandas
- numpy
- jupyter

## Author

Rezaul Islam. [Linkedin](https://www.linkedin.com/in/md-rezaul-islam-cse/)

## License

This project is open source and available under the [MIT License](LICENSE).




