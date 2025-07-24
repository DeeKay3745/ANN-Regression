# ANN Regression: Estimate Customer Salary

This project demonstrates how to use an Artificial Neural Network (ANN) for a regression problem—specifically, predicting the `EstimatedSalary` of a customer based on their profile data from the [Churn_Modelling.csv](Churn_Modelling.csv) dataset.

## Features

- **Data Preprocessing:**  
  - Drops irrelevant columns (`RowNumber`, `CustomerId`, `Surname`)
  - Label encodes `Gender`
  - One-hot encodes `Geography`
  - Scales features using `StandardScaler`
- **Model:**  
  - ANN built with TensorFlow/Keras
  - Two hidden layers (64 and 32 units, ReLU activation)
  - Output layer for regression
  - Early stopping and TensorBoard support
- **Deployment:**  
  - Streamlit app for interactive salary prediction

## Dataset

The dataset used is `Churn_Modelling.csv`, which contains customer information such as Geography, Gender, Age, Balance, Credit Score, Tenure, Number of Products, Has Credit Card, Is Active Member, and Estimated Salary.

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ANN-project-Implementation.git
   cd ANN-project-Implementation/ANN-Regression
   ```

2. **Create a virtual environment and install dependencies:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. **Train the model:**
   - Open and run `chrun_regression.ipynb` in Jupyter Notebook to preprocess data and train the ANN regression model.
   - This will save the trained model and encoders as `.pkl` and `.h5` files.

4. **Run the Streamlit app:**
   ```bash
   streamlit run streamlit_regapp.py
   ```

## Try the App Online

You can try the deployed regression app here:  
[https://ann-regression-7v9wtaxtldfctchxdbrxtq.streamlit.app/](https://ann-regression-7v9wtaxtldfctchxdbrxtq.streamlit.app/)

## Files

- `chrun_regression.ipynb` — Data preprocessing and model training notebook
- `streamlit_regapp.py` — Streamlit web app for regression
- `Churn_Modelling.csv` — Dataset
- `regression_modle.h5` — Saved ANN regression model
- `label_encoder_gender.pkl`, `onehot_encoder_geo.pkl`, `scaler.pkl` — Saved encoders and scaler
- `requirements.txt` — Python dependencies
- `runtime.txt` — Python version for deployment

## License

This project is for educational purposes.

---

**Deployed App:**  
[https://ann-regression-7v9wtaxtldfctchxdbrxtq.streamlit.app/](https://ann-regression-7v9wtaxtldfctchxdbrxtq.streamlit.app/)
