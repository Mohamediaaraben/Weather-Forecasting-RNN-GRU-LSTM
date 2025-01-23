# Weather-Forecasting-RNN-GRU-LSTM
Projet de prévision météo avec RNN, GRU et LSTM
# Weather Forecasting with RNN, GRU, and LSTM

This project leverages Recurrent Neural Networks (RNN), Gated Recurrent Units (GRU), and Long Short-Term Memory (LSTM) networks to predict temperature values using historical weather data. The project demonstrates the use of time-series data for sequence prediction, which can be extended to other applications such as financial forecasting, energy demand prediction, and more.

## 📁 Project Structure

```
Weather-Forecasting-RNN-GRU-LSTM/
│
├── DLWP/                               # Deep Learning Weather Prediction models
│   ├── DLWP_GRU_MAE.ipynb               # GRU model trained with MAE loss
│   ├── DLWP_GRU_MSE.ipynb               # GRU model trained with MSE loss
│   ├── DLWP_LSTM_MAE.ipynb               # LSTM model trained with MAE loss
│   ├── DLWP_LSTM_MSE.ipynb               # LSTM model trained with MSE loss
│
├── notebooks/                           # Jupyter notebooks for experimentation
│   ├── data/
│   │   ├── GRU_MLayer_12hrs.log          # GRU training log for 12-hour forecasting
│   │   ├── GRU_MLayer_default.log        # GRU training log for default settings
│   │   ├── LSTM_MLayer_12hrs.log         # LSTM training log for 12-hour forecasting
│   │   ├── LSTM_MLayer_default.log       # LSTM training log for default settings
│   ├── OptimizedModel_12hrs.ipynb        # Optimized 12-hour forecast model
│   ├── OptimizedModel_default.ipynb      # Optimized default forecast model
│   ├── TimeSeriesSummary.ipynb           # Summary and visualization of results
│
├── src/                                  # Source code
│   ├── Features.py                        # Feature engineering and preprocessing
│   ├── GRU.py                              # Implementation of GRU model
│   ├── LSTM.py                             # Implementation of LSTM model
│   ├── RNNmodel.py                         # Base RNN model structure
│
├── LICENSE                               # License file
├── README.md                             # Project documentation
├── requirements.txt                      # Dependencies for the project
└── .gitignore                             # Files and folders to ignore in Git
```

## 🛠️ Installation and Setup

### Prerequisites
Ensure you have the following installed on your system:

- Python (3.8 or later)
- Git

### Steps to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/Weather-Forecasting-RNN-GRU-LSTM.git
   cd Weather-Forecasting-RNN-GRU-LSTM
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Prepare the dataset by placing historical weather data in the `data/` directory.

4. Run the models:

   ```bash
   python src/GRU.py
   python src/LSTM.py
   ```

## 📊 Dataset Description

The dataset used in this project includes:

- **Formatted Date:** Timestamps in UTC format.
- **Temperature (C):** Temperature values in Celsius.

### Preprocessing Steps

- Converted Formatted Date to UTC datetime format.
- Extracted relevant columns.
- Generated sequences for time-series forecasting.
- Normalized data for better performance.

## 🧠 Model Details

### GRU Model

- Layers: 2 GRU layers with 64 units each.
- Activation: tanh.
- Loss Function: Mean Squared Error (MSE).
- Optimizer: Adam.

### LSTM Model

- Layers: 2 LSTM layers with 64 units each.
- Activation: tanh.
- Loss Function: Mean Absolute Error (MAE).
- Optimizer: Adam.

## 📈 Results

- **Loss (MSE):** Measures how close predictions are to actual values.
- **RMSE:** Provides a more interpretable error measure.

## 🚀 Future Enhancements

- Replace current models with hybrid GRU-LSTM architectures.
- Introduce additional features such as humidity and wind speed.
- Experiment with different optimizers and batch sizes.

## 📬 Contact

Author: Mohamed Iaaraben  
Email: mohamed.iaaraben@etu.uae.ac.ma  
GitHub:https://github.com/Mohamediaaraben/Weather-Forecasting-RNN-GRU-LSTM/

## 🛡️ License

This project is licensed under the MIT License. See the LICENSE file for more details.

