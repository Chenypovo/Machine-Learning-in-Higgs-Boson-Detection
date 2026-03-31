# Machine Learning for Higgs Boson Detection ⚛️

**Deep learning approach for b-quark tagging in Higgs boson decay analysis**

This project bridges High-Energy Physics (HEP) analysis with modern Deep Learning, achieving significant improvements in signal sensitivity over traditional cut-based methods.

---

## 📊 Results

| Method | Signal Sensitivity | Improvement |
| :--- | :---: | :---: |
| **Traditional Cut-Based** | 1.863 | Baseline |
| **Deep Neural Network** | **2.767** | **+48.5%** |

---

## 🧠 Methodology

### Pre-processing
- **Feature Selection**: Removed constant discriminants (nJ, nTags) to reduce model bias
- **Normalization**: Standard scaling for multi-scale kinematic features

### Network Architecture
- Fully connected feed-forward network for binary classification
- 4 hidden layers with ReLU activation
- Sigmoid output layer
- **Loss**: BinaryFocalCrossentropy (handles class imbalance)
- **Optimizer**: Nadam (lr=0.005)

---

## 🛠 Installation

```bash
# Clone the repo
git clone https://github.com/Chenypovo/Machine-Learning-in-Higgs-Boson-Detection.git
cd Machine-Learning-in-Higgs-Boson-Detection

# Install dependencies
pip install -r requirements.txt
```

---

## 🚀 Usage

### Baseline (Cut-Based Selection)
Run `Higgs-Cutbased selection (1).ipynb` to reproduce the 1.863 sensitivity benchmark.

### ML Model Training
Run `Higgs-Machine Learning (1).ipynb` to train the neural network and verify the 48.5% improvement.

---

## 📂 Project Structure

*   `Higgs-Cutbased selection (1).ipynb`: Baseline physical cut implementation
*   `Higgs-Machine Learning (1).ipynb`: Full ML pipeline (preprocessing, training, evaluation)
*   `nn/`: Hyperparameter search logs (layers, nodes, learning rates)
*   `b4 cut.png` / `after cut.png`: Mass distribution (m_BB) visualizations

---

## 📧 Contact

Developed by **YiPeng Chen**.
- **Email**: yipeng003@e.ntu.edu.sg
- **GitHub**: [Chenypovo](https://github.com/Chenypovo)

---

## 📄 License

MIT License
