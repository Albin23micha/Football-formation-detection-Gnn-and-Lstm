Tactical Formation Detection in Football using GNN + LSTM
Overview

This project develops a hybrid Graph Neural Network (GNN) and Long Short-Term Memory (LSTM) framework for automatic football formation detection using player tracking data.

The model captures:

Spatial relationships between players using Graph Neural Networks
Temporal formation evolution using LSTM
Formation clustering and classification
Tactical pattern recognition in football matches
Problem Statement

Traditional football formation analysis relies heavily on manual video review, which is:

Time-consuming
Subjective
Difficult to scale

This project automates tactical formation detection using deep learning and graph-based player interaction modeling.

Dataset

Dataset Used:

Metrica Sports Open Tracking Data

Contains:

Player coordinates (x, y)
Velocity and acceleration
Match event data
Frame-by-frame tracking information

Source:

Metrica Sports Sample Data Repository

Methodology
Data Preprocessing
Active-play filtering
Coordinate normalization
Velocity calculation
Acceleration calculation
Graph Construction

Each frame is converted into a graph:

Nodes → Players
Edges → K-Nearest Neighbors (KNN)
GNN Module

Graph Attention Network (GATConv)

Learns:

Player interactions
Team shape structure
Spatial dependencies
LSTM Module

Captures:

Formation evolution
Tactical transitions
Temporal dependencies
Classification
K-Means clustering
Formation classification
Accuracy and F1 evaluation
Architecture
Tracking Data
      │
      ▼
Data Preprocessing
      │
      ▼
Graph Construction
      │
      ▼
Graph Attention Network (GNN)
      │
      ▼
LSTM
      │
      ▼
Formation Classification
      │
      ▼
Visualization & Analytics
Results
Model	Accuracy	F1 Score
LSTM Baseline	35.7%	18.3%
GNN + LSTM	51.7%	45.0%

The hybrid GNN-LSTM model significantly outperformed the baseline by effectively learning spatial and temporal player interactions.

Technologies Used
Python
PyTorch
PyTorch Geometric
Scikit-Learn
Pandas
NumPy
Matplotlib
Future Improvements
Transformer-based temporal modeling
Real-time formation detection
Opponent-aware graph construction
Explainable AI using SHAP
Tactical transition prediction

These extensions were identified as future enhancements in the project.

Author

Albin Michael

M.Sc. Applied Data Science

SRM Institute of Science and Technology
