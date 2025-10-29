🧬 Unsupervised Clustering of Acute Leukemia Gene Expression Data

### Revealing molecular subtypes of ALL and AML using unsupervised machine learning and dimensionality reduction in R

## 📖 Overview

Advances in **high-throughput sequencing technologies** have produced massive gene expression datasets containing thousands of genes, posing challenges for conventional analytical approaches.

This study applies **unsupervised machine learning** to explore intrinsic patterns and biological subgrouping within a **high-dimensional acute leukemia gene expression dataset**, focusing on **Acute Lymphoblastic Leukemia (ALL)** and **Acute Myeloid Leukemia (AML)** subtypes.

By integrating **K-Means**, **Hierarchical Clustering**, and **Principal Component Analysis (PCA)**, the project demonstrates how data-driven clustering can uncover clinically meaningful distinctions in complex genomic profiles — without relying on prior class labels.

---

## 🎯 Research Objectives

* Investigate **natural groupings** in high-dimensional leukemia gene expression data.
* Apply and compare **unsupervised learning algorithms** for subtype identification.
* Use **dimensionality reduction (PCA)** to visualize sample separability.
* Assess whether discovered clusters correspond to known **biological subtypes (ALL vs. AML)**.

---

## 🧩 Methodology

### 1. Data Preprocessing

* Imported and cleaned the acute leukemia gene expression dataset.
* Normalized expression values to ensure comparability across samples.
* Filtered non-informative features (low-variance genes).

### 2. Dimensionality Reduction

* Applied **Principal Component Analysis (PCA)** to reduce thousands of features into principal components.
* Visualized variance distribution and cluster separability using **biplots** and **variance explained plots**.

### 3. Unsupervised Clustering

* **K-Means Clustering**

  * Optimal *k* determined using the **Elbow Method** and silhouette analysis.
* **Hierarchical Clustering**

  * Performed with **complete linkage** and **Euclidean distance metric**.
  * Dendrogram inspection confirmed two distinct subclusters.

### 4. Validation

* Both K-Means and Hierarchical Clustering consistently identified **two robust clusters**.
* PCA revealed that **PC1 captured over 90% of total variance**, effectively separating samples along one axis.

---

## 📊 Results & Interpretation

* Two well-defined clusters emerged, reflecting **ALL and AML** subtype segregation.
* High concordance between clustering algorithms confirms **structural stability** in the dataset.
* PCA visualization highlights that a **single principal component** accounts for the majority of variation — suggesting a dominant biological signal.

**Conclusion:**
Combining **unsupervised clustering** with **dimensionality reduction** offers a reliable framework for uncovering biologically relevant patterns in genomic datasets, providing a scalable and interpretable approach to precision medicine research.

---

## 💻 Implementation Details

**Language:** R

**Core Libraries:**

* `tidyverse` – data manipulation and visualization
* `cluster` – clustering algorithms and validation
* `factoextra` – PCA and cluster visualization
* `ggplot2` – data visualization and aesthetics
* `stats` – K-Means, hierarchical clustering, and PCA computation

**Environment:**

* R version ≥ 4.2.0
* RStudio IDE

## 🔍 Key Insights

* Unsupervised algorithms can **reconstruct biological subtypes** purely from expression profiles.
* The dataset exhibits a **strong two-group structure**, driven by molecular differences between ALL and AML.
* PCA serves as both a **dimensionality reduction** and **interpretability** tool for genomics data.

Would you like me to make it slightly more **visual and GitHub-optimized** (with badges, section dividers, and emoji headers that make it stand out for recruiters or scholarship reviewers)? It keeps the academic tone but improves visibility when people browse your repository.
