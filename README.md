# 🧠 Classifying Schizophrenia through EEG Recordings

## Project Overview

Schizophrenia affects cognitive processing, and understanding its neural mechanisms remains a challenge. This project analyzes EEG signals to differentiate between individuals with schizophrenia and healthy controls by examining corollary discharge disruptions. By training a machine learning model on real patient data, we aim to develop a more effective approach for identifying neural abnormalities associated with schizophrenia, improving early diagnosis and potential treatment strategies.

## Dataset

The dataset includes EEG recordings from 81 subjects, consisting of:
- 36 patients diagnosed with schizophrenia
- 22 control subjects
- Additional 10 controls & 13 schizophrenia patients from a previous study

Link: https://www.kaggle.com/datasets/broach/button-tone-sz

### Data Collection

- EEG data were recorded during a button-pressing task designed to study corollary discharge mechanisms.
- Recordings include event-related potential (ERP) data from 9 key electrode sites:
  - Fz, FCz, Cz, FC3, FC4, C3, C4, CP3, CP4
- Preprocessing steps:
  - Filtering
  - Baseline correction
  - Artifact removal
  - Independent Component Analysis (ICA)
- Single-trial data from 24 subjects, containing detailed 64-channel preprocessed EEG signals.

## Methods

### EEG Data Preprocessing
- Clean and filter EEG signals.
- Remove artifacts and segment data into meaningful trials.

### Feature Selection
- Extract relevant EEG features from event-related potentials (ERPs) across key electrode sites.

### Model Training
- Train machine learning models to distinguish between schizophrenia patients and healthy controls.
- Approaches Used:
  - Linear SVM Classifier
  - ANOVA for feature selection
  - Relative voltage differences
  - Spatial difference calculations
  - Independent Component Analysis (ICA)

### Model Evaluation
- Accuracy
- Precision
- Recall


## Results
Classification accuracy: 88%

Feature importance rankings: ['Fz', 'Cz', 'FCz', 'C3', 'C4', 'CP3', 'CP4']
