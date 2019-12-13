# Quantum-Circuit-Optimization-with-Deep-learning
This is a educational notebook about what is quantum circuit optimization and how to optimize the circuit using deep learning approach created for IBM Q Challenge teach me qiskit award
https://ibmqawards.com

`Highly recommended to go through this resource at colab`
## Index
0. Welcome :D
1. What is circuit optimization?
2. [How does optimized circuit looks like depends on hardware?](https://colab.research.google.com/drive/150ZR9zoIf8XBFpLM9IXAr6rhkSOcScpU)
3. [Check quantum hardware information](https://colab.research.google.com/drive/1m-bRNeopa6mToCv01wy3_LyjQTYZ6Nap)
4. [How to generate random circuit?](https://colab.research.google.com/drive/1AD5sX89YILQTAsL8Go2IOYXSFx_hEIaS)
5. [Generate dataset for Deep learning](https://colab.research.google.com/drive/1n_zwBDY8UyXgpQedz8sHVXAjgYcGwN91)
6. [Train LSTM Autoencoder to find circuit manifold](https://colab.research.google.com/drive/1jcYs0p-XZCoSlnf2j8nwzYeiRKL-aBpJ)
7. [Train Layout predicting Model](https://colab.research.google.com/drive/1EeWubYnIIkIdkq-5XNMZ68WXw9i1SMIc)
8. [Train Optimized circuit generating model](https://colab.research.google.com/drive/1--9oFkHl7efT0fI9s1JkrBE1uwczt3YU)
9. Future work

## Introduction
Currently Quantum computer has a lots of noise inside and circuit optimization is a effort to reduce the noise as small as possible. This is the part of one step to Fault-tolerance Quantum computer. At this notebook we are going to explain the circuit optimization in details and a way to optimize the circuit using deep learning method.

## Why deep learning?
Currently quantum circuit optimization is done by qiskit transpiler. It is using graph data structure and using A* search to find the optimized the layout and a way to swap qubits. There is few approach using deep learning model. Deep learning approach was used to check the possibility of the deep learning to quantum circuit optimization and further more.

## Where to start?
Follow this link to start :D
[Guide of this project](https://colab.research.google.com/drive/1PRtKv2vY2yKl4pDYQ9M2kcpkQ0lvdJnM)

## What Deep learning model it is using?
1. LSTM Autoencoder - `Find circuit manifold`
2. LSTM Encoder DNN - `Predict the layout`
3. LSTM seq2seq - `Generate Optimized quantum circuit`
