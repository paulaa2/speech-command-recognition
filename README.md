# Speech Command Recognition & Audio Processing

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen.svg)]()
[![Topic](https://img.shields.io/badge/Topic-Speech_Processing_%26_Audio_ML-purple.svg)]()

A practical implementation covering **audio data preprocessing**, **feature extraction**, and **speech command similarity detection** using digital signal processing (DSP) techniques studied in the Voice and Dialogue Processing (TVD) course.

---

## Project Overview

This project explores the fundamentals of audio processing for speech recognition applications. It progresses from synthetic audio signals to real-world recordings, applying state-of-the-art preprocessing pipelines and implementing a similarity-based audio comparison algorithm.

### Key Learning Areas

1. **Synthetic Audio Analysis**: Working with artificially generated audio signals to understand fundamental concepts (sampling rate, Fourier transforms, spectrograms).
2. **Real Audio Preprocessing**: Applying the same pipeline to real speech recordings — filtering, framing, windowing, and normalization.
3. **Audio Similarity Algorithm**: Building a system to compare audio clips and measure their acoustic similarity using:
   - **MFCCs** (Mel-Frequency Cepstral Coefficients)
   - **DTW** (Dynamic Time Warping) for temporal alignment
   - Spectral features (zero crossing rate, spectral centroid, etc.)

---

## Repository Structure

```
speech-command-recognition/
├── P3_resuelta.ipynb     # Main notebook: exercises, implementation & experiments
├── recordings.tar.gz     # Archive of audio recordings used for experiments
└── submission.csv        # Model predictions / competition submission file
```

---

## Audio Processing Pipeline

```
Raw Audio (.wav)
     |
     v
Pre-emphasis Filter
     |
     v
Frame Segmentation (windowing)
     |
     v
FFT / Short-Time Fourier Transform (STFT)
     |
     v
Mel Filter Bank
     |
     v
MFCC Feature Extraction
     |
     v
Similarity / Classification
```

---

## How to Run

1. Extract recordings:
   ```bash
   tar -xzf recordings.tar.gz
   ```
2. Open the notebook:
   ```bash
   jupyter notebook P3_resuelta.ipynb
   ```

---

## Authors & License

Developed as part of the **Voice and Dialogue Processing (TVD)** course at GIA.
Distributed under the **MIT License**.
