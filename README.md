# ECG R-Peak Detection using Deep Learning

##  Overview

This project focuses on detecting R-peaks in ECG signals using a deep learning approach (LSTM model).
It includes preprocessing, normalization, training, and evaluation using cross-validation.

---

##  Features

* ECG signal preprocessing
* Signal normalization
* LSTM-based deep learning model
* R-peak detection
* 5-fold cross-validation
* Performance metrics:

  * Precision
  * Recall (Sensitivity)
  * F1 Score

---

##  Results

| Fold | Precision | Recall | F1 Score |
| ---- | --------- | ------ | -------- |
| 1    | 0.99      | 0.96   | 0.98     |
| 2    | 0.96      | 0.97   | 0.96     |
| 3    | 0.69      | 0.28   | 0.40     |
| 4    | 0.96      | 0.95   | 0.95     |
| 5    | 0.95      | 0.90   | 0.92     |

###  Average Performance

* Precision: ~91%
* Recall: ~81%
* F1 Score: ~84%

---

##  Tech Stack

* Python
* PyTorch
* WFDB (MIT-BIH dataset)
* NumPy
* Matplotlib
* Scikit-learn

---

##  How to Run

1. Install dependencies:

   ```
   pip install wfdb torch numpy matplotlib scikit-learn
   ```

2. Open the notebook:

   ```
   ecg_r_peak_detection.ipynb
   ```

3. Run all cells

---

##  Project Structure

```
ECG-r-peak-detection/
│── ecg_r_peak_detection.ipynb
│── lstm_model.ipynb
│── README.md
│── results/
│   ├── raw_signal.png
│   ├── normalized_signal.png
```

---

##  Dataset

* MIT-BIH Arrhythmia Database
* Accessed using WFDB library

---

## Note

One fold shows lower performance due to data imbalance. Future improvements can include better preprocessing and threshold tuning.

---

##  Author

Shreya Sharma

---

##  Future Work

* Improve model generalization
* Hyperparameter tuning
* Real-time ECG signal processing
* Deploy as a web application
