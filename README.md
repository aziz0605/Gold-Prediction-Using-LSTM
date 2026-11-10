# 🥇 Gold Price Prediction Using LSTM

## 📌 Project Overview

This project focuses on predicting the next day's gold price using Deep Learning techniques, particularly **Bidirectional LSTM (Long Short-Term Memory)**.

The model analyzes historical gold price data along with various economic indicators to forecast future gold prices.

It uses time-series sequence modeling to learn patterns and trends from previous 15 days of data and predict the next day's gold price.

## 🎯 Project Objectives

- Predict next-day gold prices using Deep Learning.
- Analyze historical gold price trends.
- Understand time-series forecasting using LSTM.
- Explore the relationship between gold prices and economic indicators.
- Evaluate prediction performance using regression metrics.
- Visualize actual vs predicted gold prices.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook / Google Colab

## 📊 Dataset Description

The project uses a gold price time-series dataset containing approximately 300 rows.

### Features Used

| Feature | Description |
|---|---|
| Gold_Price | Historical gold price |
| USD/INR | US Dollar to Indian Rupee exchange rate |
| Crude Oil | Crude oil price |
| Silver | Silver price |
| Inflation | Inflation rate |
| Interest Rate | Interest rate |
| Stock Index | Stock market index |

**Target Variable:** Gold_Price (Next-day gold price)

## ⚙️ Project Workflow

1. Import required Python libraries.
2. Upload and load the gold price dataset.
3. Perform data preprocessing.
4. Remove the Date column.
5. Normalize features using MinMaxScaler.
6. Create time-series sequences using the previous 15 days.
7. Split the dataset into 80% training and 20% testing.
8. Build a Bidirectional LSTM model.
9. Train the model using Early Stopping and ReduceLROnPlateau.
10. Predict gold prices.
11. Evaluate the model performance.
12. Predict the next day's gold price.

## 🧠 Deep Learning Model

**Bidirectional LSTM (Long Short-Term Memory)**

The project uses a Bidirectional LSTM architecture with:

- Bidirectional LSTM – 128 units
- Dropout – 0.2
- LSTM – 64 units
- Dropout – 0.2
- LSTM – 32 units
- Dropout – 0.2
- Dense Layer – 16 neurons
- Output Layer – 1 neuron

### Model Optimization

- Optimizer: Adam
- Learning Rate: 0.001
- Loss Function: Mean Squared Error (MSE)
- Batch Size: 16
- Maximum Epochs: 100
- Early Stopping
- ReduceLROnPlateau

## 📈 Model Evaluation

The model performance is evaluated using the following metrics:

- **MAE (Mean Absolute Error):** Measures the average absolute prediction error.
- **RMSE (Root Mean Squared Error):** Measures prediction error while penalizing larger errors.
- **R² Score:** Measures how well the model explains the variation in gold prices.

## 📉 Visualizations

The project includes four visualizations:

1. Training Loss vs Validation Loss.
2. Actual vs Predicted Gold Prices.
3. Actual vs Predicted Price Comparison.
4. Prediction Error Analysis.

## 🔮 Next-Day Gold Price Prediction

The trained model uses the latest 15 days of available data to predict the next day's gold price.

It also calculates:

- Last Known Gold Price
- Predicted Next-Day Gold Price
- Price Difference
- Percentage Change
- Predicted Market Trend (Bullish / Bearish)

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Gold-Price-Prediction-LSTM.git
```

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Run the Notebook

Open `GOLD_PRICE_PREDICTION_USING_LSTM.ipynb` and run all cells.

### 5. Upload Dataset

Upload the required dataset:

`gold_price_lstm_dataset.csv`

Make sure the dataset is available at the path expected by the notebook.

## 📁 Project Structure

```text
Gold-Price-Prediction-LSTM/
│
├── GOLD_PRICE_PREDICTION_USING_LSTM.ipynb
├── gold_price_lstm_dataset.csv
└── README.md
```

## 🔮 Future Enhancements

- Increase dataset size for better model training.
- Experiment with different LSTM architectures.
- Compare LSTM with GRU and other forecasting models.
- Build an interactive web application using Streamlit.
- Integrate real-time gold price data.
- Improve prediction accuracy through hyperparameter tuning.

## ⚠️ Disclaimer

This project is developed for educational and academic purposes only. Predicted gold prices are model estimates and should not be considered financial or investment advice.

## 👨‍💻 Author

**Mohamed Aziz**

Deep Learning Project – Gold Price Prediction Using Bidirectional LSTM.

---

⭐ If you find this project useful, don't forget to star the repository!
