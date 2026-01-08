# Model Optimization using ONNX and Quantization  
### NLLB & Whisper – Performance Analysis

## 📌 Project Overview
This project focuses on optimizing large AI models used for **machine translation**
and **speech recognition** by converting them into **ONNX format** and applying
**int8 quantization**.

The objective is to reduce **RAM usage**, improve **execution speed**, and enable
efficient deployment on **low-resource devices** such as mobile phones.

---

## 🧠 Models Used
- **NLLB (No Language Left Behind)** – Language Translation Model  
- **Whisper** – Automatic Speech Recognition (ASR) Model  

---

## ⚙️ Technologies & Tools
- ONNX (Open Neural Network Exchange)
- ONNX Runtime
- Int8 Quantization
- KV-Cache
- Model Partitioning
- Olive Optimization Tool

---

## 🔍 Key Optimization Techniques

### 1. ONNX Conversion
ONNX provides a standardized representation of neural networks, enabling
faster inference and cross-platform deployment.

### 2. Quantization (int8)
Model weights are converted from float32 to int8 to reduce memory usage
and increase execution speed while maintaining accuracy.

### 3. KV-Cache Optimization
KV-Cache stores previously computed values to avoid repeated calculations,
improving performance for sequence-based models.

### 4. Model Separation
Large models are divided into smaller components to prevent memory
duplication and reduce peak RAM usage.

---

## 📊 Performance Comparison

### NLLB Model

| Model Type | RAM Usage | Execution Time | Improvement |
|-----------|-----------|----------------|-------------|
| Normal ONNX NLLB | 2.5 GB | 8 seconds | — |
| Optimized NLLB | 1.3 GB | 2 seconds | 1.9× less RAM, 4× faster |

---

### Whisper Model

| Model Type | RAM Usage | Execution Time (11s audio) | Improvement |
|-----------|-----------|-----------------------------|-------------|
| Whisper (Olive Optimized) | 1.4 GB | 1.9 seconds | — |
| Optimized Whisper | 0.9 GB | 1.6 seconds | 1.5× less RAM, 1.2× faster |

🔹 **Low-Memory Mode:**  
Whisper can run using **0.5 GB RAM** with execution time of **2.1 seconds**,
suitable for devices with less than 8 GB RAM.

---

## 🎯 Applications
- Real-time translation systems
- Speech-to-text applications
- Offline AI applications
- Mobile and embedded systems
- Edge computing

---

## 📌 Conclusion
This project demonstrates that large AI models such as **NLLB** and **Whisper**
can be effectively optimized using **ONNX**, **quantization**, and memory
management techniques. The optimized models achieve significant performance
improvements while maintaining accuracy.

---
