# Aviator Odds Prediction Model

## Overview

This project aims to predict betting odds using historical data, including odds values, color codes, and timestamps. The goal is to develop a machine learning model that can accurately forecast future odds based on these features.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Modeling](#modeling)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset consists of three columns:
1. **Odds**: The betting odds in the form of "x.xxxx".
2. **Color**: The RGB color code associated with the odds.
3. **Timestamp**: The time when the odds were recorded.

The data is used to train and evaluate various machine learning models to predict future odds.

## Data Preparation

1. **Data Cleaning**: The 'x' suffix was removed from the odds values, and the color codes were split into individual RGB components.
2. **Feature Engineering**: Additional features were created from the timestamp, such as the hour of the day and day of the week.
3. **Splitting the Data**: The dataset was split into training and testing sets to evaluate the model's performance.

## Modeling

Several machine learning models were explored, including:

- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Support Vector Regressor (SVR)**
- **XGBoost Regressor**

The models were evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## Results

The best-performing model was selected based on the lowest RMSE and MAE values. The final model provides predictions for the odds based on the input features.

## Usage

To use the model:

1. **Clone the Repository**: 
   ```
   git clone https://github.com/yourusername/aviator-odds-prediction.git
   ```

2. **Install Dependencies**:
   ```
   pip install -r requirements.txt
   ```

3. **Run the Prediction Script**:
   ```
   python predict.py --input_data path_to_input_data
   ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue for any improvements or suggestions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.