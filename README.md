# Quantum-Circuit-Optimization-with-Deep-learning
This is a collection of educational notebooks about what is quantum circuit optimization and how to optimize quantum circuits using deep learning, created for the IBM Q Challenge: Teach Me Qiskit Award.

![IBMQ](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/img/IBMQ.png?raw=true)

https://ibmqawards.com

Recommend reading following chapter of the Qiskit textbook before you start. 

[QISKIT TESTBOOK](https://community.qiskit.org/textbook/preface.html)

```
Chapter 0. Prerequisites
Chapter 1. Quantum States and Qubits 
Chapter 2. Single Qubits and Multiple-Qubits gates
```
But if you don't want to go through it and just want to directly work on this you can go through directly! Every notebook is created to be possible to implement without prior knowledge of deep learning and quantum computing. But make sure you modify the path appropriatly :D

## Introduction
Currently quantum computers have a lot of noise. Circuit optimization is an effort to reduce the statevector error (the difference between the actual statevector from the ideal statevector) caused by noise as much as possible. This is a step towards fault tolerant quantum computing. These notebooks explain circuit optimization in detail and a way to optimize quantum circuits using deep learning.

## What is Quantum Circuit Optimization?
[Quote](https://ibmqawards.com/developer-challenge-circuit-optimization/) from IBM:

`Optimize circuits to minimize noise when they are executed on a real IBMQ backend, by using the properties of the backends themselves. These properties contain information about the physics of the device, such as qubit lifetimes (decoherence and relaxation), gate and readout error rates, and gate latencies.`

## Why deep learning?
Currently, quantum circuit optimization is done by the Qiskit transpiler. It uses a graph data structure and A* search to find the optimized layout and a way to swap qubits. Few approaches use deep learning.

We made this series of educational notebooks using deep learning to provide a guideline for Deep Learning and Quantum Computing practitioners and to validate and encourage the use of deep learning to optimize quantum circuits.

## Where to start?
Click the guide link to start :D The guide notebook includes all of the informations you need! You can search one by one using the below.

[Guide of this project](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)

`Highly recommended to go through these resources through the Google Colaboratory interface because they are designed for use through that interface` [Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb)

#### Index
0. [Welcome :D](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)
1. [What is circuit optimization?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)
2. [How does optimized circuit looks like depends on hardware?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Check_how_circuit_optimized_depends_on_quantum_backend.ipynb)
3. [Check quantum hardware information](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/hardware_information.ipynb)
4. [How to generate random circuit?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Random_quantum_circuit_Generator.ipynb)
5. [Generate dataset for Deep learning](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Generate_dataset.ipynb)
6. [Train LSTM Autoencoder to find circuit manifold](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/LSTM_Autoencoder.ipynb)


6-1. [(Optional) Predicting statevectors from circuits](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/predicting_statevectors_from_circuits.ipynb)

`Check out our experiment log showing results from many experiments we ran to validate this statevector prediction model`
[experiment log](https://docs.google.com/spreadsheets/d/1LPAHmYtP5d9_qKSbEQmxlSk6NTAQU2ytRe82e3c6dVQ/edit)

7. [Train Layout predicting Model](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/layout_prediction.ipynb)
8. [Train Optimized circuit predicting model](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Optimized_circuit_generator.ipynb)
9. [How to check it is optimized?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)

## What Deep learning model is used?
1. LSTM Autoencoder - `Find circuit latent space(manifold)`
2. LSTM Encoder DNN - `Predict the layout`
3. LSTM seq2seq - `Predict transpiler level 3 Optimized quantum circuit`
4. DNN - (Optional) `Predicting the statevector from circuit`
