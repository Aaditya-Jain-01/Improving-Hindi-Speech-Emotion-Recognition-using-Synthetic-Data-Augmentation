# Improving Hindi Speech Emotion Recognition using Synthetic Data

![Python](https://img.shields.io/badge/python-3.9%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![HuBERT](https://img.shields.io/badge/HuBERT-Embeddings-orange)
![Transformer-CNN](https://img.shields.io/badge/Transformer-CNN-lightgrey)
![GitHub stars](https://img.shields.io/github/stars/Aaditya-Jain-01/Improving-Hindi-Speech-Emotion-Recognition?style=social)
![GitHub forks](https://img.shields.io/github/forks/Aaditya-Jain-01/Improving-Hindi-Speech-Emotion-Recognition?style=social)

---

## 🧠 Overview
This project focuses on **Speech Emotion Recognition (SER) in Hindi**, a low‑resource language with limited annotated datasets.  
We developed a pipeline for **synthetic voice data generation** using **HuBERT embeddings** and **Gaussian interpolation**, enabling robust emotion classification across multiple models.  

The system improves generalization across unseen speakers and sentences, addressing the scarcity of high‑quality Hindi SER datasets.

---

## ⚙️ Features
- **Synthetic Data Generation** using Gaussian interpolation on HuBERT embeddings.  
- **Emotion‑consistent augmentation** that preserves fidelity across emotion classes.  
- **Baseline models**: SVM, CNN, LSTM, ResNet, Transformer Encoder.  
- **Hybrid Transformer‑CNN** architecture with feature fusion for improved accuracy.  
- **Validation metrics**: Fréchet distance, cosine similarity, LOSO/LOAO generalization tests.  

---

## 📸 Demo
Example placeholders (replace with your plots/images):
![Confusion Matrix](images/confusion_matrix.png)
![Augmentation Sweep](images/augmentation_sweep.png)

---

## 🛠 Installation
Requires **Python 3.9+**.  

Clone the repository:
```bash
git clone https://github.com/Aaditya-Jain-01/Improving-Hindi-Speech-Emotion-Recognition.git
cd Improving-Hindi-Speech-Emotion-Recognition
```

# Install dependencies
pip install -r requirements.txt

# Run training
python train_transformer_cnn.py --data ./data/augmented
```

---

## 🧩 Key Contributions
- First systematic attempt at **synthetic augmentation for Hindi SER**.  
- Demonstrated that **Gaussian interpolation on HuBERT embeddings** preserves emotional consistency.  
- Achieved **state‑of‑the‑art performance** compared to baseline models.  

---

## 📌 Future Work
- Expand dataset with more diverse speakers.  
- Explore GAN/VAE‑based augmentation for richer emotional variation.  
- Benchmark against multilingual SER datasets.

---

## 👨‍💻 Author
**Aaditya Jain**

### My Role
- Designed and implemented the Gaussian interpolation pipeline for synthetic data generation.  
- Integrated HuBERT embeddings into the augmentation workflow.  
- Conducted experiments with Transformer‑CNN and analyzed performance improvements.  
- Organized and documented the repository for presentation.

---

## 📜 License
This project is licensed under the MIT License.
```
