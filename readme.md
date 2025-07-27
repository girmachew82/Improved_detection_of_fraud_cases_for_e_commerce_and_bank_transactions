# Improved detection of fraud cases for e-commerce and bank transactions
#### Task -1 
- Load data
    - `df_creditcard = pd.read_csv('../data/creditcard.csv')
 df_fraud = pd.read_csv('../data/Fraud_Data.csv')
 df_ipaddress = pd.read_csv('../data/IpAddress_to_Country.csv')
`
- Cleaning
   - `
    print("Drop duplicated data ", df_creditcard.drop_duplicates(inplace=True))
    `
   - Data type casting
        `df_fraud['signup_time'] = pd.to_datetime(df_fraud['signup_time'], errors='coerce')
        df_fraud['purchase_time'] = pd.to_datetime(df_fraud['purchase_time'], errors='coerce')
        `
- Exploratory Data Analysis (EDA)
    - `df_creditcard.describe(include='all')`
    - Univariate Analysis
        - `![alt text](output.png)`
    - Bivariate Analysis
- Merge Datasets for Geolocation Analysis
- Feature Engineering
- Data transformation
#### Task -2 Model Building and Training 
- Data Preparation:
- Separate features and target, and perform a train-test split. [‘Class’(creditcard), ‘class’(Fraud_Data)]
- Train-Test Split 
- Model Selection
    - Logistic Regression
    - Random Forest 
-Model Training and Evaluation


