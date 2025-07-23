# Borehole Soil Parameter Prediction and Visualization Using TensorFlow MLP

This repository contains Python code to predict soil and foundation-related parameters for boreholes using a Multilayer Perceptron (MLP) neural network implemented with TensorFlow, and to visualize the prediction results with informative plots.

---

## Overview

The project consists of two main parts:

1. **Borehole Parameter Prediction with TensorFlow MLP**  
   - Takes field data from four known boreholes (BH-1 to BH-4) as input features.  
   - Predicts key soil parameters (e.g., N-value, Bearing Capacity, Groundwater Depth, Excavation Difficulty, Settlement Potential) for two additional boreholes (BH-5 and BH-6).  
   - Encodes categorical features and normalizes numerical data for effective model training.

2. **Visualization of Actual vs Predicted Bearing Capacities and Foundation Recommendations**  
   - Compares actual and predicted bearing capacities against average N-values.  
   - Plots predicted vs actual bearing capacity across depth.  
   - Displays spatial variability of predicted bearing capacity via heatmap interpolation across borehole locations.  
   - Visualizes recommended foundation types based on predicted bearing capacities and depth.

---

## Files

- `borehole_prediction_mlp.py`  
  TensorFlow MLP model for predicting BH-5 and BH-6 parameters based on BH-1 to BH-4 input data.

- `bearing_capacity_visualization.py`  
  Code for plotting Figures 2 and 3: comparison graphs, heatmaps, and foundation recommendation plots.

---

## Requirements

- Python 3.7 or later
- TensorFlow 2.x
- NumPy
- scikit-learn
- Matplotlib
- Seaborn

Install dependencies with:

```bash
pip install tensorflow numpy scikit-learn matplotlib seaborn
