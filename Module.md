# Machine Learning in Genomics (HPC Edition)

This is a 3-week mini-module designed for undergraduate biology majors who have experience working on the command line of a high-performance computing (HPC) cluster. It introduces students to basic machine learning (ML) concepts and applies them to real genomic data.

## 🧭 Structure
- **Week 1**: Introduction to Machine Learning and Genomics
- **Week 2**: Supervised Learning with Gene Expression Data
- **Week 3**: Unsupervised Learning (PCA & Clustering)

## 📁 Folder Structure
```
ml-genomics-hpc/
├── data/
│   └── TCGA_BRCA_expression_subset.tsv
│   └── sample_labels.txt
├── week2_supervised/
│   └── run_knn_classifier.py
├── week3_unsupervised/
│   └── pca_and_clustering.py
├── env_setup.md
├── README.md
└── LICENSE
```

## 🔧 Setup
1. Log into your HPC cluster
2. Load Python:
   ```bash
   module load python/3.10
   python -m venv ml_env
   source ml_env/bin/activate
   pip install -r requirements.txt
   ```

## 🧪 Week 2 — Supervised Learning (Classification)
- Navigate to `week2_supervised/`
- Run:
  ```bash
  python run_knn_classifier.py --data ../data/TCGA_BRCA_expression_subset.tsv --labels ../data/sample_labels.txt
  ```
- Outputs:
  - Accuracy
  - Confusion matrix

## 🔍 Week 3 — Unsupervised Learning (PCA & Clustering)
- Navigate to `week3_unsupervised/`
- Run:
  ```bash
  python pca_and_clustering.py --data ../data/TCGA_BRCA_expression_subset.tsv --k 3
  ```
- Outputs:
  - PCA plot
  - Explained variance
  - Cluster assignments

## 📚 Resources
- [StatQuest on ML](https://youtube.com/playlist?list=PLblh5JKOoLUIxGDQs4LFFD--41Vzf-ME1)
- [Libbrecht & Noble 2015](https://www.nature.com/articles/nrg3920)

---

Want to contribute? Open an issue or submit a pull request!
