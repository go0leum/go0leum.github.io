---
layout: post
title: ArchiGlance 건축도면 가독성 높여주는 프로그램
date: 2025-07-29 21:01:00
description: 연구실에서 첫 임무
tags: requirement_analysis, web_development, computer_vision
categories: experience project
thumbnail: assets/img/archi_glance_diagram.png
---

건축도면의 건축도면번호가 있는데 건축도면번호를 클릭하면 관련된 건축도면 페이지로 이동되는 기능 구현해봤습니다.

토목과 컴퓨터공학을 전공한 저에게 건축 도면은 다소 낯선 영역이었습니다. 하지만 도면 이해가 선행되어야 했기에, 50페이지가 넘는 도면을 한 장 한 장 넘겨보며 건축 기호와 체계를 익혔습니다.

도면 분석 후, 저는 이 프로젝트에 **'Archi Glance'**라는 이름을 붙이고 아래와 같이 구체적인 개발 계획을 수립했습니다.

1. **웹 뷰어 개발**: PDF 도면을 웹상에서 열람하고 상호작용할 수 있는 환경 구축
2. **Computer Vision** 모델 개발: 도면 기호(참조 마크) 자동 인식을 위한 데이터 수집 및 학습
3. **OCR API 연동**: 인식된 기호 내의 텍스트(도면 번호) 추출
4. **매핑 알고리즘 구현**: 추출된 번호를 기반으로 페이지 간 링크 연결(Pagination)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/archi_glance_diagram.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Archi Glance 알고리즘 다이어그램
</div>

개발 과정에서 이전에 스타트업(LightVision)에서 쌓았던 경험들이 빛을 발했습니다. 데이터 수집 전략부터 모델 선정, 인식률 향상을 위한 패치(Patch) 분할 기법 등, 실무에서 몸으로 익혔던 노하우가 큰 자산이 되었습니다.

가장 큰 난관은 OCR 성능이었습니다. 비전 모델이 기호 위치는 잘 찾았지만, 기호 안의 작은 글자들을 명확히 읽어내지 못했습니다. Google OCR로 교체해 보았지만, 여전히 정확도는 기대에 미치지 못했습니다.

저는 실패한 OCR 결과들을 나열해 놓고 패턴을 분석하기 시작했습니다. 그러다 문득 해결의 실마리를 발견했습니다. 도면 번호는 일정한 규칙(패턴)을 가지고 있었기에, 오인식 된 결과라 하더라도 '유사도 측정'을 통해 원래 값을 역추적할 수 있겠다는 생각이 들었습니다.

이를 바탕으로 데이터를 표준화하고 유사도 기반 매핑 알고리즘을 자체 개발하여 적용했고, 결과적으로 인식 성능을 비약적으로 향상시킬 수 있었습니다.


[![ArchiGlance 개발 점검 영상](http://img.youtube.com/vi/qP_cIFxxxYQ/0.jpg)](https://youtu.be/qP_cIFxxxYQ)
<div class="caption">
    ArchiGlance 개발 점검 영상
</div>


주어진 시간은 단 2주였습니다. 다른 업무와 병행해야 했기에 빠듯한 일정이었지만, 웹 개발부터 AI 모델링, 그리고 알고리즘 개선까지 풀스택(Full-stack)으로 프로젝트를 완수해냈다는 점에 큰 성취감을 느낍니다.


