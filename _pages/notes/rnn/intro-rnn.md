---
layout: post
title: Introduction to recurrent neural networks
#date: 2022-01-01 00:00:00-0000
#description: Taking apart vanilla RNN
---
---
#### Contents



#### Introduction

In this post, a recurrent neural network in its basic form is presented for an absolute beginner such as me. Let's try and answer the question -- "What is the difference between neural networks and deep learning?"

###### ___neural networks and deep learning___

Neural networks or Artificial Neural Networks are set of algorithms that try to loosely emulate the biological brain. They consist of nodes or neurons interconnected with one another; each connection having an associated weight and each node having a nonlinear function called activation function. A given neural network architecture then specifies number of nodes or neurons, the interconnections with their weights, type of activation function in neurons and number of inputs and outputs.


Deep learning is then set of algorithms used to learn the weights, given a NN architecture and training data. It also includes choices such as number of nodes, interconnections between then and number of layers, given a particular problem. This choice leads to many architectures and this post deals with a a particular form called the Recurrent Neural Networks.


RNNs are meant for sequential data, such as time series data which have dependencies on the previous state. This is equivalent to dynamical systems which control engineers are acquainted. There exists hidden state in the cell of a NN, which is propagated to the next cell. The function of this hidden state equivalent to the function of "state" in the context of control systems.

Makes me wonder if RNN's can be used in conjunction with state space models?



#### References

1. Andrej Karpathy's blog post titled ["The Unreasonable Effectiveness of Recurrent Neural Networks"](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
