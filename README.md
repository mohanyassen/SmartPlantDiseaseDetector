# Smart Plant Disease Detector (Tomato)

**Team:** Mohanad Yassin  
**Tier:** 2 (Intermediate)

## Project Summary
An object-detection system using YOLOv8 to detect and classify common tomato leaf diseases from images and provide a concise treatment suggestion. The system aims to support farmers and agronomists by enabling early disease detection through leaf images.

## Problem Statement
Tomato crops are vulnerable to various diseases, and manual inspection can be slow and prone to mistakes. This project automates the detection process using computer vision, providing fast and consistent results to prevent crop loss.

## Solution Overview
We fine-tune a YOLOv8 model using the PlantVillage tomato dataset plus custom images collected under real conditions. The model outputs disease name, confidence level, and treatment advice.

## Technical Approach
- Model: YOLOv8
- Framework: PyTorch + Ultralytics
- Technique: Object Detection

## Dataset Plan
- Public: PlantVillage tomato dataset
- Custom: 20–50 personal images
- Labels: Disease classes + bounding boxes

## Metrics
- mAP@0.5 ≥ 0.75
- Precision/Recall ≥ 0.80
- Latency < 1.2 sec (GPU)

## Timeline
- Week 10: Dataset + Env Setup
- Week 11: Train Model
- Week 12: Test & Improve
- Week 13: Demo Video
- Week 14: Final Docs
- Week 15: Presentation

## Risks & Mitigation
| Risk | Probability | Mitigation |
|---|---:|---|
| Low accuracy | Medium | Fine-tune + augment |
| Limited data | Medium | Collect custom data |
| Compute limits | Medium | Use YOLOv8 small model |

