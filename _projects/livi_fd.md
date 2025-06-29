---
layout: page
title: Autonomous Fire Detection System
description: 
img: assets/img/livi_fd.png
importance: 2
category: work
related_publications: false
---

## 🔥 Autonomous Fire Detection System

This project introduces a deep learning–based fire detection system that localizes fires within images using **Inception V3** and **Class Activation Mapping (CAM)** techniques. To improve detection accuracy for small-scale fires, a **sliding window method** was also applied.

---

### 🧠 Model Architecture & Workflow

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/CAM_desc.png" title="CAM Visualization" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  [Class Activation Mapping (CAM)](https://doi.org/10.48550/arXiv.1512.04150)
</div>

- **Base Model**: Inception V3, pre-trained on ImageNet, was fine-tuned for binary classification (fire / non-fire)
- **Localization**: CAM was leveraged to generate heatmaps that reveal which regions of the image contributed to the fire prediction
- **Visualization**: The resulting activation maps highlight fire zones, providing both detection and interpretability

---

### 🔍 Sliding Window for Small Fire Detection

Small fires often fail to dominate global feature representations, reducing detection sensitivity. To overcome this:

- **Sliding Window Technique**:  
  The original image is partitioned into smaller overlapping regions
- **Localized Analysis**:  
  Each window is independently passed through the model and corresponding CAM is generated
- **Aggregation**:  
  Fire detection results and heatmaps from all windows are combined to yield final predictions

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/livi_fd.png" title="Model Output Example" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  Model Prediction Sample
</div>

---

### 🧪 Summary of Outcomes

| Feature                   | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| 🔍 Detection Approach      | Inception V3 + CAM                                                         |
| 📐 Localization           | Heatmap-based pixel-level fire localization                                 |
| 🧩 Enhancement Technique  | Sliding window–based sub-image analysis                                     |
| 🎯 Use Case Potential     | Smart surveillance, early wildfire detection, disaster response systems     |

---
