# OSA — Obstructive Sleep Apnea Detection

Detection and analysis of Obstructive Sleep Apnea using PSG snoring signals through signal processing, feature extraction, and machine learning–based clustering.

---

## 🧠 About

This project leverages **time-domain and frequency-domain features** extracted from PSG signals, combined with clinical data, to train deep learning models that classify OSA severity. The goal is to provide a reliable and automated diagnostic aid for clinicians.

---

## ⚙️ Tech Stack

- **Language**: Python
- **Data Processing**: NumPy, Pandas, SciPy  
- **Signal Analysis**: Feature extraction from PSG signals  


---

## 🔧 Features Extracted

- **MFCC, Delta MFCC** – Capture spectral patterns and their temporal changes from PSG signals.  
- **ZCR (Zero-Crossing Rate)** – Measures frequency variations and signal noisiness.  
- **Other Features** – Time-domain (mean, variance) and frequency-domain (spectral centroid, bandwidth) to summarize signal characteristics for OSA severity classification.


