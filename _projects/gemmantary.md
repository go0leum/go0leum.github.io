---
layout: page
title: Gemmentary: Automated Sports Commentary Generation
description: A multimodal pipeline for generating real-time sports commentary using video captioning and LLMs
img: assets/img/Gemmantary.png
importance: 4
category: project
related_publications: false
---

[GitHub Repository](https://github.com/fesua/Gemmantary)

**Collaborators:**  
[Joungho An](https://www.linkedin.com/in/joungho-an-07a865206/)  
[Junseo Choi](https://www.linkedin.com/in/wnstj0126/)

---

## 🏅 Project Overview

**Gemmentary** is an AI-powered system designed to **automatically generate real-time sports commentary** based on Olympic video footage. By combining recent advances in **video-language models**, **prompt engineering**, and **LLMs (Large Language Models)**, our system provides compelling and context-aware commentaries tailored to specific events and athletes.

This project explores the intersection of **multimodal understanding** and **creative generation**, demonstrating how AI can augment the way we experience sports broadcasts.

---

## 🛠️ System Pipeline

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Gemmantary.png" title="Gemmentary pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Gemmentary system pipeline
</div>

Our pipeline consists of the following stages:

1. **User Input**  
   The user provides:
   - A video clip of the event
   - Sport type (e.g., diving, gymnastics)
   - Athlete’s name
   - Event details (e.g., Paris Olympics, final round)

2. **Structured Formatting**  
   The input metadata is embedded into a **custom prompt format** that contextualizes the scene for the model.

3. **Video Description (Captioning)**  
   We utilize **Video-LLaVA**, a vision-language model, to generate a rich textual description of the video content, including motion, emotion, and physical dynamics.

4. **Commentary Generation**  
   Through **Retrieval-Augmented Generation (RAG)**, we combine the formatted metadata and video caption, and feed them into the **Gemma LLM**, which generates broadcast-style commentary with a natural narrative flow.

---

## 🎬 Example Output

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/gem_ex.png" title="Input example video" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Sample prompt and commentary output
</div>

**Prompt**  
> *Generate a sports commentary script for the men's 10m platform diving final featuring Chao Yuan at the Paris Olympics, using the video caption as context.*

**Generated Commentary Output**  
> *Good evening, sports fans, and welcome to the final of the men's 10m platform diving at the Paris Olympics. We have a battle for gold between two of the greatest divers of all time—Chao Yuan from China and the defending champion from [another country].*

> *The dive: The athletes take their positions on the platform. The crowd rises as the music starts. Chao Yuan launches into the air with grace and precision. He executes a flawless somersault dive, showcasing world-class control and athleticism.*

> *The aftermath: Chao Yuan hits the water with an impressive splash, creating a moment of pure exhilaration. The judges are visibly impressed, and the crowd erupts into applause.*

> *Conclusion: With that, Chao Yuan secures the gold medal. It’s been an unforgettable final filled with breathtaking performances. Thank you for joining us for our Olympic coverage.*

---

## 💡 Key Contributions

- Designed a **multimodal generation pipeline** integrating vision-language models with large language models
- Developed **prompt formats and templates** optimized for sports commentary style
- Leveraged **RAG (Retrieval-Augmented Generation)** to ground commentary in real video context
- Created a **human-friendly interface** for users to easily upload video and event data

---

## 🔚 Final Thoughts

Gemmentary demonstrates the potential of **AI-generated storytelling** in the realm of sports media. Whether for **highlight clips**, **personalized commentary**, or **low-resource sports broadcasting**, our system opens the door to scalable and immersive content creation.

---

> 🔗 Explore the [GitHub project](https://github.com/fesua/Gemmantary) for code, data, and implementation details.
