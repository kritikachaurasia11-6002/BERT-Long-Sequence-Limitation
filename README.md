# BERT-Long-Sequence-Limitation
BERT long sequence limitation using sliding window on SQuAD dataset

# BERT Long Sequence Limitation (Sliding Window Approach)

## 📌 Objective
The objective of this project is to overcome the 512 token limitation of BERT by implementing a sliding window approach and comparing it with the truncation baseline.

---

## 📊 Dataset
- SQuAD (Stanford Question Answering Dataset)
- Used subset for faster training

---

## ⚙️ Models Implemented

### 1. Baseline Model (Truncation)
- Context is truncated to 512 tokens
- Information beyond limit is lost

### 2. Improved Model (Sliding Window)
- Context is split into overlapping chunks
- Stride used: 128
- Preserves long document information

---

## 🧠 Methodology
- Tokenization using BERT tokenizer
- Sliding window technique for long sequences
- Chunk-based aggregation using max score selection

---

## 📈 Results

| Model | Accuracy | F1 Score | Training Time | Parameters |
|------|--------|---------|--------------|-----------|
| Baseline BERT | To be updated | To be updated | To be updated | ~108M |
| Sliding Window BERT | To be updated | To be updated | To be updated | ~108M |

---

## ⏱️ Observations
- Sliding window improves performance over truncation
- Helps in handling long documents
- Slight increase in training time

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
