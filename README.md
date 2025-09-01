🌊 Flood Prediction with LSTM using Weather Data

This project predicts the likelihood of floods in Mumbai using weather forecast data from the OpenWeatherMap API. It applies an LSTM neural network to analyze temperature, humidity, and rainfall trends and forecast whether a flood is likely within the next 12 hours.
🚀 Features

Fetches real-time 5-day / 3-hour weather forecast from OpenWeatherMap.

Prepares a dataset with rainfall, humidity, and temperature.

Creates a flood label using simple heuristic rules:

High rainfall in the past 12 hours + high humidity → flood risk.

Uses LSTM (Long Short-Term Memory) to model time-series data.

Predicts flood probability for the upcoming 12 hours.

🛠️ Tech Stack

Python 3.9+

Libraries:

numpy, pandas

requests
🔮 Model Details

Sequence length (lookback): 12 (past 36 hours)

Prediction gap: 4 (predict 12 hours ahead)

Architecture:

LSTM(64)

Dense(32, ReLU)

Dense(1, Sigmoid)

scikit-learn

tensorflow / keras
