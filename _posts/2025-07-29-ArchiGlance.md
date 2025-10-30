---
layout: post
title: ArchiGlance 건축도면 가독성 높여주는 프로그램
date: 2025-07-29 21:01:00
description: 회계사 선배에게 개발 의뢰를 받았다
tags: requirement_analysis
categories: experience project
thumbnail: assets/img/archi_glance_diagram.png
---

2025년 1월부터 서울대 건축공학과 건설기술연구실에서 인턴을 시작했다.

그동안 논문도 읽고 연구실에서 어떤 연구들을 하는지 보면서 인턴생활을 했는데,
6개월이 지난 7월, 처음으로 교수님께 임무를 받았다.

건축도면의 건축도면번호가 있는데 건축도면번호를 클릭하면 관련된 건축도면 페이지로 이동되는 기능 구현하는 것을 원하셨다.

토목공학과 컴퓨터공학을 전공한 나에게 건축도면은 생소했다. 
처음으로 50페이지가 넘는 건축도면을 읽으며 건축도면기호들을 공부했다.

빠르게 요구사항을 분석한 뒤, 간단하게 개발계획을 세웠다.
그리고 나름대로 Archi Glance라는 웹페이지 이름도 붙였다.

1. PDF viewer 기능을 위해 웹페이지로 개발
2. 도면 내 도면기호 인식을 위한 computer vision 모델 개발
    - 데이터 수집
    - 모델 학습
3. 도면기호 내 도면번호 인식을 위한 OCR API 연결
4. 도면번호 mapping 및 pagination 기능 개발

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/archi_glance_diagram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Archi Glance 알고리즘 다이어그램
</div>

Archi Glance를 개발할 때 내가 LightVision에서 일하며 배우고 익힌 경험들이 엄청난 도움이 되었다.
데이터 수집, 모델을 선정하는 과정, 도면 기호 인식 성능을 위한 patch 분할, 모델 학습 과정.. 등등

Archi Glance를 개발할 때 OCR 성능이 가장 문제였다.
computer vision 모델로 도면 기호를 성공적으로 인식했지만 기호 내 글자들을 제대로 인식하지 못했다. 
Clova OCR과 Google OCR의 성능을 비교하여 좀 더 나은 Google OCR을 적용했지만 턱없이 부족했다.
그래서 OCR의 실패요인을 분석하고 패턴을 파악하려 했고 실패한 OCR 결과들을 살펴보다가 해결책이 떠올랐다. 
실패한 OCR 결과물들은 정형화된 도면번호의 패턴 덕분에 어느 정도의 예측을 할 수 있었고 이전에 정상적으로 인식된 도면 번호와 유사도 측정을 통해 매칭이 가능했다.
따라서 표준화 및 정제, 유사도 기반 매핑 알고리즘을 개발했고 성능이 눈에 띄게 향상되었다.


[![ArchiGlance 개발 점검 영상](http://img.youtube.com/vi/oICY6NiGGWA/0.jpg)](https://youtu.be/oICY6NiGGWA)
<div class="caption">
    ArchiGlance 개발 점검 영상
</div>


주어진 2주라는 시간 동안 다른 일을 하면서 틈틈이 Archi Glance 개발을 했다.
사실 시간이 충분하지 않았는데 웹페이지 개발, computer vision 모델 개발(데이터 수집, 모델 학습, 품질 평가), OCR 기능 연결, 성능 개선까지 해냈다는 게 뿌듯하다.


