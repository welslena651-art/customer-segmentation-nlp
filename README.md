# Customer Segmentation & Real-Time Classification Pipeline

This project combines RFM (Recency, Frequency, Monetary) analysis with NLP-derived sentiment metrics to segment customer populations using K-Means clustering and train a real-time supervised classification model.

## Key Results
* **Optimal Clusters ($k = 3$):** Identified via Silhouette Score (0.6531).
  * **Cluster 0 (At-Risk / Disgruntled):** Low spending, high inactivity, negative sentiment (-0.65).
  * **Cluster 1 (Mid-Tier / Moderate):** Moderate spending and activity, neutral-to-positive sentiment.
  * **Cluster 2 (VIP Champions):** High spending, frequent activity, highly positive sentiment (+0.75).
* **Classification Accuracy:** 99% test accuracy using both Random Forest and XGBoost classifiers.

## Features
* Unsupervised K-Means clustering with standard feature scaling.
* Supervised model training (Random Forest & XGBoost) for real-time customer segmentation.
* Serialized `.joblib` pipelines for instant deployment.

## How to Run

1. **Clone repository:**
   ```bash
   git clone [https://github.com/your-username/customer-segmentation-nlp.git](https://github.com/your-username/customer-segmentation-nlp.git)
   cd customer-segmentation-nlp
