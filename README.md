# Smart Plant Disease Detector (Tomato)

[![Python](https://img.shields.io/badge/Python-3.9+-blue)](https://www.python.org/)

**Team:** Mohanad Yassin  
**Tier:** 1

---

## Table of Contents
1. [Project Summary](#project-summary)
2. [Problem Statement](#problem-statement)
3. [Solution Overview](#solution-overview)
4. [Technical Approach](#technical-approach)
5. [Dataset Plan](#dataset-plan)
6. [Metrics](#metrics)
7. [Timeline](#timeline)
8. [Resources](#resources)
9. [Risks & Mitigation](#risks--mitigation)
10. [How to Run](#how-to-run)

## Project Summary
An object-detection system using YOLOv8 to detect and classify common tomato leaf diseases from images and provide concise treatment suggestions.

## Problem Statement
Tomato crops are vulnerable to various diseases, and manual inspection can be slow and prone to mistakes.

## Solution Overview
Fine-tune YOLOv8 on PlantVillage tomato dataset + custom images. Outputs disease name, confidence score, and short treatment suggestion.

## Technical Approach
- Model: YOLOv8 (Ultralytics)
- Framework: PyTorch
- Technique: Object Detection

## Dataset Plan
- Public: PlantVillage tomato leaf dataset ([Kaggle link](https://www.kaggle.com/datasets/emmarex/plantdisease))
- Custom: 20–50 phone images
- Labels: Disease classes + bounding boxes

## Metrics
- mAP@0.5 ≥ 0.75
- Precision/Recall ≥ 0.80
- Inference latency <1.2 sec (GPU)

## Timeline
- Week 10: Dataset + Env Setup
- Week 11: Train Model
- Week 12: Test & Improve
- Week 13: Demo Video
- Week 14: Final Docs
- Week 15: Presentation

## Resources
- GPU (local or Colab Pro)
- Storage ~50GB
- Python 3.9+, PyTorch, Ultralytics YOLO

## Risks & Mitigation
| Risk | Probability | Mitigation |
|---|---:|---|
| Low accuracy | Medium | Fine-tune + augment |
| Limited data | Medium | Collect custom data |
| Compute limits | Medium | Use smaller YOLOv8 models |

## How to Run
1. Clone repo: `git clone <repo-url>`
2. Create env: `python -m venv venv && venv\Scripts\activate`
3. Install dependencies: `pip install -r requirements.txt`
4. Follow notebook: `notebooks/01_exploration.ipynb`
