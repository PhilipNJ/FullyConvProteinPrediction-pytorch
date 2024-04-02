# Deep Learning for Protein Secondary Structure Prediction

## Overview
This project is part of a Deep Learning course coursework, focused on predicting the secondary structure of proteins using Fully Convolutional PyTorch models. Protein secondary structure prediction is a crucial task in bioinformatics, aiding in understanding protein functions and interactions. This repository contains the Jupyter notebook detailing the entire development process, from data preprocessing to model implementation and evaluation.

## Project Setup
The project was developed as part of a Kaggle competition, specifically designed for the Deep Learning course. 

### Data
The dataset comprises protein sequence data (Protein Primary Structure) and Position-Specific Scoring Matrix (PSSM) profiles, aimed at predicting protein secondary structures classified into Helix (H), Extended Sheet (E), and Coil (C). The data is sourced from the Protein Data Bank (PDB), featuring over 200,000 proteins with unique PDB_ID codes.

### Development Environment
The project leverages Kaggle Notebooks, facilitating direct access to competition data and GPU/TPU resources for model training and evaluation. This choice was made to familiarize participants with another Jupyter Notebook system and to manage large datasets efficiently.

## Project Components

### 1. Data Processing
A custom data loader was developed for handling PDB ID CSV data and PSSM data, similar to approaches discussed in lab sessions. This component is crucial for preparing the dataset for the model.

### 2. Convolutional Neural Network (CNN) Model
The core of this project is a Fully Convolutional PyTorch model designed to input tensor representations of protein sequences or PSSM profiles and output a tensor of secondary structure labels. This approach mirrors image segmentation techniques but applied to sequence data.

### 3. Hyperparameter Tuning
The project employs Ray Tune for hyperparameter optimization, balancing the need for model efficiency with the constraints of limited Kaggle GPU/TPU resources. This step is vital for achieving optimal model performance.

### 4. Model Training and Validation
The training process includes generating loss and accuracy curves to monitor and diagnose model performance. Validation datasets are used to evaluate model efficiency, adhering to the machine learning workflow concepts emphasized in the course.

### 5. Test Implementation
Finally, the model is tested on unseen data, with predictions submitted to the Kaggle competition for evaluation against peers. This phase is critical for assessing the model's generalizability and performance in real-world scenarios.

## Conclusion and Future Work
This project encapsulates the application of deep learning techniques in bioinformatics, with a specific focus on protein secondary structure prediction. The development process, from data preprocessing to model evaluation, underscores the potential of Fully Convolutional Networks in sequence data analysis. Future work may explore the integration of additional data types and the application of more advanced model architectures to further enhance prediction accuracy.
