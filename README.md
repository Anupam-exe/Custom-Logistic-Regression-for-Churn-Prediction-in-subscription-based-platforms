<h1 style="font-size: 2.5em; text-align: center;">Customer churn prediction engine for subscription-based platforms</h1>
<h3 style="font-size: 1.3em; text-align: center; color: #586069;">NumPy-Based Logistic Regression & Mathematical Modeling</h3>

<hr>

<h2 style="font-size: 1.8em;">📝 1. Project Overview</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li>Implements a custom-built Logistic Regression engine engineered entirely from scratch using NumPy to predict customer churn behavior.</li>
  <li>Designed with a focus on mathematical transparency and robust optimization, replacing black-box libraries for core model logic.</li>
  <li>Provides full visibility into vectorization, sigmoid activation, and gradient descent optimization mechanics.</li>
  <li>Incorporates comprehensive feature engineering, numerical feature standardization, L2 regularization, and explicit class imbalance handling.</li>
  <li>Features rigorous hyperparameter tuning backed by loss-per-iteration tracking and training visualization.</li>
</ul>

<hr>

<p style="font-size: 1.1em; line-height: 1.6;">
This project was developed using data from Kaggle: 
👉 <a href="https://www.kaggle.com/datasets/sameerhussain007/subscription-churn-dataset" target="_blank">Subscription Churn Dataset</a>
</p>

<hr>

<h2 style="font-size: 1.8em;">✨ 2. Features</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Pure-NumPy Engine:</b> Implements core model training, sigmoid activation, and gradient descent entirely from scratch.</li>
  <li><b>Feature Engineering & Standardization:</b> Applies robust preprocessing and scaling to ensure stable gradient descent convergence.</li>
  <li><b>Regularization & Imbalance Management:</b> Integrates L2 regularization to prevent overfitting and handles class imbalance for reliable performance.</li>
  <li><b>Hyperparameter Tuning:</b> Enables fine-tuning of learning rates and training iterations to optimize convergence.</li>
  <li><b>Loss & Metric Tracking:</b> Visualizes gradient descent convergence, ROC curves, confusion matrices, and feature coefficients.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">🛠️ 3. Tech Stack</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Python:</b> The core programming language utilized for data manipulation, mathematical operations, and pipeline execution.</li>
  <li><b>NumPy:</b> Powers the custom logistic regression engine, enabling high-performance vectorization, matrix operations, and gradient descent calculations.</li>
  <li><b>Pandas:</b> Used for data ingestion, cleaning, manipulation, and exploratory data analysis of the customer churn dataset.</li>
  <li><b>Scikit-learn:</b> Utilized to generate standard baseline models and metrics for direct performance comparison against the custom NumPy implementation.</li>
  <li><b>Matplotlib & Seaborn:</b> Utilized for generating professional data visualizations, including gradient descent convergence curves, ROC-AUC comparisons, confusion matrices, and feature coefficient impact plots.</li>
  <li><b>Jupyter Notebook:</b> Serves as the interactive single-notebook environment (`churn_prediction_model.ipynb`) ensuring full reproducibility from raw data to final evaluation.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">🗂️ 4. Project Structure</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
The repository follows a clean, organized architecture separating code notebooks, saved model outputs, and configuration files:
</p>

<pre style="background-color: #f6f8fa; padding: 15px; border-radius: 6px; font-size: 1em;">
📊 Custom-Logistic-Regression-Churn-Prediction
├── 📁 notebooks
│   └── 📜 churn_prediction_model.ipynb    # Main Jupyter notebook containing the end-to-end pipeline
├── 📁 output
│   ├── 📄 X_test.npy                      # Serialized test features array
│   ├── 📄 b.npy                           # Trained model bias parameter
│   ├── 📄 w.npy                           # Trained model weight parameters
│   └── 📄 y_test.npy                      # Serialized test labels array
├── 📄 .gitignore                          # Specifies intentionally untracked files to ignore
├── 📄 README.md                           # Project documentation
└── 📄 requirements.txt                    # Python package dependencies list
</pre>

<p style="font-size: 1.1em; line-height: 1.6; margin-top: 15px;">
<b>Execution Workflow within the Notebook:</b>
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>1. Ingestion & EDA:</b> Loads the churn dataset, handles missing values, and explores feature distributions.</li>
  <li><b>2. Feature Engineering & Preprocessing:</b> Applies transformations, encodes categorical attributes, and standardizes numerical features.</li>
  <li><b>3. Model Training & Optimization:</b> Feeds data into the custom NumPy engine, applies L2 regularization, and executes gradient descent with loss-per-iteration tracking.</li>
  <li><b>4. Benchmarking & Evaluation:</b> Compares the custom NumPy model against a scikit-learn baseline using confusion matrices, ROC curves, and coefficient impact plots.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">⚙️ 5. Installation & Setup</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
To set up the environment and run the project locally, follow these steps:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Clone the Repository:</b> Download or clone the project files to your local machine using git.</li>
  <li><b>Install Dependencies:</b> Run the following command in your terminal to install all required libraries from the requirements file:
    <pre style="background-color: #f6f8fa; padding: 10px; border-radius: 6px; font-size: 0.95em; margin-top: 8px;">pip install -r requirements.txt</pre>
  </li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">⚡ 6. Usage</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
Because this project runs in an interactive notebook environment, follow this workflow to execute the code:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Launch Jupyter:</b> Open your terminal, navigate to the root directory, and start Jupyter Notebook or JupyterLab:
    <pre style="background-color: #f6f8fa; padding: 10px; border-radius: 6px; font-size: 0.95em; margin-top: 8px;">jupyter notebook</pre>
  </li>
  <li><b>Open Notebook:</b> Navigate to the <code>notebooks/</code> directory and open <code>churn_prediction_model.ipynb</code>.</li>
  <li><b>Execute Pipeline:</b> Run all cells sequentially from top to bottom to execute data ingestion, custom NumPy model training, gradient descent tracking, and scikit-learn benchmarking.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">⚖️ 7. Evaluation & Comparison</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
The performance of the custom NumPy logistic regression model was benchmarked directly against an industry-standard scikit-learn implementation. Below is the comparative breakdown of their evaluation metrics across test data:
</p>

<table style="width: 100%; border-collapse: collapse; margin: 20px 0; font-size: 1em; text-align: left;">
  <thead>
    <tr style="background-color: #f6f8fa; border-bottom: 2px solid #d1d5db;">
      <th style="padding: 12px; border: 1px solid #e5e7eb;">Metric</th>
      <th style="padding: 12px; border: 1px solid #e5e7eb;">Custom NumPy Model</th>
      <th style="padding: 12px; border: 1px solid #e5e7eb;">Scikit-Learn Baseline</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 10px; border: 1px solid #e5e7eb;"><b>Accuracy</b></td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">75.13%</td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">76.68%</td>
    </tr>
    <tr style="background-color: #f9fafb;">
      <td style="padding: 10px; border: 1px solid #e5e7eb;"><b>ROC-AUC Score</b></td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">0.7434</td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">0.7138</td>
    </tr>
    <tr>
      <td style="padding: 10px; border: 1px solid #e5e7eb;"><b>Class 0 Precision / Recall / F1</b></td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">0.89 / 0.80 / 0.84</td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">0.88 / 0.83 / 0.85</td>
    </tr>
    <tr style="background-color: #f9fafb;">
      <td style="padding: 10px; border: 1px solid #e5e7eb;"><b>Class 1 (Churn) Precision / Recall / F1</b></td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">0.36 / 0.53 / 0.43</td>
      <td style="padding: 10px; border: 1px solid #e5e7eb;">0.37 / 0.47 / 0.42</td>
    </tr>
  </tbody>
</table>

<p style="font-size: 1.1em; line-height: 1.6; margin-top: 15px;">
<b>🔍 Key Takeaways:</b>
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Competitive Performance:</b> The custom NumPy model achieves a competitive accuracy (75.13%) and a slightly higher <b>ROC-AUC score (0.7434 vs 0.7138)</b> compared to scikit-learn, proving the mathematical validity of the custom vectorization and gradient descent implementation.</li>
  <li><b>Class Sensitivity:</b> The custom model displays a higher recall for the churn class (0.53 vs 0.47), demonstrating an effective balance in handling class imbalance.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">🎯 8. Implementation Decisions & Trade-offs</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
Building a custom machine learning pipeline from scratch involves several critical design choices and architectural trade-offs:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Pure NumPy vs. Libraries:</b> Implemented sigmoid, vectorization, and gradient descent from scratch using NumPy, sacrificing high-level abstractions for complete mathematical transparency and control.</li>
  <li><b>Feature Standardization:</b> Standardized continuous input features prior to ingestion to prevent scale dominance and ensure stable gradient descent convergence.</li>
  <li><b>L2 Regularization:</b> Integrated L2 weight penalties directly into cost and gradient updates, adding mathematical complexity to effectively control variance and prevent overfitting.</li>
  <li><b>Class Imbalance Management:</b> Handled skewed churn distribution during execution, requiring threshold tuning to prevent deceptive high accuracy on the majority class.</li>
  <li><b>Single-Notebook Architecture:</b> Structured the project within an interactive Jupyter environment with serialized outputs, trading modularity for a clean, reproducible visual narrative.</li>
</ul>
<hr>

<h2 style="font-size: 1.8em;">⚠️ 9. Limitations</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
Current constraints and boundaries framing the scope of this project:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Single-Notebook Architecture:</b> Relies on an interactive notebook structure which lacks modular, production-grade scripts.</li>
  <li><b>Algorithm Scope:</b> Intentionally restricted to a linear logistic regression model, meaning alternative algorithm types were not explored.</li>
  <li><b>Minority Class Precision:</b> Despite class distribution management, precision for the minority churn class remains modest due to severe dataset imbalance.</li>
</ul>

<h2 style="font-size: 1.8em;">🚀 10. Future Improvements</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
Planned avenues and features for the evolution of this project:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Modular Refactoring:</b> Refactor core logic into modular Python scripts (<code>.py</code>) with automated unit tests using <code>pytest</code>.</li>
  <li><b>Advanced Tuning:</b> Implement grid search optimization for learning rates and regularization strengths.</li>
  <li><b>Enhanced Imbalance Handling:</b> Explore alternative resampling techniques or cost-sensitive learning to further improve minority class detection.</li>
  <li><b>Alternative Classifiers:</b> Integrate and benchmark non-linear and ensemble models—specifically Support Vector Machines (SVM), Decision Trees, and Random Forests—against the current implementation.</li>
</ul>
