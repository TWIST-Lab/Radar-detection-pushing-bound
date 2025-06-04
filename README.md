# Radar Detection and Waveform Identification under High Interference in CBRS Band
This repository offers a modular framework for radar detection and waveform identification in the **Citizens Broadband Radio Service (CBRS)** band, targeting environments with significant interference from commercial systems such as 5G. The repository includes two machine learning-based pipelines, each tailored to different input modalities—**In-phase/Quadrature (IQ)** data and **spectrograms**.

---

## 🔹 Introduction

As spectrum sharing becomes increasingly vital for accommodating commercial wireless growth, ensuring reliable coexistence with incumbent users—such as military radar systems—remains a key challenge. This repository addresses that challenge through two machine learning pipelines designed to detect and classify radar signals in shared-spectrum scenarios with high interference.

The framework is adaptable to various signal types and interference conditions, making it suitable for research and prototyping in **spectrum sharing**, **signal classification**, and **wireless coexistence technologies**.

---

## 🔹 Setup and Prerequisites

### System Requirements
- **Python 3.8+**: [Install Python](https://www.python.org/downloads/)
- **Jupyter Notebook**: [Install Jupyter](https://jupyter.org/install)
- **TensorFlow 2.6+**: [Install TensorFlow](https://www.tensorflow.org/install)

Install additional dependencies listed in the `requirements.txt` file (if available) using:


## 🔹 Pipelines

The repository contains two primary pipelines, each supporting both radar detection and waveform classification.
#### Pipeline 1: IQ-based Radar Detection and Waveform Identification:
This pipeline uses raw IQ samples as input to train and evaluate ML models.
1. **Data Preparation**: Use the provided MILCOM_2025_Data directory for preprocessed IQ data.
2. **Model Training**: Open IQ_ML_For_Detection_and_Identification.ipynb to define, train, and validate the model.
3. **Model Saving and Inference**: Save the trained model and reload it for further evaluation or prediction tasks.
4. **IQ_based Waveform Identification** To perform waveform classification, adjust the output layer (softmax node) to size 6 and use BIN data from the dataset. 

#### Pipeline 2: Spectrogram-based Radar Detection and Waveform Identification:
This pipeline operates on spectrogram representations of radar signals
1. **Preparing Your Data**:Load spectrogram data from the MILCOM_2025_Data directory.
2. **Run the Script**:Run the notebook ML_For_Spec_Radar_Detection_ViT.ipynb directly without modifications.
3. **Model Saving and Inference**: Save the trained model for reuse and load it during inference or evaluation.
4. **Spectogram_based Waveform Identification** Use the notebook Spec_ML_For_Identification.ipynb and the provided BIN data files for classification tasks.


### 🔹 Running the Notebooks
- After setting up either pipeline:
- Launch Jupyter and open the respective notebook.
- Follow the inline instructions to train, save, and evaluate the model.
- Use the trained models to predict or classify new radar signals under interference conditions.

## 🔹 Citation

If this work supports your research, please cite:

```Shafi Ullah Khan, Michel Kulhandjian, and Debashri Roy,“Pushing the Boundaries in CBRS Band: Robust Radar Detection within High 5G Interference,” In IEEE Military Communications Conference (MILCOM), October 2025.```
