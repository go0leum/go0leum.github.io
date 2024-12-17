---
layout: page
title: Automated Sports Commentary Generation(Gemmentary)
description:
img: assets/img/Gemmantary.png
importance: 4
category: project
related_publications: false
---

Developed a program designed to generate sports commentary based on a short video clip and a single news update, enabling a full and comprehensive commentary experience.

## Pipeline

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Gemmantary.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    gemmantary pipeline
</div>

- Input: The user provides a video, the sport type, the name of the athlete, and the event information.

- Formatting: We place the sport type, athlete name, and event information into a custom format we designed.

- Video Description: Using Video-LLaVA, we generate a description of the video content.

- Commentary Generation: We integrate the video description with our custom format through RAG (Retrieval-Augmented Generation) and generate commentary using the Gemma model.

## Example

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/gem_ex.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    input example video
</div>

- Prompt:  Make a script for a commentator's commentary on the final for the diving men's 10m platform for diving Chao Yuan at the Paris Olympics based on video caption.

- Output:
    Good evening, sports fans, and welcome to the final of the diving men's 10m platform at the Paris Olympics. We have a battle for gold between two of the greatest gymnasts of all time, Chao Yuan from China and the defending champion, [Name of the competitor from another country].

    The Dive "The athletes take their positions on the platform, and the crowd is on its feet as the music starts. Chao Yuan jumps into the air with incredible precision and grace, his body arching as he prepares to make the dive. He executes a perfect somersault dive, showcasing his incredible athleticism and control. The crowd is on its feet, and the judges are watching the performance with rapt attention."

    The Aftermath "The impact is visually stunning as Chao Yuan hits the water with a splash, creating a moment of pure exhilaration. His body is perfectly arched, and his performance is a testament to the beauty of the sport. The judges give him a standing ovation for his incredible performance."

    Conclusion "And that concludes the final of the diving men's 10m platform at the Paris Olympics. Chao Yuan has secured his gold medal, and the crowd erupts in applause. It's been an incredible final, and we've witnessed some of the best diving the world has ever seen. Thank you for joining us for the coverage of the Paris Olympics."
