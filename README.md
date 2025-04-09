# Material-Cost-Prediction-System
🔍 Project Overview
This project aims to improve early-stage construction cost predictions by integrating Building Information Modeling (BIM) data with deep learning techniques. It helps in estimating construction costs with greater accuracy even when design changes occur during the schematic stage.

📚 Key Concepts to Highlight
1. Schematic Design Stage Challenge
At this early architectural phase, accurate material cost prediction is difficult due to a lack of detailed component data. Traditional methods like unit-cost estimation have an error margin of 10–25%.

2. Building Information Modeling (BIM)
BIM provides object-level attributes like wall area, floor perimeter, number of stairs, etc., which change dynamically with design updates. These can be used to predict costs more precisely than relying on static factors.

3. Data Categorization
Building General Properties: Total area, number of floors, building area, etc.

BIM Properties: Wall area, floor perimeter, stair steps, number of openings, etc.

Combining both yields higher prediction accuracy.

4. Machine Learning Approach
Model: Deep Neural Network (DNN) with fully connected layers.

Selection of Features: Based on Pearson correlation coefficient to ensure high relevance to construction cost.

Cross-Validation: Used k-fold cross-validation to prevent overfitting due to the limited dataset (78 buildings).

5. Model Configurations
Tested various configurations (Case A–F) with different activation functions (ReLU, Tanh, Elu) and learning rates to identify optimal performance.

6. Performance Metrics
Three datasets were tested:

General-only: Error ~33%

BIM-only: Error ~37%

Combined (Com-2): Lowest error ~21%

This clearly showed that integrating BIM and general data improves cost prediction accuracy.

🚀 Technologies Used
Python

TensorFlow / Keras (for DNN)

Pearson Correlation for feature selection

BIM Tools (e.g., Revit or other modeling software)

Pandas & NumPy (for data processing)

📈 Results Summary
Dataset Type	Mean Error Rate
General Properties	33.04%
BIM Properties	37.33%
Combined (Com-2)	✅ 20.82%
Conclusion: Combining traditional and BIM attributes significantly boosts cost prediction accuracy during early design stages.

💡 Future Improvements
Collect larger datasets for better training.

Integrate real-time cost data from APIs.

Extend to include energy consumption or environmental impact predictions.
