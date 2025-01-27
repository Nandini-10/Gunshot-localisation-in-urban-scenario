# Gunshot Localization in Urban Reflective Scenarios

## Overview

This project focuses on gunshot localization in urban environments, addressing the challenges posed by multipath propagation where acoustic signals reflect off surfaces, leading to signal delays and distortions. The work explores various methods, including trilateration, linear regression, and convolutional neural networks (CNNs), to improve localization accuracy. The project also leverages the **Zenodo Gunshot/Gunfire Dataset** to evaluate the model's performance in real-world conditions.

## Project Structure

The repository contains the following files:

- **'DDP1_report.pdf`** - Detailed report covering the project's objectives, methodology, experiments, and findings.
- **`DDP_classify.ipynb`** - Jupyter Notebook for firearm classification using machine learning techniques.
- **`DDP.ipynb`** - Jupyter Notebook implementing gunshot localization techniques using trilateration and machine learning models.
- **`R&D.ipynb`** - Jupyter Notebook for exploratory research and additional analysis on the dataset.

---

## Methodology

### 1. Gunshot Signatures
Gunshot events are characterized by two main components:
- **Muzzle Blast:** The explosive sound wave propagating at the speed of sound.
- **Ballistic Shockwave:** Generated when the bullet speed exceeds the speed of sound.

### 2. Source Localization Approaches
#### a) Trilateration-Based Localization
- Utilizes an array of sensors to estimate the gunshot source location by solving time delay equations.
- Groups sensors and multipath reflections to improve localization accuracy.
- Simulations conducted with different sensor placements to evaluate performance.

#### b) Machine Learning-Based Approaches
**Linear Regression Model**
- Uses sensor positions and multipath data to estimate gunshot source location.
- Evaluated using Root Mean Square Error (RMSE) and Mean Absolute Error (MAE).

**Convolutional Neural Network (CNN) Model**
- Designed to enhance robustness in complex urban environments.
- Extracts spatio-temporal patterns from gunshot spectrograms.
- Evaluated using RMSE and R² scores.

### 3. Model Testing on Real Dataset
- **Zenodo Gunshot Dataset:** A real-world dataset with gunshot recordings collected in outdoor environments under various conditions.
- Models were trained and tested using the dataset, and their accuracy in localization and firearm classification was assessed.

---

## Installation & Setup

To run the project, ensure you have the following dependencies installed:

```bash
pip install numpy pandas matplotlib librosa scikit-learn tensorflow
