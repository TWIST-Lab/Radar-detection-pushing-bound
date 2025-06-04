# Radar Detection and Waveform Identification under High Interference in CBRS Band
This repository facilitates the detection of radar and waveform identification within the CBRS band using two pipelines.
## Introduction
This repository provides a flexible framework for signal detection and classification in shared-spectrum environments such as the Citizens Broadband Radio Service (CBRS) band. It focuses on enabling coexistence between commercial wireless systems, like 5G, and incumbent users, such as military radar systems. Using machine learning-based approaches, the code supports reliable detection and identification of signals under challenging interference conditions. It is adaptable to various signal types and can be extended to handle different detection tasks and interference scenarios, making it suitable for research and development in spectrum sharing and coexistence technologies.

## Setup and Prerequisites
## Prerequisites

Before running the signal detection code, make sure you have the following installed:

- **Python 3.8 or higher**  
  Download from the official [Python website](https://www.python.org/downloads/).

- **Jupyter Kernel**  
  Install Jupyter by following the instructions on the [Jupyter website](https://jupyter.org/install).

- **TensorFlow 2.6 or higher**  
  Install TensorFlow via pip by following the instructions on the [TensorFlow website](https://www.tensorflow.org/install).

Additionally, make sure to install any other dependencies as mentioned in the project.


## Getting Started

To get started with the project, you have two pipelines nnamely Pipeline 1  and Pipeline 2:
#### Pipeline 1: IQ_based Radar Detection and Waveform Identification.
1. **Prepare your data**: Make sure your data is properly preprocessed and formatted, yopu can use the data from the files named MILCOM_2025_Data here in the repository.
2. **Train the Model**: Train the individual model named "IQ_ML_For_Detection_and_Identification.ipynb" from scratch using the provided data. This will involve setting up the architecture and running the training process.
3. **Save the Model**: Once the training is complete, save the trained model to a directory for future use.
4. **Load the Model**: When you are ready to use the model, load it from the saved directory for further evaluation or inference.
5. **ForIQ-based Waveform Identification** You can use the same model change the output node of the softmax to 6 and use the any of the BIN data from the repository. 

#### Pipeline 2: Spectogram_based Radar Detection.
1. **Preparing Your Data**:Make sure your data is properly preprocessed and formatted, yopu can use the data from the files named MILCOM_2025_Data here in the repository.
2. **Run the Script**:Load the Spectogram data from the provided data and and run the script "ML_For_Spec_Radar_Detection_ViT.ipynb" with out any changes.
3. **Save the Model**: Once the training is complete, save the trained model to a directory for future use.
4. **Load Model**: When you are ready to use the model, load it from the saved directory for further evaluation or inference.
**For Spectogram_based Waveform Identification** USe  use the script "Spec_ML_For_Identification.ipynb" and use teh BIN data from the repository. 


### Running the Script
- After completing either of the two options above, you can run the Python script using the provided Jupyter notebooks. These allows you to interact with the model, make predictions, or evaluate its performance on new data.

By following these steps, you can either build/use the IQ-based model or take advantage of Spectogram_based model for improved results, depending on your specific needs.


## Cite

If you find this radar detection approach useful in your research, please cite our work:
