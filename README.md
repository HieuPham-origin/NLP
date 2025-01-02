# NLP Repository

Welcome to the NLP repository! This project focuses on solving tasks in Natural Language Processing (NLP), including machine translation and information extraction. By leveraging state-of-the-art techniques and models, this repository aims to address challenges in technology and digitalization domains effectively.

## Table of Contents

1. [Machine Translation](#machine-translation)
2. [MetaLlama8B for Information Extraction](#metallama8b-for-information-extraction)
3. [Requirements](#requirements)
4. [Contributors](#contributors)

---

## Machine Translation

This module implements two variations of sequence-to-sequence models based on LSTMs, build with PyTorch:

1. **LSTM-to-LSTM Without Attention**:
   - This is a baseline encoder-decoder model where the input sequence is transformed into a fixed-size vector representation before being decoded into the target sequence.
   - It is suitable for relatively short sentences but struggles with longer sequences due to the lack of a mechanism to focus on specific parts of the input.

2. **LSTM-to-LSTM With Attention**:
   - This model incorporates an attention mechanism, which allows the decoder to dynamically attend to different parts of the input sequence during generation.
   - The attention mechanism significantly improves performance on longer and more complex sentences by overcoming the bottleneck of fixed-size vector representations.

Both implementations support training, evaluation, and inference functionalities.

---

## MetaLlama8B for Information Extraction

This module addresses information extraction tasks in the field of technology and digitalization using a two-stage approach:

1. **Data Labeling with Meta Llama**:
   - The Meta Llama 8B model is utilized to annotate data efficiently. It leverages its large-scale pretraining to generate high-quality labels for various aspects of information extraction tasks.

2. **Model Training with PhoBERT**:
   - PhoBERT, a robust transformer-based model pre-trained on Vietnamese text, is fine-tuned using the labeled data for specific information extraction tasks.
   - This stage focuses on identifying and extracting structured information from unstructured text efficiently.

This hybrid approach combines the strengths of large language models and domain-specific fine-tuning to achieve state-of-the-art results.

---

## Requirements

- Python 3.8+
- PyTorch 1.10+
- Transformers
- scikit-learn
- numpy
- matplotlib

---

## Contributors

- Hieu Pham ([GitHub](https://github.com/HieuPham-origin))

---
