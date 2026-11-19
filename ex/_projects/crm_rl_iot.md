---
layout: page
title: Construction Resource Management using Reinforcement Learning
description: 
img: assets/img/crm_rl_iot.png
importance: 1
category: project
giscus_comments: false
---

[GitHub Repository](https://github.com/go0leum/crm_rl_iot.git)

**Collaborators:**  
[Junseok Park](https://github.com/peterjr123)

---

## 🧠 Construction Resource Management using Reinforcement Learning

Efficiently allocating construction resources is essential for controlling costs, meeting project deadlines, and maintaining quality. This project proposes a novel approach using **deep reinforcement learning** to determine optimal operational policies for resource deployment across dynamic construction site environments.

---

### 🎯 Project Objectives

- **Dynamic Resource Allocation**: Efficiently assign equipment and workforce based on time-sensitive and location-specific requirements.
- **Task Modeling**: Define project tasks with varying priorities and dependencies within the construction process.
- **Reinforcement Learning Integration**: Train agents to autonomously learn optimal resource scheduling strategies.
- **Optimization**: Minimize total construction duration and idle time through learned policy execution under limited-resource constraints.

---

### 🧩 Approach & Methodology

This work builds upon the framework introduced in  
📖 *[Simulation of autonomous resource allocation through deep reinforcement learning-based portfolio-project integration](https://doi.org/10.1016/j.autcon.2024.105381)*,  
adopting **deep Q-learning** and a discrete-event simulation environment to train and evaluate agent behavior across multiple construction sites.

---

### 🛠️ System Overview & Simulator

The custom-built simulator supports:
- Customizable construction environments
- Real-time task allocation and equipment tracking
- Visualization of agent decisions and performance improvements

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/crm_rl_iot.png" title="Reinforcement Learning Simulator" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/crm_rl_iot_desc.png" title="Simulator Description" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

> 🖥️ *The simulator delivers a visual and analytical interface for observing how reinforcement learning policies adapt to varying construction environments.*

---

### 🧪 Results & Outcomes

- Improved resource utilization efficiency over rule-based baselines
- Reduced project duration across multiple simulation runs
- Demonstrated scalability to multi-site construction operations

---

### ⚙️ Technologies Used

| Component              | Stack                                      |
|------------------------|---------------------------------------------|
| Programming Language   | Python                                      |
| Frameworks             | Gymnasium       |
| Visualization          | Tkinter       |
| Deployment             | GitHub, Local Simulation Environment        |

---

> 🔗 Explore the [GitHub project](https://github.com/go0leum/crm_rl_iot.git) for code, data, and implementation details.