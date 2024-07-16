# FamilySeatingArrangementWavenet

This repository contains a project that leverages Wavenet technology to optimize family seating arrangements. The goal is to arrange individuals in a way that maximizes compatibility and minimizes conflicts.

<div align="center">
    <img width="80%" src="https://github.com/faezeh-gholamrezaie/FamilySeatingArrangementWavenet/blob/main/Wavenet_Seating_arrangement.png">
</div>

Project Overview
In this project, we start by generating 400 random names for individuals, including both first names and surnames. These individuals are then organized into 80 groups of 5, ensuring each group is contiguous.

To simulate seating arrangements, we create differences between individuals, ensuring that individuals within the same group have zero differences. A difference matrix is constructed where individuals with differences are marked with a value of 1.

For dataset creation, we prioritize compatible groups first, followed by incompatible groups.

Model Architecture
The seating arrangement model is implemented with the following layers:

- Input Layer
- Linear Layer
- Batch Normalization (BatchNorm1d)
- Tanh Activation Function
- Embedding Layer
- Flatten Consecutive Layer
- Output Layer
  
This architecture is designed to process the generated data and optimize the seating arrangements effectively.

## Causal Convolution

A Causal Convolution is a type of convolution used in neural networks for sequential data processing. It ensures that the output at a given time step depends only on the current and previous time steps, preserving the temporal order of data. This is crucial for tasks like time series forecasting and autoregressive models, where future inputs should not influence the current output.

## Dilated Convolution

A Dilated Convolution is a type of convolution that uses a dilation factor to increase the receptive field of the filter without increasing the number of parameters or the amount of computation. This allows the network to capture wider context in the input data, which is particularly useful for tasks requiring long-range dependencies, such as image segmentation and time series analysis.

Imagine you are looking at a very large picture with a magnifying glass. Standard convolutions are like moving the magnifying glass slowly and step-by-step over the picture, seeing only a small piece of the image at a time.

Now, dilated convolutions are like holding the magnifying glass a bit higher above the picture each time, allowing you to see larger sections of the image together while still noticing the details. This helps you view a bigger part of the picture in less time without losing the quality of the details.

This way, you can observe both small and large parts of the picture effectively. That's exactly what dilated convolutions do; they help the model process data on a larger scale with more detail.

## Residuals

Residuals in a statistical or machine learning model are the differences between observed and predicted values of data. They are a diagnostic measure used when assessing the quality of a model. They are also known as errors.

## Skip Connections

Skip Connections (or Shortcut Connections) as the name suggests skips some of the layers in the neural network and feeds the output of one layer as the input to the next layers. 

## Understanding the Naming and Architecture of the File
The reason this file is named "CNN" but implements the WaveNet architecture is that WaveNet also utilizes convolution techniques. In fact, WaveNet is a type of convolutional neural network that uses dilated convolutions instead of standard convolutions.

# Resource 

https://github.com/karpathy/nn-zero-to-hero/blob/master/lectures/makemore/makemore_part5_cnn1.ipynb
