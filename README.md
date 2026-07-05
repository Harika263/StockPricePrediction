# StockPricePrediction

# Stock Price Prediction Using Machine Learning and Django

## Overview

The AI Stock Price Prediction System is a web-based application developed using Django and Machine Learning techniques to forecast future stock prices based on historical stock market data.

This project uses historical stock data obtained from Yahoo Finance and applies Linear Regression algorithms to predict future stock prices. The application provides an interactive web interface where users can enter a stock ticker symbol and the number of days for prediction.

The project demonstrates the integration of:

- Django Web Framework
- Machine Learning
- Data Analysis
- Data Visualization
- Real-time Financial Data Collection

---

## Features

✅ Real-time stock data retrieval using Yahoo Finance

✅ Stock ticker validation

✅ Future stock price prediction

✅ Interactive graphical visualization using Plotly

✅ Error handling for invalid ticker symbols

✅ Error handling for invalid prediction days

✅ Responsive web interface

---

## Technologies Used

### Backend
- Python
- Django

### Machine Learning
- Scikit-learn
- Linear Regression

### Data Processing
- Pandas
- NumPy

### Data Collection
- yfinance

### Data Visualization
- Plotly

### Frontend
- HTML
- CSS
- Bootstrap

---

## Project Workflow

```text
User Input
     ↓
Django URL Routing
     ↓
Views.py
     ↓
Yahoo Finance API
     ↓
Pandas Data Processing
     ↓
Feature Engineering
     ↓
Train/Test Split
     ↓
Linear Regression Model
     ↓
Prediction
     ↓
Plotly Graph Generation
     ↓
HTML Template Rendering
```

---

## Data Source

This project uses historical stock market data from:

### Yahoo Finance

The stock data is retrieved dynamically using the Python library:

```python
import yfinance as yf
```

The downloaded data contains:

- Open Price
- High Price
- Low Price
- Close Price
- Adjusted Close Price
- Volume

---

## Machine Learning Model

The prediction model uses:

### Linear Regression

The model is trained using historical closing prices.

Example:

```text
Day        Close Price
1          100
2          105
3          110
4          115
```

The model learns historical patterns and predicts future stock prices.

---

## Project Structure

```text
StockPricePredictionProject
│
├── .gitignore
├── manage.py
├── requirements.txt
├── README.md
├── db.sqlite3
│
├── app
│   ├── templates
│   ├── static
│   ├── views.py
│   ├── models.py
│   ├── admin.py
│   └── urls.py
│
├── core
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
│
└── .venv
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/Harika263/StockPricePrediction.git

cd StockPricePredictionProject
```

---

### Create Virtual Environment

```bash
python -m venv .venv
```

Activate environment:

#### Windows

```bash
.venv\Scripts\activate
```

#### Linux/Mac

```bash
source .venv/bin/activate
```

---

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

### Run Migrations

```bash
python manage.py migrate
```

---

### Run Project

```bash
python manage.py runserver
```

Open:

```text
http://127.0.0.1:8000/
```

---

## Error Handling

The project handles:

- Invalid stock ticker
- Negative prediction days
- Invalid day formats
- API connection failures
- Overflow prediction days

---

## Future Improvements

- LSTM Deep Learning Model
- Random Forest Regression
- Stock News Analysis
- Sentiment Analysis
- Technical Indicators
- Portfolio Comparison Dashboard
- Multi-stock Prediction

---

## Author

### HarikaKalluru

LinkedIn:

https://www.linkedin.com/in/harikakalluru

GitHub:

https://github.com/Harika263

---

## License

This project is developed for educational and portfolio purposes.
