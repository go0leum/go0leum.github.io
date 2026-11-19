---
layout: page
title: AuditMate-Lite - Audit Assistance Automation
description: Automating repetitive accounting audit tasks
img: assets/img/AuditMate-Lite.png
importance: 1
category: project
giscus_comments: false
---

[Service Link](https://auditmate-793615282246.asia-northeast3.run.app/) | [Tutorial Video](https://youtu.be/W8GGaPYeKFU)

# 📊 AuditMate-Lite: Cloud-Based Audit Automation Tool

### 🚀 Transforming Manual Audit Workflows into Automated Systems

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/AuditMate-Lite.png" title="AuditMate-Lite Thumbnail" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

Auditing involves rigorous and repetitive tasks that often follow strict rules. **AuditMate-Lite** is a web-based solution developed to automate the mundane aspects of an accountant's workflow, specifically the verification of client records and proof documents. 

Born from a real-world request by a professional accountant to automate rule-based tasks, this tool streamlines the audit process, allowing professionals to focus on complex decision-making rather than repetitive checking.

---

## 🎯 Project Objectives

The primary goal was to digitize and automate the "Rule-Base" operational logic of accounting audits.

*   **Automate Core Workflows:** Automate 3 out of 5 key audit steps: confirming details, reviewing proof documents, and organizing missing items.
*   **Cloud Accessibility:** Transition from a local script to a **Google Cloud Platform (GCP)** hosted service for easy access without installation.
*   **User-Centric Design:** Provide a simple web interface and tutorial for non-technical users.

---

## ⚙️ Process & Architecture

The audit process was analyzed into five stages. AuditMate-Lite focuses on automating the middle three, which are highly repetitive.

1.  External Guideline Analysis (Manual)
2.  **Client Detail Verification (Automated)**
3.  **Proof Document Review (Automated)**
4.  **Deficiency Listing (Automated)**
5.  Client Communication (Manual)

### 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Backend** | Python, Django |
| **Frontend** | JavaScript, HTML/CSS |
| **Cloud** | Google Cloud Platform (Cloud Run, Cloud Build, GCS) |

---

## ☁️ Cloud Deployment & DevOps

Moving from a local environment to the cloud was a key milestone for this project.

*   **Google Cloud Run:** Used for serverless deployment of the Django application.
*   **CI/CD:** Established a deployment pipeline from local development to the cloud.
*   **Infrastructure:** Managed bucket storage and build configurations.

---

## 🎥 User Experience & Tutorial

To ensure the tool is usable by accountants with varying degrees of technical comfort, a comprehensive video tutorial was created.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    <div class="embed-responsive embed-responsive-16by9">
      <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/W8GGaPYeKFU" allowfullscreen></iframe>
    </div>
  </div>
</div>
<div class="caption">
    AuditMate-Lite Tutorial Video
</div>

---

## 🧩 Development Story

> "I want to automate parts of my work, is it technically possible?"

This project started with a simple question from a senior accountant. Through **Requirement Analysis**, I translated vague ideas into concrete specifications. Seeing the client smile when the abstract idea became a reality was the most rewarding part of this journey.

It was my first experience applying theoretical **Requirements Engineering** to a real-world client, analyzing their needs, and effectively implementing a solution that solved their pain points.

---

## 🔗 Links

*   **Service:** [AuditMate-Lite Web App](https://auditmate-793615282246.asia-northeast3.run.app/)
*   **Demo Video:** [YouTube Link](https://youtu.be/W8GGaPYeKFU)
