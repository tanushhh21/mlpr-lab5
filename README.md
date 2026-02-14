

Overview
This repository contains the implementation of Lab 5 for the course Machine Learning and Pattern Recognition (Spring 2026). The project demonstrates a complete computer vision and machine learning workflow involving face detection, feature extraction, unsupervised clustering, and classification of a new image based on learned patterns.

Methodology
Face Detection
Faces are detected from the image Plaksha_Faculty.jpg using the OpenCV Haar Cascade classifier. Detected faces are highlighted using bounding boxes to verify successful detection.
Feature Extraction
Detected face regions are converted from BGR to HSV color space. The mean Hue and Saturation values are computed for each face and used as feature vectors representing color characteristics.
K-Means Clustering
The extracted features are clustered using the K-Means algorithm. Faces with similar color distributions are grouped together, and cluster centroids are calculated to represent each group.
Template Image Classification
A template image (Dr_Shashi_Tharoor.jpg) undergoes the same preprocessing and feature extraction steps. The trained K-Means model predicts the cluster label of the template image based on its feature values.
Visualization
Scatter plots are generated to visualize clusters, centroids, and the classification of the template image. These visualizations help interpret clustering behavior and classification outcomes.

Results
The implementation successfully detects faces, extracts color-based features, clusters similar faces, and classifies a new face image into an existing cluster. The visualizations demonstrate clear separation between clusters and validate the effectiveness of the chosen features.
Technologies Used
Python
OpenCV
NumPy
Matplotlib
Scikit-learn (K-Means)
SciPy


Lab-5/
│
├── Lab 5-Spring 2026.ipynb
├── Plaksha_Faculty.jpg
├── Dr_Shashi_Tharoor.jpg
├── README.md
└── results/ results.pdf

Key Learning Outcomes
Implementation of face detection using Haar Cascade classifiers.
Feature extraction using HSV color space.
Application of unsupervised learning through K-Means clustering.
Visualization and interpretation of clustering results.
Classification of unseen data using learned cluster patterns.

Conclusion
This lab demonstrates how computer vision techniques and unsupervised machine learning can be integrated to analyze and group visual data. The approach highlights the practical use of feature extraction and clustering methods for image-based analysis and classification tasks.

