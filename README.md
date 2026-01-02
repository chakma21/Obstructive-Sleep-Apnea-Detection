# OSA — Obstructive Sleep Apnea Detection

Detection and analysis of **Obstructive Sleep Apnea (OSA)** using **PSG (Polysomnography) snoring audio signals** through **signal processing, feature extraction, and machine learning–based clustering**.

---

## About

This project focuses on analyzing **PSG audio signals**, particularly **snoring and respiratory sounds**, to identify patterns associated with Obstructive Sleep Apnea.  
Instead of relying on raw signals, meaningful **time-domain, frequency-domain, and cepstral features** are extracted and used with **classical machine learning techniques** to distinguish between **normal breathing and apnea-related snoring events**.

The objective is to explore an **automated and data-driven approach** that can assist clinicians by reducing the manual effort involved in PSG analysis.

---

## Tech Stack

- **Language**: Python  
- **Numerical & Data Processing**: NumPy, Pandas  
- **Signal Processing**: SciPy 
- **Machine Learning**: sklearn  
- **Visualization**: Matplotlib, Seaborn

---

## Features Extracted

- **MFCC & Delta MFCC**  
  Capture short-term spectral characteristics of snoring sounds and their temporal variations.

- **ZCR (Zero-Crossing Rate)**  
  Measures how frequently the signal changes sign, indicating irregular breathing patterns.

- **Time-Domain Features**  
  Mean, variance, RMS, peak-to-peak, skewness, and kurtosis to describe signal behavior over time.

- **Frequency-Domain Features**  
  Spectral centroid and bandwidth to analyze the distribution of signal energy.

- **LPC & Formant-Based Features**  
  Linear Predictive Coding (LPC) used to estimate formant frequencies, capturing vocal-tract variations during apnea events.

---

## Methodology

1. PSG audio recordings are divided into **fixed-length (60-second) clips**.  
2. Noise reduction and filtering are applied to isolate snoring-related frequencies.  
3. Relevant audio and signal features are extracted from each clip.  
4. **Unsupervised clustering** (Hierarchical clustering and K-Means) is used to group clips into:
   - Normal breathing  
   - Normal snoring  
   - Apnea-related snoring  
5. Predicted clusters are compared with annotated PSG data to evaluate performance.

---

## Outcome

The results demonstrate that **signal processing combined with machine learning–based clustering** can effectively differentiate apnea-related snoring from normal breathing patterns, highlighting the potential of automated approaches in sleep disorder analysis.

---

## Notes

- This project focuses on **signal processing and classical machine learning**, not end-to-end deep learning.
- It is intended for **research and academic exploration** in biomedical signal analysis.

