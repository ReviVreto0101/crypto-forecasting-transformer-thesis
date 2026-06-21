# crypto-forecasting-transformer-thesis
Reproducibility package for the Master thesis on multivariate cryptocurrency forecasting using ARIMA, LSTM and TFT_LOG_RETURN.

# Revi Vreto – Diploma Reproducibility Package

This repository contains the reproducibility materials for the Master thesis:

**“Përdorimi i modeleve me arkitekturë Transformer për parashikimin multivariat të monedhave kripto.”**

**“Using Transformer-Based Models for Multivariate Cryptocurrency Forecasting.”**

## Repository contents

* `FINAL_Revi_Diploma_Models_ARIMA_LSTM_TFT.ipynb` – final notebook with preprocessing, ARIMA, LSTM, TFT_LOG_RETURN, metrics and statistical tests.
* `crypto_dataset_full.csv` – final multivariate dataset.
* `crypto_train_2019_2022.csv` – training split.
* `crypto_validation_2023_H1.csv` – validation split.
* `crypto_test_2023_H2_2024.csv` – test split.
* `final_metrics_arima_lstm_tft.csv` – final evaluation metrics.
* `combined_predictions_arima_lstm_tft.csv` – combined predictions of the models.
* `statistical_tests_clean_summary.csv` – clean summary of statistical tests.
* `statistical_tests_dm_wilcoxon.csv` – full Diebold-Mariano and Wilcoxon results.

## Models

The empirical analysis compares three models:

* ARIMA
* LSTM
* TFT_LOG_RETURN

TFT_LOG_RETURN forecasts cryptocurrency log-returns and reconstructs predicted prices for final evaluation.

## Forecasting horizons

The models are evaluated for three forecasting horizons:

* H=1
* H=7
* H=30

## Evaluation metrics

The evaluation uses:

* MAE
* RMSE
* MAPE
* R²
* Directional Accuracy
* Diebold-Mariano test
* Wilcoxon Signed-Rank test

## How to reproduce the experiment

1. Open `FINAL_Revi_Diploma_Models_ARIMA_LSTM_TFT.ipynb` in Google Colab or Jupyter Notebook.
2. Upload or keep all CSV files in the same working directory as the notebook.
3. Run the notebook cells from top to bottom.
4. The notebook loads the dataset, applies preprocessing, creates the Train/Validation/Test splits, trains or evaluates the models, calculates the final metrics and produces the statistical test results.
5. The final outputs can be compared with the CSV files included in this repository.
