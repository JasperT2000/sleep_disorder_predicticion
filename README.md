# sleep_disorder_predicticion
Sleep Disorder Prediction using PPG Sensor Readings
Overview
This project aims to predict sleep stages and identify potential sleep disorders using photoplethysmogram (PPG) sensor recordings. The system involves extracting features from raw PPG signals, analyzing sleep metrics, and using machine learning models for classification.

Deliverables
1. feature_extraction.py
Purpose: This script extracts necessary features from raw PPG sensor recordings. These features are used to predict the sleep stage of an individual.
Features Extracted:
Average peak-to-peak amplitude
Pulse width
Systolic and diastolic areas
Hjorth parameters
Poincare features
Fractal dimensions
Robust statistical features
2. sleep_metrics.py
Purpose: This script computes sleep metrics required to predict whether a person has a sleep disorder.
Metrics Extracted:
Sleep state classification (Awake, REM, NREM stages)
Arousal index
Sleep efficiency and other relevant parameters
3. predict.py
Purpose: This script integrates the feature extraction and sleep metrics, utilizing pre-trained models to predict sleep stages and determine if a person has a sleep disorder.
How it works:
Reads raw PPG data.
Extracts features using feature_extraction.py.
Computes sleep metrics using sleep_metrics.py.
Predicts sleep disorder using the trained models.
4. Models Directory
Path: models/
Contains the machine learning models trained to predict sleep stages and sleep disorders. These models are used in the predict.py script.
5. Jupyter Files
The development and testing of both the feature extraction model (for sleep stage prediction) and the classifier (for sleep disorder detection) are documented in Jupyter notebooks.
The notebooks detail data preprocessing, feature extraction, model training, evaluation, and testing.