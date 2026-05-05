```markdown
# Improving Hindi Speech Emotion Recognition using Synthetic Data

## 🚀 Overview
This project addresses the challenge of **Speech Emotion Recognition (SER) in Hindi**, a low‑resource language with limited annotated datasets.  
We developed a pipeline for **synthetic voice data generation** using HuBERT embeddings and Gaussian interpolation, enabling robust emotion classification across multiple models (SVM, CNN, Transformer‑CNN).

---

## 🎯 Motivation
- Hindi has **600M+ speakers**, but lacks high‑quality SER datasets.  
- Existing augmentation methods often distort emotional consistency.  
- Our approach generates **synthetic yet emotionally faithful data**, improving generalization and reducing overfitting.

---

## 🛠️ Methodology
1. **Data Preprocessing**
   - Mel‑spectrogram projection and audio decoding.
   - Dataset organization across emotion categories.

2. **Synthetic Data Generation**
   - HuBERT‑based embeddings.
   - Gaussian interpolation for emotion‑consistent augmentation.

3. **Models Evaluated**
   - Classical ML: SVM, Random Forest.  
   - Deep Learning: CNN, LSTM, ResNet, Transformer Encoder.  
   - Hybrid: Transformer‑CNN with feature fusion.

---

## 📊 Results
- **Baseline Models:**  
  - CNN achieved ~62% accuracy, LSTM ~59%, ResNet ~61%.  
  - Performance limited by small dataset size.

- **Gaussian Interpolation Validation:**  
  - Fréchet distance and cosine similarity confirmed synthetic data preserved emotional fidelity.  
  - Distributional overlap between synthetic and real samples was high.

- **Transformer‑CNN on Augmented Data:**  
  - Macro F1 improved from **0.61 (baseline)** to **0.74 with augmentation**.  
  - Accuracy improved from **63% to 78%**.  
  - Stronger generalization across unseen speakers and sentences (LOSO/LOAO tests).

*(Insert confusion matrices, accuracy plots, or spectrograms here for visual impact.)*

---

## 📂 Repository Structure
- `Gaussian Interpolation/` – synthetic data generation pipeline.  
- `RVC Emotion Conversion/` – emotion conversion experiments.  
- `transformer_with_synth_aug/` – Transformer‑CNN training scripts.  
- `.gitattributes` / `.gitignore` – repo hygiene.  
- `LICENSE` – MIT License.

---

## ⚡ How to Run
```bash
# Clone the repo
git clone https://github.com/Aaditya-Jain-01/Improving-Hindi-Speech-Emotion-Recognition-using-Synthetic-Data-Augmentation.git
cd Improving-Hindi-Speech-Emotion-Recognition-using-Synthetic-Data-Augmentation

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