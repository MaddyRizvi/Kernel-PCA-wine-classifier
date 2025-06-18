# Kernel PCA for Wine Classification

## 📝 Summary

This project implements Kernel Principal Component Analysis (Kernel PCA) for dimensionality reduction followed by Logistic Regression for classification. The model is trained and evaluated on the Wine dataset, visualizing the decision boundary in reduced dimensions.

## 📂 Dataset

The dataset used is `Wine.csv`, containing chemical analysis results of wines grown in the same region in Italy but derived from three different cultivars.

- **Features:** 13 chemical analysis attributes (e.g., alcohol, malic acid, etc.)
- **Target:** Cultivar class (1, 2, or 3)

## 📁 Project Structure

```
├── Wine.csv
├── kernel_pca_classification.py
├── README.md
└── CONTRIBUTING.md
```

## 📦 Requirements

Install the following Python packages:

```
numpy
matplotlib
pandas
scikit-learn
```

You can install them using:

```bash
pip install -r requirements.txt
```

## 🚀 How to Run

1. Ensure `Wine.csv` is in the same directory.
2. Run the script:

```bash
python kernel_pca_classification.py
```

## 📊 Output

- Confusion matrix and accuracy printed to the console.
- Visualizations for both training and test sets after Kernel PCA reduction and classification.

## 📌 Details

- **Algorithm:** Kernel Principal Component Analysis + Logistic Regression
- **Dimensionality Reduction:** `KernelPCA` with RBF kernel, reducing to 2 components
- **Distance Metric:** Implicitly handled by RBF kernel (Gaussian)
- **Classifier:** Logistic Regression (Multiclass)

## 🧠 Understanding

Kernel PCA allows projecting data into higher-dimensional space implicitly through kernel functions, making linear separation possible for non-linearly separable data.

Here, after applying RBF Kernel PCA, the dataset is reduced to 2 dimensions to visualize decision boundaries clearly and improve classifier performance on complex, nonlinear data.

## 🤝 Contributing

Please see `CONTRIBUTING.md` for how to contribute and suggest improvements.

## 📄 License

This project is licensed under the MIT License.