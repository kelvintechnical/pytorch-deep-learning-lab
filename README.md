# PyTorch Deep Learning Lab

> **"A diagnostic environment for low-level neural architecture and optimization."**

This repository is my technical laboratory for mastering **PyTorch** and end-to-end Machine Learning pipelines. It documents my progress through 40+ real-world Data Science projects, with a specific focus on architecture search, gradient behavior, and production-minded implementation.

---

## Engineering Focus

Instead of treating models as black boxes, I use a diagnostic mindset to understand:

- **Custom Autograd Functions:** Engineering non-standard backpropagation for specialized loss landscapes.
- **Architecture Profiling:** Measuring latency and memory efficiency during training.
- **Gradient Flow Analysis:** Troubleshooting vanishing and exploding gradients in deep networks.
- **Model Deployment:** Translating research models into production-ready inference systems.

---

## Lab Tracker

| # | Lab | Concepts Covered | Status |
| --- | --- | --- | --- |
| 01 | [Tensor Fundamentals](https://github.com/kelvintechnical/Lab_01_PyTorch_Tensor_Fundamentals) | `torch.tensor()`, `zeros`, `ones`, `arange`, `zeros_like` | ✅ Complete |
| 02 | Random Tensors and Seeds | `torch.rand`, `torch.randn`, `manual_seed` | ⏳ Up Next |
| 03 | Data Types and Memory | `int8`, `float32`, `bool` masks | ⏳ Pipeline |
| 04 | Tensor Attributes | `shape`, `ndim`, `reshape`, `unsqueeze` | ⏳ Pipeline |
| 05 | Tensor Operations | `matmul`, `dot`, `argmax`, aggregation | ⏳ Pipeline |
| 06 | Bio Challenge | DNA one-hot encoding end-to-end | ⏳ Pipeline |

---

## Completed Projects Showcase

| Project | Type | Highlights | Stack | Link | Status |
| --- | --- | --- | --- | --- | --- |
| Dog Breed Prediction (CNN + Streamlit) | Image Classification | Built a custom CNN from scratch for 3 breeds, added L2 regularization and tuned `Adam(lr=0.0001)`, then served predictions in a Streamlit app. | Python, TensorFlow/Keras, Streamlit, Colab | [View Project](https://github.com/kelvintechnical/dog-breed-prediction) | ✅ Complete |

### Dog Breed Prediction Notes

- Trained without transfer learning to strengthen fundamentals in convolutional feature extraction and architecture tradeoffs.
- Used a train/validation/test split of **72% / 18% / 10%** across 3 classes.
- Architecture pipeline:

```text
Input (224x224x3)
  -> Conv2D(64, 5x5, relu) + MaxPool2D
  -> Conv2D(32, 3x3, relu, L2) + MaxPool2D
  -> Conv2D(16, 7x7, relu, L2) + MaxPool2D
  -> Conv2D(8,  5x5, relu, L2) + MaxPool2D
  -> Flatten
  -> Dense(128, relu, L2)
  -> Dense(64,  relu, L2)
  -> Dense(3, softmax)
```

---

## Tech Stack

- **Primary Framework:** PyTorch
- **Supporting Frameworks:** TensorFlow / Keras (for selected projects)
- **Environment:** Google Colab / Linux (Pop!_OS)
- **Experiment Tracking:** Weights and Biases
- **Version Control:** Git and GitHub

---

## Mission

To develop deep technical fluency in neural network internals, optimization strategies, and scalable AI system design, bridging research experimentation with production engineering.

---

## Maintainer

**Kelvin R. Tobias**  
B.S. Software Engineering (WGU, Jan 2026)  
Incoming M.S. AI Engineering (WGU, Dec 2026)  
*Kelvinintech AI Engineering Track - Diesel to DNA*
