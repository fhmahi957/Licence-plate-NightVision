## Robust Nighttime License Plate Detection using Lightweight Deep Super-Resolution

## Overview

This project addresses the domain shift problem in license plate detection under adverse nighttime conditions. We propose a lightweight pipeline combining FSRCNN (Fast Super-Resolution Convolutional Neural Network) for image enhancement with Faster R-CNN (MobileNetV3 backbone) for detection, achieving significant recovery of detection performance while maintaining real-time capability.

## Problem Statement

License plate detection systems trained on daytime images suffer severe performance degradation  when deployed at night due to domain shift. This project quantifies this degradation and proposes a computationally efficient solution.

## Methodology

### Pipeline Architecture
1. **Baseline Detector**: Faster R-CNN with MobileNetV3-Large backbone trained on clean daytime images
2. **Image Enhancement**: FSRCNN (lightweight super-resolution) to restore nighttime image quality
3. **Domain Adaptation**: Fine-tuning the detector on enhanced nighttime images
4. **OCR Integration**: EasyOCR for license plate text recognition (proof-of-concept, optional)

### Key Components
- **FSRCNN**: 5-layer lightweight architecture for real-time enhancement
- **Faster R-CNN**: Two-stage detector edge deployment
- **Traditional Baselines**: CLAHE (Histogram Equalization) and Gamma Correction for comparison

