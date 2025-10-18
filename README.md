# 📘 Bank Churn Prediction using Optimized ANN

This project aims to **predict customer churn** in a bank using an **optimized Artificial Neural Network (ANN)**. The dataset used is available on [Kaggle](https://www.kaggle.com/datasets/filippoo/deep-learning-az-ann).

---

## 📂 Project Structure

- `bankexit.pynb` : Complete notebook with the optimized ANN code.  
- `images/` : Folder containing screenshots (confusion matrix, loss, accuracy).  
- `README.md` : Project description.  

---

## ⚙️ Requirements

- Python >= 3.8  
- Libraries:  
  - `numpy`  
  - `pandas`  
  - `matplotlib`  
  - `scikit-learn`  
  - `keras` / `tensorflow`  

```bash
pip install numpy pandas matplotlib scikit-learn keras tensorflow
📝 Code Description
Data Loading and Preparation

Encoding categorical columns (Geography, Gender) using LabelEncoder.

Train/test split (80/20) and feature scaling with StandardScaler.

Handling Class Imbalance

Compute class_weights to compensate for the lower number of churned customers.

Building the ANN

3 hidden layers with ReLU activation and he_uniform initializer.

Dropout of 0.2 to prevent overfitting.

Output layer with sigmoid activation for binary prediction.

Optimizer: adam, Loss: binary_crossentropy.

Training

EarlyStopping on val_loss with patience = 10.

Batch size = 16.

Evaluation

Classification report and confusion matrix.

Visualize accuracy and loss curves.

Example Prediction

Predict a sample customer using an adjusted threshold (threshold = 0.6) for churn.

📊 Results
Confusion Matrix

Accuracy Curve

Loss Curve


📈 Conclusion
The optimized ANN predicts churn effectively with good overall accuracy.

Using class_weights and adjusting the threshold improves detection of at-risk customers.

This notebook can serve as a foundation for supervised machine learning projects on banking data.

🔗 Dataset
Churn Modelling Dataset on Kaggle
