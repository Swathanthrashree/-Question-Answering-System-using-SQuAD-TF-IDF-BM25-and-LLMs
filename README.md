## 📚 Question Answering System Evaluation: IR + Pre-trained Language Models

This project presents a comprehensive evaluation of Question Answering (QA) systems that combine traditional Information Retrieval (IR) techniques with pre-trained language models. Our goal is to understand how different combinations of retrieval and language modeling impact QA performance.

We experimented with classical IR methods — **BM25** and **TF-IDF** — alongside transformer-based models such as **DistilBERT**, **RoBERTa**, and **BERT**, as well as newer models hosted on **Groq’s inference platform**, including **Gemma** and **LLaMA** variants.

### 📊 Benchmark: SQuAD v1.1

We used the **Stanford Question Answering Dataset (SQuAD v1.1)** for evaluation. Performance was measured using two key metrics:
- **Exact Match (EM)**
- **F1 Score**

### 🔍 Key Findings

- **BM25** consistently outperforms **TF-IDF** in retrieval quality.
- **RoBERTa** achieved the best QA performance overall with:
  - **81% EM**
  - **84.24% F1**
- Among Groq-hosted models, **Gemma 2B Instruct** stood out for its efficiency:
  - **50% EM**
  - **72.99% F1**
  - Despite being a compact model, it delivered impressive results.

These results emphasize the need to balance **retrieval strength** and **language model capabilities** when building QA systems—especially for **resource-constrained environments**.

### ❓ Research Questions Addressed

- How do different retrieval methods (**BM25**, **TF-IDF**) impact overall QA system performance?
- Which pre-trained language models provide optimal answer extraction capabilities?
- How do **parameter-efficient models** compare to larger models in QA tasks?
- What architectural configurations yield the best performance when combining retrieval and extraction components?

---

This work serves as a step toward building **robust**, **resource-efficient**, and **scalable** QA systems for real-world applications.
