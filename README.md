# CogniSense: Early Dementia Detection System

CogniSense is a research-focused multimodal machine learning system designed to study early indicators of dementia by analyzing speech patterns, linguistic features, and cognitive task performance. The project combines Natural Language Processing and Reinforcement Learning to explore scalable and non-invasive approaches to cognitive health assessment.

This work was developed as part of an academic research project and has been accepted at an IEEE conference.

---

## 🧠 Motivation

Early-stage dementia is difficult to diagnose because symptoms are subtle and often mistaken for normal aging. Traditional clinical assessments can be costly, time-consuming, and inaccessible in low-resource settings.

This project explores whether **speech characteristics and simple cognitive tasks**, analyzed through machine learning, can provide early signals of cognitive decline in a scalable and non-invasive way.

---

## 🔍 System Overview

The system integrates three primary data modalities:

### 1. Speech & Acoustic Features
- MFCCs
- Pitch and intonation
- Pause count
- Speech rate

Speech recordings are transcribed using OpenAI’s Whisper ASR model and analyzed for linguistic and acoustic patterns associated with cognitive impairment.

### 2. Text & Semantic Features
- Transcripts generated from speech
- BERT-based embeddings (768-dimensional) to capture semantic richness, coherence, and syntactic structure

### 3. Cognitive & Behavioral Features
- Reaction time
- Task accuracy
- Completion time
- Attention span
- Error rate
- Processing speed

These features capture executive function and cognitive consistency during structured tasks.

---

## ⚙️ Methodology

- **Preprocessing**
  - Speech-to-text using Whisper
  - Acoustic feature extraction from raw audio
  - Text cleaning and BERT embedding generation
  - Normalization and imputation for behavioral data

- **Classification Model**
  - XGBoost classifier trained on combined multimodal feature vectors
  - Binary classification: Healthy vs Dementia

- **Adaptive Cognitive Task Recommendation**
  - Reinforcement Learning using a Deep Q-Network (DQN)
  - Dynamically adjusts cognitive task difficulty based on user performance
  - Reward function encourages engagement and appropriate challenge level

---

## 📊 Results

- Achieved **84% overall classification accuracy** on a public multimodal dataset
- Strong performance in identifying healthy participants
- Identified limitations in recall for dementia cases, highlighting the importance of class balance and further model refinement
- Reinforcement learning agent demonstrated reasonable task adaptation behavior based on cognitive state

This analysis provided valuable insight into both the strengths and limitations of multimodal cognitive assessment systems.

---

## 🧪 Key Learnings

- Multimodal feature fusion provides richer cognitive signals than speech alone
- Speech rate, pauses, and reaction time showed strong correlation with cognitive decline
- Model evaluation and error analysis are critical, especially in healthcare-related ML
- Reinforcement learning can be effectively used for personalization, even in prototype systems

---

## 📁 Repository Structure

- `MODEL TRAINING.ipynb` – Feature extraction, preprocessing, model training
- `MODEL TESTING.ipynb` – Evaluation, metrics, visualizations
- `Dementia Research Paper.pdf` – Full research paper with methodology and results

---

## ⚠️ Disclaimer

This project is a **research prototype** and is **not intended for clinical diagnosis or medical use**. Results are based on public datasets and are meant for academic exploration and learning.

---

## 📄 Publication

**CogniSense: Early Dementia Detection System**  
Accepted at *IEEE ACDSA 2025*

---

## 🚀 Future Work

- Improve class imbalance handling
- Expand dataset diversity
- Incorporate longitudinal data
- Integrate additional modalities such as wearables or physiological signals

---

**Jai Vasi**  
MS Data Science, Stony Brook University  
📧 jai.n.vasi1108@gmail.com  
🔗 LinkedIn: https://www.linkedin.com/in/jaivasi1108
