# EEG_Signal_Classification

This repository contains the code and data for a preliminary classification of EEG signals using Convolutional Neural Networks (CNN) on scalograms and spectrograms. The project involves analyzing electroencephalographic (EEG) time series data, including surface EEG recordings from healthy volunteers and intracranial EEG recordings from epilepsy patients.

## Overview

The goal of this project is to classify EEG signals using Convolutional Neural Networks (CNN) based on features extracted from Continuous Wavelet Transform (CWT) and Short Time Fourier Transform (STFT) on the raw EEG signal. The project focuses on classifying different EEG conditions such as eyes closed, eyes open, and epileptic seizures.

## Feature Extraction

The raw EEG signals were preprocessed and transformed into feature representations using the following methods:

1. **Filtering:** A 6th order Butterworth 0.53–40 Hz bandpass filter was applied to the raw EEG signals to remove noise and retain relevant frequency components.

2. **Transformation:** Raw EEG signals were transformed into feature representations using the following methods:
   - Continuous Wavelet Transform (CWT): Scalograms were generated from the EEG signals to capture time-frequency features.
   - Short Time Fourier Transform (STFT): Spectrograms were computed to represent frequency content over time.

## Data

The dataset used in this project consists of five sets, each containing 100 single-channel EEG segments of 23.6 seconds duration. The data includes:

- Surface EEG recordings from healthy volunteers with eyes closed and eyes open.
- Intracranial EEG recordings from epilepsy patients during the seizure-free interval from within and from outside the seizure generating area.
- Intracranial EEG recordings of epileptic seizures.

## Approach

1. Data Preprocessing: Raw EEG signals are filtered and transformed into feature representations (scalograms and spectrograms).
2. Convolutional Neural Network (CNN): CNN models are trained on the extracted features to perform EEG signal classification.
3. Evaluation: The trained CNN model is evaluated using accuracy as the performance metric.

## Results

- The trained model achieved an accuracy of 90% using scalograms for classification.
- The trained model achieved an accuracy of 94% using spectrograms for classification.