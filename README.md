# Zero-Shot Multimodal Anomaly Detection using Vision-Language Models

## Overview

This project presents a **training-free multimodal anomaly detection system** using advanced Vision-Language Models (VLMs). The framework combines **OWL-ViT v2** for open-vocabulary object and defect detection with the **Segment Anything Model (SAM)** for precise pixel-level segmentation.

The system can detect and localize anomalies such as:

- Cracks
- Dents
- Surface discoloration
- Structural defects
- Manufacturing irregularities

without requiring any task-specific fine-tuning or supervised training.

---
<img width="960" height="496" alt="plate vlm" src="https://github.com/user-attachments/assets/ccc13250-0627-4241-966e-83e081535ea6" />

## Features

- Zero-shot anomaly detection
- Open-vocabulary defect recognition
- Pixel-level segmentation using SAM
- Training-free pipeline
- Natural language defect querying
- Anomaly heatmap generation
- Industrial inspection ready

---

## Architecture

### Two-Stage Detection Pipeline

### 1. Open-Vocabulary Defect Detection

Uses **OWL-ViT v2** to detect anomaly regions using natural language prompts.

Example prompts:

```python
["crack", "surface defect", "metal dent", "corrosion"]
```

### 2. Pixel-Level Segmentation

Detected regions are passed into **Segment Anything Model (SAM)** for:

- Segmentation masks
- Defect boundary extraction
- Heatmap generation

---

## Workflow

```text
Input Image
     │
     ▼
OWL-ViT v2 (Zero-Shot Detection)
     │
     ▼
Bounding Box Proposals
     │
     ▼
Segment Anything Model (SAM)
     │
     ▼
Pixel-Level Segmentation
     │
     ▼
Anomaly Heatmaps & Localization
```

---

## Tech Stack

| Component | Technology |
|---|---|
| Detection Model | OWL-ViT v2 |
| Segmentation Model | SAM |
| Framework | PyTorch |
| NLP + Vision | Hugging Face Transformers |
| Image Processing | OpenCV |
| Visualization | Matplotlib |

---

## Applications

- Industrial quality inspection
- Manufacturing defect analysis
- Infrastructure monitoring
- Surface anomaly detection
- Automated visual inspection
- Smart factory systems

---

## Key Highlights

- No training required
- Detects unseen anomaly categories
- Open-vocabulary querying
- High-quality segmentation masks
- Generalized defect localization
- Scalable multimodal AI pipeline

---

## Example Defects Detected

| Defect Type | Description |
|---|---|
| Crack | Surface fractures |
| Dent | Structural deformation |
| Discoloration | Color inconsistencies |
| Corrosion | Surface degradation |
| Structural Damage | Irregular damaged regions |

---


## Output

The system generates:

- Bounding-box localization
- Segmentation masks
- Defect heatmaps
- Open-vocabulary anomaly predictions

---
<img width="960" height="496" alt="egg vlm" src="https://github.com/user-attachments/assets/10420d20-1d43-42d5-9327-92102b30b9a0" />

## Example Pipeline

1. Input industrial image
2. OWL-ViT detects anomaly candidates
3. Bounding boxes generated
4. SAM refines anomaly regions
5. Heatmaps and segmentation masks produced

---

## Future Improvements

- Real-time video anomaly detection
- Edge AI deployment
- Temporal anomaly tracking
- Industrial IoT integration
- Diffusion-based refinement

---

## Research Contribution

This work demonstrates how **Vision-Language Models (VLMs)** can enable:

- Zero-shot anomaly detection
- Training-free industrial inspection
- Generalized defect localization
- Multimodal semantic understanding

for next-generation intelligent inspection systems.

---

## Advantages

- Eliminates expensive defect labeling
- Works on unseen anomaly categories
- Highly scalable
- Flexible natural-language querying
- Minimal deployment overhead

---

## Limitations

- Dependent on prompt quality
- May struggle with extremely subtle anomalies
- Inference can be computationally expensive

---

## Acknowledgements

This project uses:

- OWL-ViT v2
- Segment Anything Model (SAM)
- Hugging Face Transformers
- PyTorch
- OpenCV

---
