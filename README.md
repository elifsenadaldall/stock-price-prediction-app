# Stock Price Prediction App Using Prophet and LSTM Models

## **Authors**: Elif Sena Daldal
**Department**: Computer Engineering  
**Course**: CENG412 Graduation Project

---

## **Abstract**
This project presents a **Stock Price Prediction App** built on the Streamlit platform, designed to forecast stock prices using both the **Prophet** and **Long Short-Term Memory (LSTM)** models. The app utilizes historical stock data from Yahoo Finance and incorporates technical indicators such as **Exponential Moving Average (EMA)**, **Moving Average Convergence Divergence (MACD)**, and **Relative Strength Index (RSI)** to enhance prediction accuracy. Users can interactively select stock tickers to view historical trends and predict future stock prices.

Model performance is evaluated using metrics like **Root Mean Squared Error (RMSE)**, **Mean Absolute Error (MAE)**, and **R-squared (R²)**. This application bridges traditional statistical methods with advanced deep learning techniques, offering valuable insights for investors and market analysts.

---

## **Introduction**
The financial market demands accurate stock price predictions for better investment decisions and strategic planning. This project combines **Prophet**, a robust statistical model, and **LSTM**, a deep learning-based approach, to develop a Stock Price Prediction App that:

1. Visualizes historical data and technical indicators.
2. Provides interactive prediction capabilities.
3. Evaluates prediction accuracy using comprehensive backtesting techniques.

The goal is to simplify financial forecasting for both novice and experienced users, enabling them to make informed investment decisions.

---

## **Dataset**
- **Source**: Historical stock data from [Yahoo Finance](https://finance.yahoo.com/).
- **Attributes**: Opening price, highest price, lowest price, closing price, and volume.
- **Technical Indicators**:
  - **EMA**: Highlights recent price trends.
  - **MACD**: Identifies momentum and trend strength.
  - **RSI**: Signals overbought or oversold conditions.

---

## **Methodology**

### **1. Preprocessing Steps**
1. **Data Cleaning**:
   - Removed missing values.
   - Selected relevant attributes: 'Close', 'Volume', 'EMA', 'MACD', 'RSI', etc.
2. **Normalization**:
   - Scaled features using Min-Max normalization for better model performance.
3. **Train-Test Split**:
   - Divided data into 80% training and 20% testing sets.

### **2. Models Used**
1. **Prophet**:
   - Captures seasonality and holiday effects.
   - Known for interpretability and robust long-term forecasts.

2. **LSTM**:
   - Captures long-term dependencies in time series data.
   - Utilizes sequential embeddings for enhanced prediction accuracy.

### **3. Performance Metrics**
- **RMSE**: Measures average magnitude of prediction errors.
- **MAE**: Calculates average absolute errors.
- **R²**: Determines the proportion of variance explained by the model.

---

## **Results**

### **Model Comparison**
| Metric  | Prophet     | LSTM        |
|---------|-------------|-------------|
| RMSE    | Moderate    | Low         |
| MAE     | Moderate    | Low         |
| R²      | High        | Very High   |

### **Insights**
- **Prophet**:
  - Handles seasonality well and provides interpretable results.
  - Suitable for analyzing holiday effects and long-term trends.
- **LSTM**:
  - Outperforms Prophet in capturing complex patterns.
  - Requires higher computational resources but delivers better accuracy for volatile markets.

---

## **Features**
1. **Interactive Stock Selection**:
   - Users can choose stock tickers and visualize historical data.
2. **Historical Trends**:
   - Displays technical indicators like EMA, MACD, and RSI.
3. **Future Predictions**:
   - Provides forecasted prices using Prophet and LSTM models.

---

## **Usage**

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/username/stock-price-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### **Running the App**
1. Navigate to the project directory:
   ```bash
   cd stock-price-prediction
   ```
2. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

---

## **Technologies Used**
- **Streamlit**: For building the web application.
- **Prophet**: Statistical time series forecasting.
- **TensorFlow/Keras**: For implementing the LSTM model.
- **Pandas, NumPy**: Data manipulation and analysis.
- **Matplotlib, Seaborn**: Data visualization.

---

## **Future Work**
1. **Integration of More Models**:
   - Add models like ARIMA and GRU for comparison.
2. **Real-Time Data**:
   - Incorporate real-time stock data using APIs.
3. **Advanced Indicators**:
   - Include additional technical indicators like Bollinger Bands.
4. **Portfolio Optimization**:
   - Develop features for multi-stock analysis and portfolio management.

---

## **License**
This project is licensed under the MIT License. See the LICENSE file for more details.

---

## **Acknowledgments**
- Yahoo Finance for providing stock data.
- TensorFlow and Prophet for model implementation.
- Streamlit for enabling rapid app development.

