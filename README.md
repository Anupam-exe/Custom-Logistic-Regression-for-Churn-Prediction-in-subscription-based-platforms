<h1 style="font-size: 2.5em; text-align: center;">Customer churn prediction engine for subscription-based platforms</h1>
<h3 style="font-size: 1.3em; text-align: center; color: #586069;">NumPy-Based Logistic Regression & Mathematical Modeling</h3>

<hr>

<h2 style="font-size: 1.8em;">1. Project Overview</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
This project implements a custom-built Logistic Regression engine engineered entirely from scratch using NumPy to predict customer churn behavior. Designed with a focus on mathematical transparency and robust optimization, the system replaces black-box machine learning libraries for core model logic to provide full visibility into vectorization, sigmoid activation, and gradient descent. The framework incorporates comprehensive feature engineering, numerical feature standardization, L2 regularization, and explicit class imbalance handling. Furthermore, it features rigorous hyperparameter tuning (learning rate and iterations) backed by loss-per-iteration tracking and visualization.
</p>

<hr>

<p style="font-size: 1.1em; line-height: 1.6;">
This project was developed using data from Kaggle: 
👉 <a href="https://www.kaggle.com/datasets/sameerhussain007/subscription-churn-dataset" target="_blank">Subscription Churn Dataset</a>
</p>

<hr>

<h2 style="font-size: 1.8em;">2. Features</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Pure-NumPy Logistic Regression Engine:</b> Implements core model training, sigmoid activation, and gradient descent optimization entirely from scratch without relying on pre-built machine learning libraries.</li>
  <li><b>Feature Engineering & Standardization:</b> Includes robust preprocessing steps to enhance data quality, alongside numerical feature standardization to improve gradient descent convergence stability.</li>
  <li><b>L2 Regularization & Class Imbalance Handling:</b> Integrates L2 regularization to penalize large weights and prevent overfitting, alongside dedicated handling for class imbalance to ensure reliable prediction performance.</li>
  <li><b>Hyperparameter Tuning:</b> Allows fine-tuning of critical model configurations, specifically learning rates and total training iterations, to optimize model convergence.</li>
  <li><b>Loss & Iteration Tracking:</b> Visualizes gradient descent convergence, ROC curve comparisons, confusion matrices for both the custom NumPy model & scikit-learn baseline, and feature coefficients with their directional impact.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">3. Tech Stack</h2>

<h2 style="font-size: 1.8em;">3. Tech Stack</h2>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Python:</b> The core programming language utilized for data manipulation, mathematical operations, and pipeline execution.</li>
  <li><b>NumPy:</b> Powers the custom logistic regression engine, enabling high-performance vectorization, matrix operations, and gradient descent calculations.</li>
  <li><b>Pandas:</b> Used for data ingestion, cleaning, manipulation, and exploratory data analysis of the customer churn dataset.</li>
  <li><b>Scikit-learn:</b> Utilized to generate standard baseline models and metrics for direct performance comparison against the custom NumPy implementation.</li>
  <li><b>Matplotlib & Seaborn:</b> Utilized for generating professional data visualizations, including gradient descent convergence curves, ROC-AUC comparisons, confusion matrices, and feature coefficient impact plots.</li>
  <li><b>Jupyter Notebook:</b> Serves as the interactive single-notebook environment (`churn_prediction_model.ipynb`) ensuring full reproducibility from raw data to final evaluation.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">4. Project Structure</h2>

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

<h2 style="font-size: 1.8em;">5. Installation & Setup</h2>

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

<h2 style="font-size: 1.8em;">6. Usage</h2>

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

<h2 style="font-size: 1.8em;">7. Evaluation & Comparison</h2>

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
<b>Key Takeaways:</b>
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Competitive Performance:</b> The custom NumPy model achieves a competitive accuracy (75.13%) and a slightly higher <b>ROC-AUC score (0.7434 vs 0.7138)</b> compared to scikit-learn, proving the mathematical validity of the custom vectorization and gradient descent implementation.</li>
  <li><b>Class Sensitivity:</b> The custom model displays a higher recall for the churn class (0.53 vs 0.47), demonstrating an effective balance in handling class imbalance.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">8. Implementation Decisions & Trade-offs</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
Building a custom machine learning pipeline from scratch involves several critical design choices and architectural trade-offs:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Pure NumPy Implementation vs. Black-Box Libraries:</b> <i>Choice:</i> Implemented sigmoid activation, vectorization, and gradient descent entirely from scratch using NumPy. <i>Trade-off:</i> Sacrifices high-level library abstractions for complete mathematical transparency, granular control over matrix operations, and a deep understanding of underlying optimization mechanics.</li>
  <li><b>Numerical Feature Standardization:</b> <i>Choice:</i> Standardized all continuous input features prior to model ingestion. <i>Trade-off:</i> Introduces an extra preprocessing step, but is vital for preventing features with larger numeric scales from dominating the cost function and ensuring stable gradient descent convergence.</li>
  <li><b>Incorporating L2 Regularization:</b> <i>Choice:</i> Integrated L2 weight penalty terms directly into the custom cost function and gradient update formulas. <i>Trade-off:</i> Adds mathematical complexity to the codebase, but effectively controls model variance and prevents overfitting on training data.</li>
  <li><b>Explicit Class Imbalance Management:</b> <i>Choice:</i> Handled the skewed customer churn distribution during pipeline execution to boost minority class metrics. <i>Trade-off:</i> Requires careful threshold tuning, but prevents the model from achieving a misleadingly high accuracy by simply predicting the majority non-churn class.</li>
  <li><b>Single-Notebook Workflow Architecture:</b> <i>Choice:</i> Structured the project inside an interactive Jupyter environment (<code>churn_prediction_model.ipynb</code>) accompanied by serialized model outputs (<code>.npy</code>). <i>Trade-off:</i> Less modular than a multi-file production software package, but provides a clean, visual, and self-contained narrative ideal for exploratory analysis, debugging, and transparent reproducibility.</li>
</ul>

<hr>

<h2 style="font-size: 1.8em;">9. Limitations & Future Improvements</h2>

<p style="font-size: 1.1em; line-height: 1.6;">
Transparency regarding current constraints helps frame the scope of this project and outlines clear avenues for future evolution:
</p>

<ul style="font-size: 1.1em; line-height: 1.6;">
  <li><b>Current Limitations:</b> The pipeline relies on a single-notebook architecture which, while great for exploratory transparency, lacks modular production-grade scripts. Additionally, the project scope was intentionally restricted to a linear logistic regression model, meaning alternative algorithm types were not explored. While class distribution is managed, the custom model's minority class precision (churn class) also remains modest due to the inherent severe imbalance of the dataset.</li>
  <li><b>Future Improvements:</b> Next steps include refactoring the core logic into modular Python scripts (<code>.py</code>) with automated unit tests using <code>pytest</code>, implementing advanced hyperparameter tuning via grid search, and exploring alternative resampling techniques or cost-sensitive learning to further improve minority class detection. Furthermore, non-linear and ensemble alternatives—specifically <b>Support Vector Machines (SVM)</b>, <b>Decision Tree Classifiers</b>, and <b>Random Forest Classifiers</b>—can be added and benchmarked against the current implementation to evaluate complex decision boundaries and performance gains.</li>
</ul>
