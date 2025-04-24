# **Bitcoin Price Forecasting with Neural Networks & VARMAX**

This repository contains a data science project that leverages **machine learning** and **time series analysis** to forecast cryptocurrency price trends, specifically focusing on **Bitcoin price prediction**. The goal is to provide investors, traders, and financial institutions with predictive insights to make informed decisions in the volatile cryptocurrency market. The model is deployed on AWS for scalability, real-time predictions, and live data ingestion.

---

## **Key Features**

### **1. Machine Learning Modeling**
Two main modeling approaches are used to predict cryptocurrency prices:

- **LSTM-based Sequential Model**: A deep learning model trained on historical data to predict future price trends.
- **VARMAX Time Series Model**: A statistical model that performs time series forecasting based on historical price data.

The **LSTM model** achieves significant accuracy by using features like **open**, **high**, **low**, **close** prices, and **volume** over time.

### **2. Interactive Visualization**
The **Streamlit** dashboard provides:

- Real-time cryptocurrency price predictions.
- Visual comparison between observed and predicted prices.
- **Date hover** functionality for precise price retrieval.
  
The dashboard is hosted on **AWS EC2** for easy access and scalability.

### **3. AWS Cloud Deployment**
- **AWS SageMaker**: The model is deployed on SageMaker for scalable training and real-time predictions.
- **AWS Lambda & API Gateway**: For live cryptocurrency data ingestion.
- **AWS SNS (Simple Notification Service)**: Sends alerts when price thresholds are crossed.
- **AWS EC2**: Hosts the interactive **Streamlit** dashboard for visualization.

---

## **Prerequisites**

### **Libraries**
This project requires the following Python libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `bokeh`
- `sklearn`
- `keras`
- `statsmodels`
- `boto3` (for AWS integrations)
- `streamlit`

### **Data**
The model uses **historical cryptocurrency data** obtained from [Investing.com](https://www.investing.com/crypto/bitcoin/historical-data), containing features such as:

- **Open**, **High**, **Low**, **Close** prices
- **Volume**
- **Percentage change**

You can download the historical cryptocurrency data from the above website and use it with this project.

---

## **Getting Started**

### **Obtaining the Data**
1. Download historical cryptocurrency data from the Investing.com website:
   - [Bitcoin Data](https://www.investing.com/crypto/bitcoin/historical-data)
2. Save the data as `historical_prices.csv` in the `data/` folder.

