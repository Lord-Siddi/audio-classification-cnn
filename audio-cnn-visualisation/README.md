# Audio Classification using CNN & ResNet

This project implements an end-to-end audio classification system capable of recognizing environmental sounds such as dog barking and bird chirping.

## Features
- Mel Spectrogram-based audio preprocessing
- CNN + ResNet architecture implemented in PyTorch
- Data augmentation using mixup
- Serverless FastAPI inference deployed using Modal
- Visualization of intermediate CNN feature maps
- Frontend dashboard built with Next.js and React

## Model Architecture
- Input: Mel Spectrograms (128 mel bands)
- Backbone: Residual CNN blocks
- Output: Softmax over ESC-50 sound classes

## Dataset
- ESC-50 environmental sound dataset
- Original sample rate: 44.1 kHz
- Training and inference performed at 22.05 kHz for efficiency

## Deployment
The trained model is deployed as a serverless FastAPI endpoint using Modal, enabling GPU-backed inference on demand.

## Tech Stack
- Python, PyTorch, torchaudio
- FastAPI, Modal
- React, Next.js

## How to Run (Training)
```bash
python train.py
