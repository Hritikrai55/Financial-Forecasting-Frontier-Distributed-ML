# Big Data Banking Analysis Project

A comprehensive big data analytics project focused on banking data analysis using Apache Spark, Hadoop, and machine learning techniques to predict term deposit subscriptions and derive business insights.

- 🎓 [Project Certification](https://verified.sertifier.com/en/verify/22268440375331/)

## 📊 Project Overview

This project demonstrates end-to-end big data processing and analytics on banking data, including:
- Exploratory Data Analysis (EDA) with PySpark
- Machine Learning model development for predictive analytics
- Real-time transaction analysis
- Data parallelism implementation
- MapReduce programming examples

## 🎯 Business Objective

Predict whether a bank client will subscribe to a term deposit based on their demographic information, account details, and previous marketing campaign interactions. The insights help optimize marketing strategies and improve customer targeting.

## 📁 Project Structure

```
big-data-project/
├── README.md                                          # This file
├── bank.csv                                          # Banking dataset
├── Exploratory Data Analysis with Spark.ipynb       # EDA notebook
├── Machine Learning with Spark ML.ipynb             # ML modeling notebook
├── Real-Time Transaction Analysis.ipynb             # Real-time analytics
├── Data Parallelism.ipynb                          # Parallel processing examples
├── MapReduce Codes/                                # MapReduce implementations
└── Data Analysis and Management using Hadoop & Hive.docx  # Documentation
```

## 🔧 Technologies Used

- **Apache Spark**: Distributed data processing and analytics
- **PySpark**: Python API for Spark
- **Spark ML**: Machine learning library
- **Hadoop**: Distributed storage and processing
- **Hive**: Data warehousing and SQL-like queries
- **MapReduce**: Distributed computing paradigm
- **Python**: Primary programming language
- **Jupyter Notebooks**: Interactive development environment
- **Pandas & Matplotlib**: Data manipulation and visualization

## 📈 Dataset Description

The `bank.csv` dataset contains information about bank clients and their responses to marketing campaigns:

- **Size**: ~375KB with multiple features
- **Target Variable**: `y` (binary: yes/no for term deposit subscription)
- **Features Include**:
  - Demographics: age, job, marital status, education
  - Financial: balance, housing loan, personal loan
  - Campaign: contact type, duration, previous outcomes
  - Temporal: month, day of week

## 🚀 Key Features & Analysis

### 1. Exploratory Data Analysis (`Exploratory Data Analysis with Spark.ipynb`)
- **Data Inspection**: Schema analysis, summary statistics, data quality checks
- **Outlier Handling**: Filtered extreme values in balance column (>0 and <72,000)
- **Feature Engineering**: 
  - Created quarterly groupings from months
  - Age categorization using UDFs (<30, 30-60, >60)
  - String manipulations and transformations
- **Business Insights**:
  - Subscription rates by education level
  - Loan default rates by profession
  - Monthly contact success rates
  - Correlation analysis between age and balance
- **Visualizations**: Job distribution, contact patterns, success metrics

### 2. Machine Learning Pipeline (`Machine Learning with Spark ML.ipynb`)
- **Data Preprocessing**:
  - Missing value analysis (no missing values found)
  - Categorical encoding using StringIndexer
  - Feature vector assembly with VectorAssembler
- **Model Development**:
  - Algorithm: Logistic Regression
  - Train/Test Split: 80/20
  - Hyperparameter Tuning: 5-fold cross-validation
- **Model Performance**:
  - Training Accuracy: ~88.5%
  - Test Accuracy: ~89.8%
  - Feature Importance Analysis
- **Key Predictive Features**:
  - Previous outcome (`poutcome_index`)
  - Housing loan status (`housing_index`)
  - Personal loan status (`loan_index`)

### 3. Real-Time Analytics (`Real-Time Transaction Analysis.ipynb`)
- Stream processing capabilities
- Real-time data ingestion and analysis
- Transaction pattern detection

### 4. Data Parallelism (`Data Parallelism.ipynb`)
- Parallel processing techniques
- Performance optimization strategies
- Distributed computing examples

### 5. MapReduce Implementation (`MapReduce Codes/`)
- Custom MapReduce jobs
- Distributed data processing examples
- Hadoop ecosystem integration

## 📋 Prerequisites

### Software Requirements
- Python 3.7+
- Apache Spark 3.0+
- Hadoop (optional, for full ecosystem)
- Jupyter Notebook
- Java 8 or 11

### Python Dependencies
```bash
pip install pyspark pandas matplotlib numpy jupyter
```

## 🏃‍♂️ Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Hritikrai55/big-data-project.git
   cd big-data-project
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

4. **Run the notebooks in order**:
   - Start with `Exploratory Data Analysis with Spark.ipynb`
   - Then proceed to `Machine Learning with Spark ML.ipynb`
   - Explore other notebooks as needed

## 📊 Key Results & Insights

### Business Insights
- **Customer Segmentation**: Identified key demographic patterns in term deposit subscriptions
- **Campaign Optimization**: Previous campaign outcomes are the strongest predictor
- **Risk Assessment**: Loan status significantly impacts subscription likelihood
- **Temporal Patterns**: Certain months show higher contact success rates

### Technical Achievements
- **Scalable Processing**: Handled large datasets efficiently with Spark
- **Model Performance**: Achieved 89.8% accuracy in predicting subscriptions
- **Feature Engineering**: Created meaningful derived features for better predictions
- **Real-time Capability**: Implemented streaming analytics for live data processing

## 🔄 Model Pipeline

```
Raw Data → Data Cleaning → Feature Engineering → Model Training → Hyperparameter Tuning → Model Evaluation → Deployment Ready
```

## 📈 Performance Metrics

| Metric | Training Set | Test Set |
|--------|-------------|----------|
| Accuracy | 88.5% | 89.8% |
| Model Type | Logistic Regression | Logistic Regression |
| Cross-Validation | 5-fold | - |

## 🚀 Future Enhancements

- **Advanced Algorithms**: Implement Random Forest, Gradient Boosting
- **Feature Engineering**: Create interaction terms and polynomial features
- **Class Imbalance**: Address potential imbalance in target variable
- **Model Deployment**: Containerize model for production deployment
- **Real-time Scoring**: Implement real-time prediction API
- **A/B Testing**: Framework for testing different model versions

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-analysis`)
3. Commit your changes (`git commit -am 'Add new analysis'`)
4. Push to the branch (`git push origin feature/new-analysis`)
5. Create a Pull Request


## 👨‍💻 Author

**Hritik**


## 📞 Contact
- 🌐 [LinkedIn Profile](https://www.linkedin.com/in/hritik-rai-/)
---

*This project demonstrates practical application of big data technologies in the banking sector, showcasing end-to-end data science workflows from exploration to model deployment.*
