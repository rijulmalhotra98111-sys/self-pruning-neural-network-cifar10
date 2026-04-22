# Repository Name

`self-pruning-neural-network-cifar10`

---

# Repository Description

A PyTorch-based implementation of a self-pruning neural network trained on CIFAR-10 using learnable gating mechanisms and sparsity regularization. The project demonstrates dynamic neuron pruning, adaptive sparsity control, and efficient model compression techniques.

---

# README.md

```markdown
# Self-Pruning Neural Network on CIFAR-10

A PyTorch implementation of a **Self-Pruning Neural Network** that dynamically learns sparse connections during training using learnable gates and sparsity regularization.

The model is trained on the CIFAR-10 dataset and demonstrates how neural networks can automatically reduce unnecessary parameters while maintaining competitive accuracy.

---

## Features

- Dynamic self-pruning architecture
- Learnable gating mechanism for neurons/weights
- Sparsity regularization using L1 penalty
- CIFAR-10 image classification
- Automatic sparsity measurement
- Cosine Annealing learning rate scheduler
- Warmup training strategy
- GPU acceleration support (CUDA)
- Visualization of learned gate distributions

---

## Tech Stack

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib

---

## Project Structure

```

.
├── Case_Study_Tredence.ipynb
├── requirements.txt
├── .gitignore
└── README.md

````

---

## Model Overview

The project implements:

- `PrunableLinear` layer with learnable gate scores
- `SelfPruningNet` fully connected architecture
- L1 sparsity regularization
- Adaptive pruning during training

### Architecture

```text
Input (32×32×3)
      ↓
FC Layer (512)
      ↓
FC Layer (256)
      ↓
FC Layer (128)
      ↓
Output Layer (10 classes)
````

---

## Dataset

The model is trained on the CIFAR-10 dataset containing:

* 60,000 color images
* 10 object classes
* Image size: 32×32

Classes:

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/self-pruning-neural-network-cifar10.git
cd self-pruning-neural-network-cifar10
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Case_Study_Tredence.ipynb
```

Run all cells to:

* Train the model
* Apply sparsity regularization
* Evaluate performance
* Visualize gate distributions

---

## Training Details

### Optimizer

* Adam Optimizer
* Separate learning rates for:

  * Network weights
  * Gate scores

### Scheduler

* Cosine Annealing LR Scheduler

### Regularization

* L1 sparsity penalty on gate scores

### Warmup

* Initial warmup epochs without sparsity penalty

---

## Results

The project evaluates:

* Test Accuracy
* Sparsity Percentage
* Gate Distribution
* Tradeoff between sparsity and performance

---

## Future Improvements

* Convolutional self-pruning architecture
* Structured channel pruning
* FPGA deployment optimization
* Quantization support
* Real-time inference benchmarking

---

## Applications

* Efficient AI systems
* Edge AI deployment
* FPGA/Embedded AI acceleration
* Model compression research
* Low-power inference systems

---

## Author

Rijul Malhotra

---

## License

This project is for educational and research purposes.

````

---
