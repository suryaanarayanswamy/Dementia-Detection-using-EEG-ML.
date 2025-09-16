# Dementia Detection Using EEG  

##  Overview  
Built a CNN-LSTM model to classify EEG signals into Alzheimer’s Disease (AD), Frontotemporal Dementia (FTD), and Healthy Controls.  
Achieved 94% accuracy using class weighted training, outperforming baseline ML models.  

---

##  Tech Stack  
Python · TensorFlow/Keras · Scikit-learn · MNE · NumPy · Matplotlib  

---

## Dataset  
- EEG resting state, eyes closed recordings from **88 subjects** (AD, FTD, and Healthy Controls).  
- Source: [OpenNeuro ds004504 v1.0.8](https://openneuro.org/datasets/ds004504/versions/1.0.8)  
- Preprocessing: filtering, downsampling, normalization.  

---
## Code Files (what to run)

- `cnn-lstm with weights.ipynb` — **Main model** (AD vs FTD vs Healthy) with **class weights** → best results (~94%).
- `cnn-lstm without weights.ipynb` — Same multiclass model **without class weights** (for comparison/ablation).
- `binary.ipynb` — Binary setup (e.g., Dementia vs Healthy) to show the gap vs multiclass.
- `Multiclass.ipynb` — Multiclass Model with Dimentia vs FTD vs Healthy
  
---

## How to Build / Extend  
If you want to build from this project, you can:  
- Use the provided preprocessing pipeline to prepare EEG data for training.  
- Modify the CNN-LSTM architecture (e.g, add attention layers or dropout tuning).  
- Experiment with other deep learning models (e.g, Transformers for EEG).  
- Try different segmentation strategies (longer windows, overlapping samples).  
- Apply the same framework to other EEG datasets for generalization.  

---

##  Report  
Full details: [final_report.pdf](./ReportDimentia.pdf)  
