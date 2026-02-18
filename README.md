# Metaheuristic Algorithms for Feature Selection: A Comparative Study

Implementation and comparison of four metaheuristic algorithms for wrapper-based feature selection in high-dimensional machine learning under noise and complexity constraints.

## Overview
- **Dataset**: Breast Cancer Wisconsin (Diagnostic) – UCI  
  569 samples, 30 features, binary classification (M/B)
- **Base Model**: Logistic Regression (fixed hyperparameters)
- **Objective**:  
  Maximize: Accuracy (5-Fold CV) − α × (selected features / total)  
  α = 0.1
- **Algorithms** (4500 function evaluations each, 10 independent runs):
  - Genetic Algorithm (GA)
  - Simulated Annealing (SA)
  - Binary Particle Swarm Optimization (PSO)
  - Tabu Search (TS)
- **Noise Levels Tested**: 0, 0.05, 0.1
- **Key Results**:
  - **Best trade-off & stability**: Tabu Search (highest fitness, lowest #features ≈5–6, lowest std)
  - GA: very close second, good robustness
  - PSO: fast but less stable
  - SA: weakest performance and higher #features
