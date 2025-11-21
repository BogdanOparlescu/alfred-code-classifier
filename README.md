# **Alfred Code Classifier**

**Alfred** is a lightweight Code Classifier trained on the *[burtenshaw/PleIAs_common_corpus_code_classification](https://huggingface.co/datasets/burtenshaw/PleIAs_common_corpus_code_classification)* dataset, able to identify 154 programming languages plus an additional Unknown class.

The original dataset provides 127,723 test and 14,192 validation samples.
Both sets were expanded to 3,132,962 and 338,402 samples respectively using a 256-token sliding window with a stride of 128.

## **Model Overview**
- Architecture: ALBERT-based Classification Model
- Parameters: 997,595
- Tokenizer vocab size: 11,273
- Epochs: 4
- Batch size: 64
- Learning rate: 2×10⁻⁴
- Regularization: None
- Training time: 12h
- Hardware: NVIDIA T4 (Google Colab)

## **Performance**
- Final validation accuracy: *0.8195*
- Final training loss: *0.6735*

## **Results**
### Training Dataset Confusion Matrix
![Training Confusion Matrix](Confusion%20Matrix%20Results/Alfred4_CM_full_training.png)

### Validation Dataset Confusion Matrix
![Validation Confusion Matrix](Confusion%20Matrix%20Results/Alfred4_CM_full_validation.png)