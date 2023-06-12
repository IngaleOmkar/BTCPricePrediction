# Bitcoin Price Prediction with Ensemble Models

This repository contains the code and resources for Bitcoin price prediction using ensemble modeling techniques. The project aims to develop an accurate prediction model by combining the predictions from multiple base models at different levels.

Table of Contents

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The main objective of this project is to predict the price of Bitcoin (BTC-USD) cryptocurrency using ensemble models. The ensemble approach leverages the strengths of different models to improve prediction accuracy. The project explores a two-level ensemble architecture, where level 0 consists of LSTM and GRU models with diverse look-back windows, and level 1 incorporates various models such as LSTM, CNN, Linear regression, SVR, Random forest regressor, and KNN.

## Methodology

The methodology involves the following steps:

- Data collection: Gather historical Bitcoin price data using the yfinance API.
- Ensemble Architecture (Level 0): Implement LSTM and GRU models with different look-back windows to capture diverse temporal patterns in the data.
    - The look-back windows were implemented for 1, 3, 7, 15, 30 and 60 days
- Level 1 Models: Train and integrate various models, including LSTM, CNN, Linear regression, SVR, Random forest regressor, and KNN, to combine the predictions generated at level 0.
- Evaluation: Assess the performance of the ensemble model and individual level 1 models using suitable evaluation metrics such as RMSE and MAE.

## Results

The results indicate the predictive performance of the ensemble model and the individual level 1 models. Detailed analyses and comparisons of the models' strengths and weaknesses are provided. The findings highlight the potential for accurate Ethereum price prediction through the proposed ensemble approach.

## Usage

Clone the repository:
```shell
git clone https://github.com/IngaleOmkar/BTCPricePrediction.git
```

Install the dependencies listed in the requirements.txt file:
```shell
pip install -r requirements.txt
```

## Contributing

Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [GPL-3.0 License](https://choosealicense.com/licenses/gpl-3.0/). You can find the full text of the license in the [LICENSE](LICENSE) file.

