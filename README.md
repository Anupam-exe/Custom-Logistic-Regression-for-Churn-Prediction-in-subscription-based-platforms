<h1 style="font-size: 2.5em; text-align: center;">Customer churn prediction engine for subscription-based platforms</h1>
<h3 style="font-size: 1.3em; text-align: center; color: #586069;">NumPy-Based Logistic Regression & Mathematical Modeling</h3>

<hr>

<h2 style="font-size: 1.8em;">1. Project Overview</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
This project implements an industrial-grade, custom-built Logistic Regression engine engineered entirely from scratch using NumPy to predict customer churn behavior. Designed with a focus on mathematical transparency and robust data visualization, the system replaces black-box machine learning libraries for core model logic to provide full visibility into vectorization, sigmoid activation, and gradient descent optimization. To handle class imbalance and maximize practical utility, the framework integrates advanced threshold tuning strategies—including Youden’s J-statistic and F1-score optimization—alongside detailed feature coefficient impact analysis to identify primary customer retention and attrition drivers.
</p>

<hr>

<h2 style="font-size: 1.8em;">2. Features</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Pure-NumPy Logistic Regression Engine:</b> Implements core model training, sigmoid activation, and gradient descent optimization entirely from scratch without relying on black-box machine learning libraries.</li>
  <li><b>Advanced Threshold Tuning:</b> Integrates optimization strategies using Youden’s J-statistic and F1-score to handle class imbalance and maximize prediction accuracy beyond the default 0.5 threshold.</li>
  <li><b>Feature Coefficient Impact Analysis:</b> Analyzes and visualizes model weights to explicitly identify key customer retention and attrition drivers.</li>
  <li><b>Comprehensive Evaluation Metrics:</b> Generates professional performance diagnostics including ROC-AUC curves, confusion matrices, precision-recall metrics, and cost-benefit analysis.</li>
  <li><b>Clean Single-Notebook Architecture:</b> Organizes the entire data pipeline—from exploratory data analysis and preprocessing to model training and evaluation—inside a streamlined, reproducible environment.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">3. Tech Stack</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Python:</b> The core programming language utilized for data manipulation, mathematical operations, and pipeline execution.</li>
  <li><b>NumPy:</b> Powers the custom logistic regression engine, enabling high-performance vectorization, matrix operations, and gradient descent calculations.</li>
  <li><b>Pandas:</b> Used for data ingestion, cleaning, manipulation, and exploratory data analysis of the customer churn dataset.</li>
  <li><b>Matplotlib & Seaborn:</b> Utilized for generating professional data visualizations, including feature correlation heatmaps, ROC-AUC curves, confusion matrices, and coefficient impact plots.</li>
  <li><b>Jupyter Notebook:</b> Serves as the interactive single-notebook environment (`churn_prediction_model.ipynb`) ensuring full reproducibility from raw data to final evaluation.</li>
</ul>
