---
layout: post
title: AuditMate-Lite 버전 배포
date: 2025-12-06 21:01:00
description: 회계사 선배에게 개발 의뢰를 받았다
tags: requirement_analysis, Google Cloud System, Django, Java_Script
categories: experience project
thumbnail: assets/img/AuditMate-Lite.png
---

**[Project] AuditMate-Lite: Google Cloud 배포부터 튜토리얼 제작까지의 여정**

기존에 개발했던 감사 보조 솔루션 **AuditMate**의 핵심 기능만을 담아 경량화한 **'AuditMate-Lite'** 버전을 출시했습니다. 이번 프로젝트는 단순한 기능 구현을 넘어, **Google Cloud Platform(GCP)** 을 활용한 실제 배포와 사용자 편의를 위한 **튜토리얼 제작**까지 전 과정을 직접 수행했다는 점에서 큰 의미가 있습니다.

**1. 첫 클라우드 배포 도전: Local에서 Cloud로**

가장 큰 도전은 **Google Cloud Service**를 활용한 배포 작업이었습니다.
이전까지는 로컬 환경에서의 개발에 익숙했기에, 클라우드 컴퓨팅 서비스를 이용해 실제 사용자가 접속 가능한 환경을 구축하는 것은 완전히 새로운 영역이었습니다.

  * **배포 환경:** Google Cloud Platform (GCP)
  * **주요 활용:** Cloud Run, Bucket, Cloud Build 등

처음 접해보는 콘솔 화면과 수많은 설정 값들, 그리고 IAM 권한 관리나 네트워크 설정 등 클라우드 서비스 내의 다양한 자원들을 이해하고 연결하는 과정에서 많은 시행착오를 겪었습니다. 
이 과정은 어렵기도 했지만, 서버 인프라와 배포 파이프라인에 대해 깊이 이해할 수 있는 값진 시간이었습니다.

**2. AuditMate-Lite 서비스 배포 완료**

우여곡절 끝에 안정적인 배포에 성공했습니다. 이제 별도의 설치 과정 없이 웹 브라우저를 통해 AuditMate-Lite의 기능을 체험해보실 수 있습니다.

**[AuditMate-Lite 서비스 바로가기](https://auditmate-793615282246.asia-northeast3.run.app/)**

**3. 사용자 경험(UX)을 위한 튜토리얼 제작**

서비스 배포 후, 단순히 "만들었다"는 것에 그치지 않고 **"사용자가 이 툴을 어떻게 받아들일까?"** 를 고민했습니다. 이를 위해 직접 사용 가이드를 담은 튜토리얼 영상을 제작했습니다.

영상을 기획하고 녹화하면서 개발자의 시선이 아닌 **사용자의 시선**에서 제 서비스를 바라볼 수 있었습니다.

  * *"이 부분은 설명 없이 직관적으로 이해가 될까?"*
  * *"워크플로우가 끊기지 않고 자연스러운가?"*

**[AuditMate-Lite 튜토리얼 영상]**

[![AuditMate-Lite 튜토리얼 영상](http://img.youtube.com/vi/W8GGaPYeKFU/0.jpg)](https://youtu.be/W8GGaPYeKFU)
<div class="caption">
    AuditMate-Lite 튜토리얼 영상
</div>

**4. 마치며**

이번 AuditMate-Lite 프로젝트는 **'개발(Development) - 배포(Deployment) - 문서화(Documentation)'** 로 이어지는 소프트웨어 생명주기의 주요 단계를 모두 경험해볼 수 있었던 뜻깊은 프로젝트였습니다. 특히 클라우드 환경에 대한 막연한 두려움을 없애고, 사용자 친화적인 서비스를 고민하는 개발자로 한 단계 성장할 수 있었습니다.

