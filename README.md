
# ECG Signal Classification with Bio-Simulated Data

This notebook processes bio-simulated ECG signal, extracts QRS complex after denoising, and classifies them using a pre-trained model (from previous project). The model successfully predicts the class as **Normal (N)** for the provided data.

## Workflow

1. **Signal Creation**:
   - ECG signals are generated using a bio-simulator.
   - These signals are recorded and saved in CSV format using a digital oscilloscope.

2. **Preprocessing**:
   - The ECG signal is filtered using a bandpass filter to remove noise.
   - Z-score normalization is applied for standardization.

3. **R-Peak Detection**:
   - Detects R-peaks in the ECG signal to locate QRS complexes.

4. **QRS Complex Extraction**:
   - Extracts QRS complexes around detected peaks.
   - The extracted complexes are saved in a CSV file for classification.

5. **Classification**:
   - A pre-trained deep learning model classifies the QRS complex.

---

## Requirements

Install the following Python libraries:
- `numpy`
- `scipy`
- `matplotlib`
- `pandas`
- `tensorflow`

---


## Outputs

- **Plots**:
  - Raw ECG signal.
  - Denoised and normalized ECG signal.
  - Detected R-peaks and QRS complexes.

- **CSV File**:
  - Extracted QRS complexes (`qrs_complex.csv`).

- **Prediction**:
  - The predicted class is **Normal (N)**.

---

![prediction class](https://github.com/murugaveltarun/ECG-single-sample-prediction/blob/86902c223a2f294e7faa353a78643e1b13f9fb2a/files/pred.png)
