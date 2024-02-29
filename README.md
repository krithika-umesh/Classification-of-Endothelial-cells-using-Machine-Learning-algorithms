# Classification-of-Endothelial-cells-using-Machine-Learning-algorithms
This repository aims to classify endothelial cell types using scRNA-seq datasets from brain and lymph node tissues. Employing supervised and unsupervised learning approaches, it integrates, preprocesses, and trains algorithms for accurate classification.
# Project Objective
The objective of this project was to integrate publicly available single-cell RNA sequencing datasets of endothelial cells from brain and lymph node tissues. The integrated data was then utilized to train different classification algorithms with the aim of determining the best model for classifying cell types using supervised and unsupervised learning approaches.
# Project Components
1) Preprocessing: Publicly available single-cell RNA sequencing datasets from brain (GSE134058) and lymph node tissues (GSE140348 and GSE198069) were sourced from NCBI GEO repository. The datasets underwent preprocessing steps like quality control, normalization and feature selection befor data integration.
2) Data integration: The datasets were integrated by using SCTransform method as a part of Seurat, a popular scRNA seq data analysis tool. The cell-types were grouped according to tissue-origin for UMAP visualization after the integration process for easy understanding. PCA and UMAP were performed on this data in R for visualizing the integration. The integrated data was extracted and used for classification using supervised learning approaches.
# Classification algorithms
Unsupervised learning: In this approach dimensionality reduction techniques of PCA and UMAP were used to visualize the data. K-Means algorithm was used for clustering. The elbow plot was used to determine the optimal k value. Accuracy and silhouette coefficient was used for the evaluation of clustering.
Supervised learning: The data was split into training and testing set in the ratio 80:20. Under supervised learning approach four different models were trained and tested with 3-fold cross-validation for accuracy, precision, and recall. The models are:
1) Support Vector Machines (SVM)
2) Decision Tree
3) Random Forest
4) Neural Network
# Technologies Used:
Python and R scripting languages were utilized for data preprocessing, feature engineering, and model training.
