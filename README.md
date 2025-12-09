# 🧠 Tri-Modal Clinical Diagnosis via Speech, Image, and Text Fusion

This repository contains the code, data loaders, and evaluation pipeline for our tri-modal classifier that fuses **speech, image, and textual** inputs to perform multi-label classification of clinical conditions.

## 📦 Modalities
- **Text**: TF-IDF embeddings from patient queries
- **Audio**: `wav2vec2` representations of speech
- **Images**: EfficientNet image features

## 🧪 Datasets
We use a translated English version of the **VietMed-Sum** dataset (500 samples, 18 labels). Audio is synthetically generated for each case.

## 🚀 Models
- `text-only`, `image-only`, `audio-only`
- `text+image`, `text+audio`, `image+audio`
- `tri-modal`: fusion of all three modalities

## 📊 Evaluation
- 5-fold cross-validation
- Micro- and Macro-F1 metrics
- **95% bootstrap confidence intervals**
- Fold-wise performance variation


## 📈 Results Summary

| Model         | Micro-F1 | Macro-F1 |
|---------------|----------|----------|
| Tri-modal     | 0.7822   | 0.6786   |
| Text-only     | 0.7085   | 0.4929   |
| Image-only    | 0.6278   | 0.4994   |
| Audio-only    | 0.5004   | 0.3230   |



