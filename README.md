# Machine Learning for Higgs Boson Detection ⚛️🚀

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)
[![Nadam](https://img.shields.io/badge/Optimizer-Nadam-brightgreen.svg)](https://keras.io/api/optimizers/nadam/)
[![FocalLoss](https://img.shields.io/badge/Loss-BinaryFocalCrossentropy-blue.svg)](https://keras.io/api/losses/probabilistic_losses/#binaryfocalcrossentropy-class)

A specialized investigation into **b-quark tagging** for the detection of Higgs boson decay products. This project bridges the gap between traditional **High-Energy Physics (HEP)** analysis and modern **Deep Learning**, achieving significant gains in signal sensitivity.

---

## 📈 Performance Summary

The core objective was to maximize **Signal Sensitivity** against massive background noise. Our Machine Learning approach significantly outperformed the standard physical cut-based baseline.

| Method | Signal Sensitivity | Improvement |
| :--- | :---: | :---: |
| **Traditional Cut-Based Analysis** | 1.863 | Baseline |
| **Deep Neural Network (Proposed)** | **2.767** | **+48.5%** 🚀 |

---

## 🧠 Methodology & Architecture

### 1. Physics-Informed Pre-processing
- **Feature Selection**: Removed constant discriminants (`nJ`, `nTags`) to reduce model bias.
- **Normalization**: Standard scaling to ensure equitable influence across multi-scale kinematic features.

### 2. Deep Neural Network Design
A fully connected feed-forward network optimized for binary classification in HEP:
- **Architecture**: Input Layer → 4 Hidden Layers (ReLU) → Sigmoid Output.
- **Advanced Loss**: Utilizes `BinaryFocalCrossentropy` to address class imbalance between signal and background events.
- **Optimizer**: `Nadam` with a learning rate of 0.005 for faster convergence.

---

## 📂 Repository Structure

*   `Higgs-Cutbased selection (1).ipynb`: Implementation of the baseline physical cut logic.
*   `Higgs-Machine Learning (1).ipynb`: Full ML pipeline: Pre-processing, Training, and Evaluation.
*   `nn/`: Hyperparameter search logs (layers, nodes, learning rates).
*   `b4 cut.png` / `after cut.png`: Mass distribution ($m_{BB}$) visualizations.

---

## 🛠 Getting Started

### Installation
```bash
git clone https://github.com/Chenypovo/Machine-Learning-in-Higgs-Boson-Detection.git
cd Machine-Learning-in-Higgs-Boson-Detection
pip install -r requirements.txt
```

### Reproducing Results
1.  **Baseline**: Run `Higgs-Cutbased selection (1).ipynb` to establish the 1.863 sensitivity benchmark.
2.  **ML Training**: Run `Higgs-Machine Learning (1).ipynb` to train the neural network and verify the 48.5% improvement.

---

## 📧 Contact
Developed by **YiPeng Chen**. 
Specializing in the intersection of **Physics** and **Artificial Intelligence**.
- **Contact**: yipeng003@e.ntu.edu.sg
