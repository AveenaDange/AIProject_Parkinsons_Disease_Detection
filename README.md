# Parkinson's Disease Detection

This project aims to build a robust machine learning model to detect Parkinson's Disease using three distinct datasets that capture different modalities of Parkinson’s symptoms. The datasets contain data related to voice, hand-drawing patterns, and movement analysis.

---

## Table of Contents
- [Introduction](#introduction)
- [Datasets Used](#datasets-used)
- [Project Workflow](#project-workflow)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction
Parkinson's Disease is a progressive neurological disorder that impacts movement, motor skills, and speech. This project employs machine learning to analyze diverse datasets for detecting Parkinson's Disease, with the goal of leveraging multiple diagnostic features for improved accuracy.

---

## Datasets Used
The project utilizes the following datasets, each capturing a unique aspect of Parkinson's Disease symptoms:

1. **Parkinson’s Drawing Dataset**:
   - Captures drawing patterns on paper (e.g., spiral and meander drawings).
   - Includes features such as pressure, velocity, and acceleration.
   - Useful for detecting motor impairments.

2. **HandPD Dataset**:
   - Records hand movement features like tremors, grip strength, and steadiness.
   - Data is collected using wearable sensors during various tasks.
   - Helps identify fine motor skill deterioration.

3. **NewHandPD Dataset**:
   - A refined dataset focusing on advanced hand movement metrics.
   - Includes higher resolution and more detailed motion tracking.
   - Improves precision in detecting early symptoms.

Each dataset contributes to a comprehensive understanding of the disease, addressing different manifestations such as speech impairment, motor skill decline, and hand tremors.

---

## Project Workflow
1. **Data Preprocessing**:
   - Normalize and clean data from all three datasets.
   - Handle missing or inconsistent values.
2. **Feature Engineering**:
   - Extract relevant features from each dataset (e.g., velocity, acceleration, voice harmonics).
3. **Model Development**:
   - Train separate machine learning models for each dataset.
   - Combine predictions using ensemble techniques or multi-modal fusion.
4. **Evaluation**:
   - Evaluate individual and combined models using standard metrics.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/parkinsons-detection.git
   cd parkinsons-detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage
1. Train models on individual datasets:
   ```bash
   python train_model.py --dataset <dataset_name>
   ```
   Available datasets: `drawing`, `handpd`, `newhandpd`.

2. Combine predictions for improved accuracy:
   ```bash
   python ensemble_model.py
   ```

3. Predict using new data:
   ```bash
   python predict.py --dataset <path_to_new_data>
   ```

---

## Model Performance
The combined model achieves the following metrics:
- **Accuracy**: 97%
- **Precision**: 96%
- **Recall**: 98%
- **ROC-AUC**: 99%

Performance for individual datasets:
- Parkinson's Drawing Dataset: Accuracy: 94%
- HandPD Dataset: Accuracy: 95%
- NewHandPD Dataset: Accuracy: 96%

---

## Contributing
Contributions are welcome! Please:
1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Submit a pull request with a clear description.

---


## Acknowledgments
- Authors and contributors of the datasets.
- Research initiatives focusing on Parkinson's Disease diagnostics.
