# Affective Computing-Facial-Expression-Analysis

## Description:

This project focuses on building a speech emotion recognition system. The system extracts prosodic correlates and cepstral features from speech recordings, and then classifies emotions using a supervised SVM classifier.

## Dataset:

- Simulated emotional speech data (acted) from ten speakers.
- Five different pre-segmented sentences of roughly 2-3 seconds each.
- Two emotional states: happy and sad.
- Total of 100 samples.

## Features:
- Prosodic features:
  - Intensity/Energy parameters (mean, standard deviation, percentiles, kurtosis)
  - Pitch/F0 features (mean, standard deviation, percentiles, kurtosis)
  - Rhythm/Durations parameters (voiced/unvoiced segment lengths, voicing ratio)

- Cepstral features:
  - Mel-Frequency Cepstral Coefficients (MFCCs)

## Methodology:
### 1. Preprocessing:
 - Downsample speech signal to 11.025 kHz.
 - Pre-emphasize the signal.

### 2. Feature Extraction:
 - Calculate MFCC features.
 - Extract intensity/energy parameters.
 - Extract pitch/F0 features
 - Extract rhythm/durations parameters.

### 3. Classification:
 - Train SVM classifiers using prosodic and MFCC features.
 - Test classifiers on training and testing data.
 - Evaluate performance using accuracy, confusion matrices, and other metrics.

### Libraries:
   - NumPy
   - SciPy
   - Matplotlib
   - Python Speech Features
   - Scikit-Learn
   - Seaborn

### Usage:
   - Clone the repository.
   - Install required libraries using pip install -r requirements.txt.
   - Run the Jupyter Notebook (Exercise 2_Md Rabiul_Hasan_2410234.ipynb).

## Results:
### Performance
   - Reported classification accuracies for training and testing data using both prosodic and MFCC features.
   - Analyzed confusion matrices to understand classification errors.
