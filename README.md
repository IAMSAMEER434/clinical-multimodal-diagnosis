# Clinical Multimodal Diagnosis

This repository supports the paper:  
**Speech–Image Multimodal Understanding Framework for Clinical Visual Diagnosis via Audio Caption Alignment**

## Contents
- Notebooks and scripts for training
- Out-of-fold logits
- Trained model checkpoints
- Evaluation figures (Grad-CAM, architecture)

## Reproducibility
Run `pip install -r requirements.txt`.  
All outputs saved in `/analysis_outputs/`.

## Available OOF Artifacts

- `trimodal_oof_logits.npy`: OOF logits for tri-modal model
- `text_only_oof_logits.npy`: OOF logits for text-only model
- `image_only_oof_logits.npy`: OOF logits for image-only model
- `audio_only_oof_logits.npy`: OOF logits for audio-only model

