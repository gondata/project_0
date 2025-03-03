# Interest Rate Prediction Using ARIMA

## 📌 Project Overview
This project applies **ARIMA (AutoRegressive Integrated Moving Average)** to predict **US 10-Year Treasury Yield (interest rates)** using historical data from **Yahoo Finance**. The goal is to build an accurate forecasting model, evaluate its performance, and compare it with Auto-ARIMA.

## 📊 Dataset
- **Source**: Yahoo Finance (`^TNX` - US 10-Year Treasury Yield)
- **Date Range**: 2000 - 2023
- **Frequency**: Daily interest rate closing values

## 🛠️ Libraries Used
```bash
pip install pandas numpy statsmodels matplotlib seaborn yfinance pmdarima
```
- `pandas`, `numpy`: Data manipulation
- `statsmodels`: ARIMA modeling
- `yfinance`: Download financial data
- `matplotlib`, `seaborn`: Data visualization
- `pmdarima`: Auto-ARIMA for model selection

## 🔹 Steps in the Notebook
### **1️⃣ Data Collection & Exploration**
- Download **US 10Y Treasury Yield** from Yahoo Finance
- Perform **Exploratory Data Analysis (EDA)**
- Visualize the interest rate trends

### **2️⃣ Stationarity Check & Differencing**
- Apply **ADF Test** to check stationarity
- If non-stationary, perform **first-order differencing**
- Re-run ADF test to confirm stationarity

### **3️⃣ ARIMA Model Implementation**
- Identify **(p, d, q) parameters** using **ACF & PACF plots**
- Train an **ARIMA model** and fit the data
- Generate **360-day interest rate forecasts**

### **4️⃣ Model Evaluation**
- Plot actual vs. predicted values
- Calculate **Root Mean Squared Error (RMSE)**
- Compare manual ARIMA vs. Auto-ARIMA results

## 📈 Results
- The ARIMA model provides short-term predictions with **confidence intervals**.
- RMSE is used to measure forecasting accuracy.
- Auto-ARIMA is tested to compare performance against manually tuned ARIMA.

## 🚀 Future Improvements
- Implement **SARIMA** to incorporate seasonal effects.
- Test **other financial datasets** (inflation rates, LIBOR, etc.).
- Build an interactive **dashboard** for better visualization.

## 📜 How to Run the Code
1. Clone this repository:
```bash
git clone https://github.com/yourusername/interest-rate-arima.git
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the Jupyter Notebook or Google Colab.

## 📂 Required Files
- `project_0.ipynb`: The main Jupyter Notebook containing the ARIMA model implementation.
- `requirements.txt`: List of dependencies needed to run the notebook.

## 🔗 Open in Google Colab
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yourusername/interest-rate-arima/blob/main/project_0.ipynb)
1. Clone this repository:
```bash
git clone https://github.com/gondata/interest-rate-arima.git
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the Jupyter Notebook or Google Colab.

## 💡 Author
**Gonzalo Noblega** - Data Scientist & Financial Modeling Enthusiast

---
📌 **If you find this project useful, feel free to ⭐ the repository!** 🚀

