


A Machine Learning project focused on unsupervised document classification using **Agglomerative Hierarchical Clustering**. This project explores text vectorization, dimensionality reduction, and a comparative analysis of different linkage methods against the K-Means baseline.

## 📌 Project Overview
This project aims to group BBC news articles into coherent categories without using predefined labels. By utilizing Hierarchical Clustering, we can visualize the relationships between documents through a dendrogram, allowing for a more granular understanding of document similarity compared to flat clustering methods.

## 🛠 Tech Stack
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** * `Scikit-learn` (TF-IDF, PCA, Clustering)
    * `Scipy` (Dendrograms & Linkage matrices)
    * `Pandas/Numpy` (Data Manipulation)
    * `Matplotlib/Seaborn` (Visualization)

## 📂 Dataset
The project uses the **BBC News Classification Dataset**, which contains 2,225 documents across five thematic categories: **Business, Entertainment, Politics, Sport, and Tech.**

## 🚀 Implementation Pipeline

### 1. Feature Engineering
* **Text Cleaning:** Removal of stop words and punctuation.
* **Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency) to convert text into numerical vectors.
* **Dimensionality Reduction:** Application of **PCA (Principal Component Analysis)** to reduce features to 50 dimensions, preserving variance while removing noise.

### 2. Hierarchical Clustering
We implement Agglomerative Clustering, where each document starts in its own cluster and pairs are merged based on similarity.
* **Linkage Methods Compared:** Single, Complete, Average, and Ward.
* **Dendrogram Analysis:** Visualizing the hierarchy to determine the optimal number of clusters.



### 3. Evaluation & Visualization
* **Cluster Purity:** Comparing the "ground truth" categories against the generated clusters.
* **K-Means Baseline:** Benchmarking the Hierarchical results against K-Means to evaluate performance differences.
* **2D Visualization:** Using PCA-reduced data to plot clusters on a 2D scatter plot.

## 📊 Key Results
| Method | Linkage/Algorithm | Purity Score |
| :--- | :--- | :--- |
| Hierarchical | Ward | *TBD%* |
| Hierarchical | Complete | *TBD%* |
| K-Means | N/A | *TBD%* |

> **Note:** Ward linkage typically outperforms other hierarchical methods on this dataset as it minimizes the variance within clusters.

## 🔧 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/saixg/hierarchical-clustering.git
   ```
2. Open the `notebook.ipynb` in Google Colab.
3. Upload your `kaggle.json` to download the dataset or manually upload the BBC CSV.
4. Run all cells to generate the plots and evaluation metrics.

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.


