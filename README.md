# 📱 High-End Phone Classifier using ANN Optimized with Whale Optimization Algorithm (WOA)

This project implements an **Artificial Neural Network (ANN)** to classify smartphones as high-end or not, based on selected hardware features. The model is further optimized using the **Whale Optimization Algorithm (WOA)** to enhance classification accuracy.

---

## 🚀 Project Overview

Smartphones vary widely in specifications and price. This project aims to predict whether a phone is high-end based on features like battery power, screen resolution, and RAM. Initially, an ANN is trained using the **Adam Optimizer**. Later, **WOA** is applied to optimize key hyperparameters—improving accuracy significantly.

---

## 📌 Features Used

- `battery_power`
- `px_height`
- `px_width`
- `ram`  


---


## 🧠 Model Architecture

- Input Layer: 4 features
- 2 Hidden Layers: ReLU Activation
- Output Layer: Sigmoid Activation
- Loss Function: Binary Crossentropy
- Optimizers: 
  - Phase 1: Adam
  - Phase 2: Whale Optimization Algorithm (WOA)

---

## ⚙️ Optimization with WOA

**WOA** is a bio-inspired optimization algorithm mimicking humpback whales' bubble-net hunting strategy. It's used here to fine-tune:
- Number of neurons
- Learning rate
- Batch size

This significantly boosts the model's predictive performance.

---

## 📈 Workflow

1. Load and preprocess dataset
2. Create binary classification label (`High_End`)
3. Handle missing values and scale features
4. Train baseline ANN using Adam optimizer
5. Apply WOA to tune hyperparameters
6. Compare accuracies and analyze results

---

## 🧪 Evaluation Metrics

- **Accuracy**
- **Confusion Matrix**
- **Loss Value per Epoch**

---

## 📊 Results

| Model | Accuracy |
|-------|----------|
| ANN + Adam | ~60% |
| ANN + WOA Optimized | 🚀 Improved by 10–15% |

---

## 📚 Libraries Used

- `numpy`
- `pandas`
- `tensorflow`
- `scikit-learn`
- `matplotlib`
- `WOA` 

---

## 💡 Future Scope

- Include more features like CPU speed, screen size, etc.
- Extend the model for multi-class classification (low, mid, high-end).
- Explore alternative optimizers (PSO, GA, HHO).
- Deploy model as a web app using Flask/Streamlit.

---

## 🔗 References

- [Whale Optimization Algorithm Paper (Mirjalili & Lewis, 2016)](https://doi.org/10.1016/j.advengsoft.2016.01.008)
  


