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
