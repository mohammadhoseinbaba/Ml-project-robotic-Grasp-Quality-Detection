# Grasp Quality Detection via Vibration Analysis

This project uses accelerometer data and machine learning techniques to predict the quality of robotic grasps. The goal is to classify grasps as **successful** or **failed** based on vibration signals during the manipulation process.

---

## Overview

Grasp quality is critical in robotic manipulation. This notebook-based project leverages:

- **Accelerometer data** from the Kaggle [Grasping Dataset](https://www.kaggle.com/datasets/ugocupcic/grasping-dataset)
- **Feature extraction** from vibration signals
- **Machine Learning classification** (Random Forest, SVM)
- **Model evaluation** with accuracy, F1-score, confusion matrix, and visualization

---

## Dataset

- **Source**: [Kaggle Grasping Dataset](https://www.kaggle.com/datasets/ugocupcic/grasping-dataset)
- **Content**: Accelerometer signals from robotic gripper movements
- **Target Label**: Binary classification (0 = failed grasp, 1 = successful grasp)

---

## Features Extracted

From each vibration signal sample:
- Statistical metrics (mean, std, min, max)
- Signal energy and entropy
- Frequency-domain features via FFT

---

## Models Trained

- **Random Forest**
- **Support Vector Machine (SVM)**

Hyperparameter tuning was performed using `GridSearchCV`.

---

## Evaluation Metrics

- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix
- Feature Importance Plot

---

## How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/grasp-quality-detection.git
   cd grasp-quality-detection
   ```

2. Open the notebook:
   ```bash
   jupyter notebook grasp_detection.ipynb
   ```

3. Make sure the dataset is in the correct relative path or update the file path accordingly.

---

## Sample Results

| Metric      | Value |
|-------------|-------|
| Accuracy    | ~95%  |
| F1-Score    | ~0.97 |
| Success Rate| High reliability in classifying vibration patterns |

---

## References

- Dataset: [Grasping Dataset - Kaggle](https://www.kaggle.com/datasets/ugocupcic/grasping-dataset)
- Techniques inspired by studies in robotic grasp stability and vibration sensing.

---

## Future Improvements

- Real-time deployment on physical robot
- Use of Deep Learning (LSTM/CNN) for raw signal input
- Integration with vision-based grasping systems

---

## Author

Mohammadhossein baba<br>
Feel free to contact for collaboration or feedback.
