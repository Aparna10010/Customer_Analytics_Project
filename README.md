Great update! Since you applied PCA (Principal Component Analysis) in your Customer Segmentation, here’s your fully updated README.md with that added under the correct section.


---

🧠 Customer Analytics Project

An end-to-end customer churn prediction and segmentation project. It includes EDA, SMOTE for class balancing, model training (baseline and tuned), dimensionality reduction using PCA, segmentation, model logging using MLflow, a live prediction interface using Gradio (with XGBoost tuned model), and Docker for containerization.


---

📁 Project Workflow

🔹 1. Data Preprocessing

Loaded the dataset

Cleaned and explored using EDA

Feature engineering & manipulation

Scaling and label encoding


🔹 2. Class Imbalance Handling

Visualized Churn Distribution

Applied SMOTE to fix imbalance


🔹 3. Model Building – Baseline

Trained the following models on imbalanced data:

Logistic Regression

Decision Tree

Random Forest

XGBoost


Evaluated using:

Confusion Matrix

AUC-ROC Curve


🔹 4. Model Building – Balanced (After SMOTE)

Re-trained above models

Added Feedforward Neural Network (FFNN)


🔹 5. Customer Segmentation

Applied PCA to reduce dimensionality and improve clustering results

Clustering Techniques:

K-Means

DBSCAN


Used:

Elbow Method

Silhouette Score


Clustered post-PCA-transformed data for better separation

Saved clustering results


🔹 6. Model Tracking with MLflow

Logged all baseline models

Applied Hyperparameter Tuning (RandomizedSearchCV)

Tuned: Logistic Regression, Decision Tree, Random Forest, XGBoost, FFNN


Logged all tuned models to MLflow with parameters, metrics, and artifacts


🔹 7. Gradio Deployment

Developed Gradio interface using XGBoost (tuned model)

Logged and tracked in MLflow with screenshot and link


🔹 8. Docker Containerization

Added Dockerfile and built image for portability



---

📸 Screenshots & Live Demo

📊 Class Imbalance Visualization



> Churn: 1 = Yes, 0 = No — imbalance handled using SMOTE




---

🌐 Live Gradio UI

▶ Launch Live App

> Predict customer churn using an interactive and minimal UI.




---

📋 MLflow Screenshot



> Shows baseline and tuned models, metrics, parameters, and Gradio App as an artifact.




---

🧪 Tech Stack

Languages & Libraries: Python, Pandas, NumPy, Scikit-learn, XGBoost, Keras/TensorFlow

Balancing: SMOTE (via imbalanced-learn)

Dimensionality Reduction: PCA

Clustering: KMeans, DBSCAN

Model Logging: MLflow

Deployment: Gradio

Containerization: Docker



---

🛠 Installation

✅ Create Environment & Install Dependencies

pip install -r requirements.txt

✅ Run Gradio App

python app.py

🐳 Docker Setup

docker build -t customer-analytics .
docker run -p 8501:8501 customer-analytics



❗ Limitations

Azure deployment skipped due to unavailability of a valid card (Visa/MasterCard required for signup)



---

🙋‍♀ Author

Aparna Sharmaa
Fresher | M.Com | Data Science Enthusiast
🔗 Actively looking for Data Analyst / ML roles


---
