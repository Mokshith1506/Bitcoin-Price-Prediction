# Bitcoin-Price-Prediction

# Project Structure
bitcoin-price-prediction/
├── train_model.py                  # Script to train and save LSTM model
├── bitcoin_actual_vs_forecast.py  # Final visualization and forecast script
├── model.h5                        # Trained LSTM model (saved after training)
├── scaler.pkl                      # Scaler used for normalization
├── requirements.txt                # Dependencies
└── README.md

# Install Dependencies
pip install -r requirements.txt

# Train the Model (First Time Only)
python train_model.py
-> Downloads BTC-USD price data
-> Trains an LSTM model
-> Saves the model and scaler

 Run Forecast and Visualization
Once the model is trained and saved, run:

# Run Forecast and Visualization
python bitcoin_actual_vs_forecast.py
This script:
-> Fetches last 60 days of real BTC prices
->Predicts next 7 days
->Plots actual vs predicted prices
