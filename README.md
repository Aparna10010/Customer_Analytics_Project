
---

# 🧠 Customer Analytics Project

An end-to-end **Customer Churn Prediction and Segmentation** pipeline built from scratch. The project includes EDA, class balancing with SMOTE, model training and tuning, dimensionality reduction, customer segmentation, live predictions using Gradio, model tracking via MLflow, and Docker containerization.

---

## 📁 Project Workflow

### 🔹 1. Data Preprocessing

* Loaded dataset and explored via EDA
* Feature engineering and transformation
* Scaling and label encoding

### 🔹 2. Class Imbalance Handling

* Visualized churn distribution
* Applied **SMOTE** to fix class imbalance

### 🔹 3. Model Building – Baseline

Trained on **imbalanced** data:

* Logistic Regression
* XGBoost

Evaluated using:

* Confusion Matrix
* AUC-ROC Curve

### 🔹 4. Model Building – After SMOTE (Balanced)

Re-trained above models and added:

* **Feedforward Neural Network (FFNN)**

### 🔹 5. Customer Segmentation

* Applied **PCA** for dimensionality reduction
* Clustering Techniques:

  * K-Means
  * DBSCAN
* Evaluated with:

  * Elbow Method
  * Silhouette Score
* Saved post-PCA cluster results

### 🔹 6. Model Tracking with MLflow

* Logged **all baseline and tuned models**
* Hyperparameter tuning with **RandomizedSearchCV**
* Tracked metrics, parameters, and artifacts

### 🔹 7. Gradio Deployment

* Built interactive **Gradio interface** using tuned XGBoost
* Integrated with MLflow as an artifact

### 🔹 8. Docker Containerization

* Dockerized entire app with `Dockerfile`
* Built and ran container for portability

---

## 📸 Screenshots & Visuals

### 📊 Class Imbalance Visualization
![Churn Distribution]()

> Churn: `1 = Yes`, `0 = No` — imbalance addressed using **SMOTE**

### 🌐 Live Gradio UI

▶ [Launch Gradio App Live](https://74210d45131a11131e.gradio.live/)

> Predict customer churn using an interactive, minimal UI.

### 📋 MLflow Tracking
![ML-Flow Screenshots]()


> Includes baseline and tuned models with metrics, parameters, and UI screenshots logged as artifacts.

---

## 🧪 Tech Stack

* **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, XGBoost, Keras/TensorFlow
* **Balancing**: SMOTE (via `imbalanced-learn`)
* **Dimensionality Reduction**: PCA
* **Clustering**: KMeans, DBSCAN
* **Model Tracking**: MLflow
* **Deployment**: Gradio
* **Containerization**: Docker

---

## 🛠 Installation & Usage

### ✅ Setup Environment

```bash
pip install -r requirements.txt
```

### ✅ Run Gradio App

```bash
python app.py
```

### 🐳 Docker Setup

```bash
docker build -t customer-analytics .
docker run -p 8501:8501 customer-analytics
```

---

## ❗ Limitations

* Azure deployment was **skipped** due to the unavailability of a valid card (Visa/MasterCard required for signup)

---

## 🙋‍♀ Author

**Aparna Sharmaa**
Fresher | M.Com | Data Science Enthusiast
🔍 *Actively looking for Data Analyst / Scientist*

---

