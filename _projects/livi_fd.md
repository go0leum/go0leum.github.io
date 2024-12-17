---
layout: page
title: Autonomous Fire Detection System
description: 
img: assets/img/livi_fd.png
importance: 2
category: work
related_publications: false
---

## Model

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/CAM_desc.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    [Class Activation Mapping(CAM)](https://doi.org/10.48550/arXiv.1512.04150)
</div>

Implemented fire detection within images using the Inception V3 model, and utilized Class Activation Maps (CAM) to pinpoint the exact location of fires in the images.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/livi_fd.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Model Description
</div>

Enhanced the accuracy of small-scale fire detection by applying a sliding window method. Created a set of windows from the original image using the sliding window technique, and computed the detection results and CAM outcomes for each window to generate the final detection results.