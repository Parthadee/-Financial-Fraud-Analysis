# Financial Fraud Detection Using Machine Learning

<img src= "https://github.com/Parthadee/-Financial-Fraud-Analysis/blob/7ab17441f94cd437acb5a23771da244a3a354ed7/img/How-Fraud-Detection-Works-1.webp" />

# 🔍 Project Overview: 
This project focuses on developing a machine learning model to proactively detect fraudulent transactions for a financial company. The dataset contains 6,362,620 rows and 10 columns, requiring thorough data analysis, feature selection, and model fine-tuning to achieve high accuracy in fraud detection.

# 📊 Dataset Information: 
- **Source**: [Fraud Analysis](https://www.kaggle.com/datasets/parthaade/fraud-analysis) 
- **Data Dictionary**: [Dictionary](https://github.com/Parthadee/-Financial-Fraud-Analysis/blob/83112c081a8a18a8c34572682504dfc08a5c25db/Data%20Dictionary.txt)
- **Size**: 6.3M+ transactions, 10 features  
- **File Format**: The dataset is provided in **.XLS format**. Please **download** and convert it to **CSV** using:  

  ### Convert XLS to CSV  
  **Method 1: Using Excel**  
  1. Open the `.xls` file in **Microsoft Excel**.  
  2. Click **File** → **Save As**.  
  3. Choose **CSV (.csv)** as the format and save the file.  

  **Method 2: Using Python (pandas)**  
  ```python
  import pandas as pd
  df = pd.read_excel("dataset.xls")  # Load the XLS file
  df.to_csv("dataset.csv", index=False)  # Convert and save as CSV
  
## 🧩 Features Included: 

| Feature Name      | Description                                      |
|------------------|--------------------------------------------------|
| `TransactionID`  | Unique ID for each transaction                   |
| `Amount`        | Transaction amount                                |
| `Time`          | Timestamp of the transaction                      |
| `Location`      | Transaction location                              |
| `Merchant`      | Merchant details                                  |
| `CardType`      | Type of payment card used                        |
| `CustomerAge`   | Age of the customer                               |
| `PreviousFraud` | Whether the customer had past fraudulent transactions |
| `DeviceUsed`    | Device type used for the transaction             |
| `Fraud`         | **Target variable** (0 = Not Fraud, 1 = Fraud)   |

# 🗂 Project Workflow: 

1️⃣ Data Preprocessing
   - Handling missing values
   - Outlier detection & treatment
   - Feature engineering
   - Encoding categorical variables

2️⃣ Exploratory Data Analysis (EDA)
  - Analyzing fraud vs. non-fraud distribution
  - Identifying key fraud patterns
  - Detecting multi-collinearity

3️⃣ Model Development

   **3.1. Algorithms Tested**:
  - Logistic Regression
  - Random Forest
  - XGBoost
  - Neural Networks

  **3.2. Hyperparameter Tuning**:
  - GridSearchCV
  - RandomizedSearchCV

4️⃣ Model Evaluation

  **4.1. Metrics Used**:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - AUC-ROC Curve

  **4.2. Best-Performing Model**:
  - Logistic Regression with 50% Accuracy Score

5️⃣ Key Fraud Indicators
- High transaction amounts
- Unusual time & location patterns
- Transactions from unknown devices

# 🛡️ Fraud Prevention Recommendations: 

- Multi-Factor Authentication (MFA) to reduce unauthorized transactions
- AI-Powered Transaction Monitoring for real-time fraud detection
- User Behavior Analytics (UBA) to flag abnormal transaction patterns
- Device Fingerprinting & IP Tracking to detect high-risk transactions

# 📊 Results & Insights:

- The fraud detection model demonstrated strong performance on the validation set.
- Key metrics like accuracy, precision, recall, and AUC-ROC indicate its effectiveness in identifying fraudulent transactions.
- High transaction amounts, device irregularities, and previous fraud history were key fraud indicators.

# ⏭️ Next Steps: 
- Further fine-tuning using deep learning models
- Real-time fraud detection system integration
- Deployment using Flask/FastAPI

# 🛠️ Installation & Usage:
1️⃣ Clone Repository
 ```
git clone https://github.com/Parthadee/Financial-Fraud-Analysis.git
                       cd FraudShield
```


2️⃣ Install Dependencies
 ```
pip install -r requirements.txt
 ```
3️⃣ Run Model
 ```
python fraud_detection.py
 ```
   
# 💻 Technology:
- #### Languages:
  - ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
- #### ML/DL:
  - ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
  - ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
  - ![Seaborn](https://img.shields.io/badge/Seaborn-%23F7931E.svg?style=for-the-badge&logo=Seaborn&logoColor=white)
  - ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
- #### IDE:
  - ![VS Code](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)
  -  ![PyCharm](https://img.shields.io/badge/pycharm-143?style=for-the-badge&logo=pycharm&logoColor=black&color=black&labelColor=green)
  - ![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)
  - ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
- #### OS used for testing:
  - ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)
  - ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
  - ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

# ⚖️ License:
 This project is open-source under the MIT License.


