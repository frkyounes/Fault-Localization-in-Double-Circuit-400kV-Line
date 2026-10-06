# Fault Detection, Classification and Localization in a 400 kV Double-Circuit Transmission Line

## Overview
This project presents the development of an intelligent system for the detection, classification, and localization of electrical faults in a 400 kV double-circuit transmission line.

The system is developed and simulated using MATLAB/Simulink and Artificial Neural Networks (ANNs).

The study focuses on the challenges associated with fault analysis in double-circuit transmission lines, particularly the influence of mutual coupling between the two circuits.

![Simulink Model](image.png)

## Integrated Protection System

The three ANN models are integrated into a unified MATLAB/Simulink protection system for fault detection, classification, and localization.

![Integrated Protection System](images/Figure%204.19%20.png)

## System Description

The simulated transmission system is characterized by:

* Voltage level: 400 kV
* Frequency: 50 Hz
* Transmission line length: 100 km
* Configuration: Double-circuit transmission line
* Simulation environment: MATLAB/Simulink
* Intelligent technique: Artificial Neural Networks (ANNs)

## Objectives

The main objectives of the project are:

* Detect the occurrence of an electrical fault.
* Classify the type of fault.
* Identify the affected transmission circuit.
* Estimate the location of the fault along the transmission line.
* Develop an intelligent approach based on Artificial Neural Networks.

## Methodology

The project follows the following general approach:

1. Modeling of the 400 kV double-circuit transmission line in MATLAB/Simulink.
2. Generation of different fault scenarios.
3. Acquisition and processing of electrical signals.
4. Development of a database representing different fault conditions.
5. Training of Artificial Neural Network models.
6. Fault detection.
7. Fault classification.
8. Fault localization.
9. Analysis of the obtained results.
## Neural Network Models

Three neural network models are used in the project:

- **Fault Detector** – detects the presence of a fault and identifies the affected circuit.
- **Fault Classifier** – identifies the fault type.
- **Fault Localizer** – estimates the fault distance along the transmission line.

## Key Results

The three ANN models achieved strong performance on the simulated dataset:

- **Fault Detector:** 12-20-10-2 architecture, validation MSE of `1.885 × 10⁻⁶`, with `R = 1.000` on validation and test data.
- **Fault Classifier:** 12-40-20-10 architecture, validation MSE of `1.247 × 10⁻⁵`, with `R = 0.99992` on validation data.
- **Fault Localizer:** 12-50-25-10-1 architecture, validation MSE of `0.317 km²`, with `R = 0.99978` on validation data.

The integrated system was also evaluated on representative fault scenarios. The majority of estimated fault locations showed an error below 1 km.

### Simulink Model

`PFE_2Lignes_RNA (2).slx`

Main MATLAB/Simulink model used for the electrical system and fault simulations.

### Neural Network Models

The trained neural network models are provided as MATLAB `.mat` files:

- `RNA_Detecteur_100km (3).mat`
- `RNA_Classificateur_100km (3).mat`
- `RNA_Localisateur_100km (3).mat`

## Tools and Technologies

* MATLAB
* Simulink
* Artificial Neural Networks
* Power System Modeling
* Electrical Fault Analysis
* Transmission Line Protection

## Project Context

This work was carried out as a Final-Year Engineering Project in Electrical Engineering, with a specialization in Electrical Networks.

The project combines electrical power system modeling, protection, fault analysis, signal processing, and artificial intelligence.

## Future Improvements

Possible future developments include:

* Testing the models under a wider range of operating conditions.
* Improving fault localization accuracy.
* Evaluating the influence of measurement noise.
* Testing the approach on more complex network configurations.
* Exploring other machine learning and deep learning techniques.

## Author

**Younes Ferkous**

Electrical Engineering – Electrical Networks
