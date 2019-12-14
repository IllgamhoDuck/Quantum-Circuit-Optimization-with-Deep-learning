# Quantum-Circuit-Optimization-with-Deep-learning
This is a educational notebook about what is quantum circuit optimization and how to optimize the circuit using deep learning approach created for IBM Q Challenge teach me qiskit award.

https://ibmqawards.com

Recommend reading following chapter at qiskit textbook before you start. 

[QISKIT TESTBOOK](https://community.qiskit.org/textbook/preface.html)

```
chapter 0. Prerequisites
chapter 1. Quantum States and Qubits 
chapter 2. Single Qubits and Multiple-Qubits gates
```
But if you don't want to go through it and just want to directly work on this you can go through directly! Every notebook is created to be possible to implement without prior knowledge of deep learning and quantum computing. But make sure you modify the path appropriatly :D

## Introduction
Currently Quantum computer has a lots of noise inside and circuit optimization is a effort to reduce the noise as small as possible. This is the part of one step to Fault-tolerance Quantum computer. At this notebook we are going to explain the circuit optimization in details and a way to optimize the circuit using deep learning method.

## What is Quantum Circuit Optimization?
`Below phrase is what IBM mentioned`

Optimize circuits to minimize noise when they are executed on a real IBMQ backend, by using the properties of the backends themselves. These properties contain information about the physics of the device, such as qubit lifetimes (decoherence and relaxation), gate and readout error rates, and gate latencies.

## Why deep learning?
Currently quantum circuit optimization is done by qiskit transpiler. It is using graph data structure and using A* search to find the optimized the layout and a way to swap qubits. There is few approach using deep learning model.

We are trying to give a guide line for Deep learning practitioners or quantum computer practitioners to encourage the participate to the circuit optimization using deep learning and to check possibility of the deep learning to quantum circuit optimization and further more. This is why we made a education notebook using deep learning.

## Where to start?
Follow this link to start :D The guide notebook includes following index!

[Guide of this project](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)

`Highly recommended to go through this resource at colab`

#### Index
0. [Welcome :D](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)
1. [What is circuit optimization?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)
2. [How does optimized circuit looks like depends on hardware?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Check_how_circuit_optimized_depends_on_quantum_backend.ipynb)
3. [Check quantum hardware information](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/hardware_information.ipynb)
4. [How to generate random circuit?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Random_quantum_circuit_Generator.ipynb)
5. [Generate dataset for Deep learning](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Generate_dataset.ipynb)
6. [Train LSTM Autoencoder to find circuit manifold](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/LSTM_Autoencoder.ipynb)


6-1. [(Optional) Predicting statevectors from circuits](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/predicting_statevectors_from_circuits.ipynb)

`Check more about the experiment results of this statevector predicting model`
[experiment log](https://docs.google.com/spreadsheets/d/1LPAHmYtP5d9_qKSbEQmxlSk6NTAQU2ytRe82e3c6dVQ/edit)

7. [Train Layout predicting Model](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/layout_prediction.ipynb)
8. [Train Optimized circuit generating model](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Optimized_circuit_generator.ipynbU)
9. [How to check it is optimized?](https://github.com/IllgamhoDuck/Quantum-Circuit-Optimization-with-Deep-learning/blob/master/Quantum_circuit_optimization_with_Deep_learning.ipynb)

A. Future work

## What Deep learning model it is using?
1. LSTM Autoencoder - `Find circuit latent space(manifold)`
2. LSTM Encoder DNN - `Predict the layout`
3. LSTM seq2seq - `Generate Optimized quantum circuit`
4. DNN - (Optional) `Predicting the statevector from circuit`
