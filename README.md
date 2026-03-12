# Final Project Submission - Machine Learning Dicoding

This project is the final submission for the **Machine Learning Beginner** class at Dicoding. It covers the implementation of **Clustering** and **Classification** using various machine learning algorithms.

---

## 📁 Repository Structure
├── [Clustering]Submission_Akhir_BMLP_Irfan_Maulana_Hakim.ipynb</br>
├── [Klasifikasi]Submission_Akhir_BMLP_Irfan_Maulana_Hakim.ipynb</br>
├── [Clustering]Submission_Akhir_BMLP_Irfan_Maulana_Hakim.py</br>
├── [Klasifikasi]Submission_Akhir_BMLP_Irfan_Maulana_Hakim.py</br>
├── data_clustering.csv</br>
├── data_clustering_inverse.csv</br>
├── model_clustering.h5</br>
├── PCA_model_clustering.h5</br>
├── decision_tree_model.h5</br>
├── explore_RandomForest_classification.h5</br>
├── tuning_classification.h5</br>
└── README.md</br>

---

## 🔬 Analysis Results

### 🎯 Clustering

|                |                         |
|----------------|-------------------------|
| **Method Used**               | K-Means        |
| **Optimal Number of Clusters**| 2              |
| **Determined using**          | Elbow Method   |

| Cluster | Characteristics | Sample Count | Interpretation |
|---------|-----------------|--------------|----------------|
| 0 | Older age (45.06), lower transaction amount ($255.55), longer transaction duration (121.12s), higher account balance ($5,142.17), Doctor occupation, Charlotte location | 980 | Mature professionals with stable financial behavior, prefer thorough and careful transaction processing |
| 1 | Middle age (44.33), higher transaction amount ($258.15), shorter transaction duration (117.30s), lower account balance ($5,058.81), Student occupation, Tucson location | 965 | Efficient students or postgraduates with practical transaction patterns, prioritize time optimization |

**Evaluation Metrics:**
- **Silhouette Score:** [0.5720739691275379] [Moderate]

**Visualization:**  
- **Include PCA 2D plot showing cluster distribution**

---

### 🎯 Classification

**Algorithms Compared:** Decision Tree, Random Forest</br>
⚠️Overfitting

| Model | Accuracy | Precision | Recall | F1-Score | Notes |
|-------|----------|-----------|--------|----------|-------|
| Decision Tree | 100% | 1.00 | 1.00 | 1.00 | Baseline model |
| Random Forest | 100% | 1.00 | 1.00 | 1.00 | Best performance |

**Hyperparameter Tuning Results:**

| Parameter | Best Value |
|-----------|------------|
| `n_estimators` | 50, 100, 200 |
| `max_depth` | None, 10, 20, 30 |
| `min_samples_split` | 2, 5, 10 |

| Field | Value |
|-------|-------|
| Final Model Selected | RandomForest |
| Reason | Both models achieved identical perfect performance (100% accuracy, precision, recall, and F1-Score). Random Forest selected as final model due to better robustness and generalization capability through bagging ensemble technique, reducing variance compared to single Decision Tree. |

---

## 🚀 How to Run

### Installation

```bash
# Clone the repository
git clone https://github.com/hanaricode/Submission-proyek-akhir-ML-Dicoding.git

# Navigate to directory
cd Submission-proyek-akhir-ML-Dicoding

# Install dependencies
pip install -r requirements.txt
```

### Running the Notebooks
```bash
# Launch Jupyter Notebook
jupyter notebook

# Or run specific notebook
jupyter notebook "[Clustering]_Submission_Akhir_BMLP_Irfan_Maulana_Hakim.ipynb"
jupyter notebook "[Klasifikasi]_Submission_Akhir_BMLP_Irfan_Maulana_Hakim.ipynb"
```
