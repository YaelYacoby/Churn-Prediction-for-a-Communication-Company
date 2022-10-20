# A Machine Learning Framework with an Application to Predicting Customer Churn
The telecom operator Interconnect would like to be able to forecast their churn of clients. If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options. Interconnect's marketing team has collected some of their clientele's personal data, including information about their plans and contracts.

### Interconnect's services

Interconnect mainly provides two types of services:

1. Landline communication. The telephone can be connected to several lines simultaneously.
2. Internet. The network can be set up via a telephone line (DSL, *digital subscriber line*) or through a fiber optic cable.

Some other services the company provides include:

- Internet security: antivirus software (*DeviceProtection*) and a malicious website blocker (*OnlineSecurity*)
- A dedicated technical support line (*TechSupport*)
- Cloud file storage and data backup (*OnlineBackup*)
- TV streaming (*StreamingTV*) and a movie directory (*StreamingMovies*)

The clients can choose either a monthly payment or sign a 1- or 2-year contract. They can use various payment methods and receive an electronic invoice after a transaction.

### Data Description

The data consists of files obtained from different sources:

- `contract.csv` — contract information
- `personal.csv` — the client's personal data
- `internet.csv` — information about Internet services
- `phone.csv` — information about telephone services

In each file, the column `customerID` contains a unique code assigned to each client.

The contract information is valid as of February 1, 2020.

## Framework Steps
1. _Data Preparation_
  * Upload libraries
  * Preprocessing
  * Merging Strategy
2. _Exploratory Data Analysis_
  * Missing Values
  * Plottong Categorical Features
  * Plotting Numerical Features
  * Correlation
  * Pairplots
  * Boxplot
3. _Feature formating - One Hot Encoding_
  * Target class imbalance
  * Evaluation function
4. _Building a Model_
  * Split data
  * Choosing a metric
  * GridSearch and hyperparameter tuning for Random Forest
  * Creating a Model Pipeline
  * Find the best number for KNN model
  * Neural Network model with TensorFlow
  * Comparing Models using a Dummy Classifier

The final results of the ROC-AUC comparing several models are shown below:


| Model                                     | ROC AUC |
|-------------------------------------------|---------|
| Dummy Classifier                          | 0.5     |
| Decision Tree Classifier                  | 0.84    |
| Random Forest Classifier                  | 0.86    |
| KNN Classifier                            | 0.82    |
| CNN Classifier                            | 0.82    |
