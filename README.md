
# Geomagnetic Storm Forecasting Using NASA OMNI Data with Machine Learning

This project will involve developing a geomagnetic storm forecasting model using OMNI 2 space weather data from the NASA OMNIWEB website.

The idea is to train a Long Short-Term Memory (LSTM) model to forecast geomagnetic storm parameters such as the planetary Kp index and the Dst Index.

The necessary data will be downloaded from:
- [OMNI Low Resolution Data](https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/)
- [OMNI Data Description](https://omniweb.gsfc.nasa.gov/ow.html)

---

### 1. Clone the repository

```bash
git clone https://github.com/ngoosojk/geomagnetic-storm-forecasting.git
cd geomagnetic-storm-forecasting
```

### 2. Set up the virtual environment

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install required packages

```bash
pip install -r requirements.txt
```

### 4. Launch the Jupyter notebook

```bash
jupyter notebook Analysis.ipynb
```

---

## 🧠 Modeling Approach

- **LSTM (Long Short-Term Memory)** neural networks are used for time-series forecasting.
- The **multi-class learning** approach will be utilised to predict Kp and Dst simultaneously.
- **Autocorrelation (ACF) and Partial Autocorrelation (PACF)** are used to analyse temporal dependencies and guide feature selection.
- Missing values are handled using **time-aware strategies** such as interpolation, masking, or LSTM’s inherent ability to manage sequences with missing data.

---

## 🎯 Project Objectives

- Forecast **Kp Index** and **Dst Index** values ahead of time.
- Understand the link between **solar wind conditions** and **geomagnetic activity**.
- Develop a baseline model for **space weather forecasting**.
- Provide clear visualizations and insights from the data over time.

---

## 📌 Dependencies

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `plotly`
- `statsmodels`
