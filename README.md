---
description: 실제 침해사고 사례를 AWS 환경에서 안전하게 재현하고, 로그·탐지·대응 흐름을 검증한 프로젝트입니다.
icon: house
layout:
  width: wide
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: false
  outline:
    visible: false
  pagination:
    visible: false
  metadata:
    visible: false
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: false
---

# 프로젝트 개요

### 프로젝트 소개

Team SC3N4R1O는 실제 침해사고 사례를 기반으로 공격 흐름을 분석하고, 이를 AWS 기반의 통제된 실습 환경에서 안전하게 재현하는 프로젝트를 진행했습니다.

본 프로젝트는 단순히 침해사고 사례를 조사하는 데 그치지 않고, 공격 과정에서 어떤 로그와 흔적이 남는지, 보안 담당자가 이를 어떻게 탐지하고 대응할 수 있는지 확인하는 데 초점을 두었습니다.

이를 위해 침해사고 시나리오 분석, AWS 재현 환경 구축, Red Team 공격 재현, 보안 솔루션 조합 테스트, 배치 암호화 구현, AI 기반 로그 분석 파이프라인을 하나의 흐름으로 연결했습니다.

{% hint style="info" %}
본 프로젝트는 실제 공격 수행을 목적으로 하지 않으며, 침해사고 대응 과정을 이해하기 위한 교육·연구 목적의 안전한 재현 실습입니다.
{% endhint %}

### 프로젝트 목표

본 프로젝트의 핵심 목표는 실제 침해사고를 바탕으로 공격부터 탐지, 분석, 대응까지 이어지는 전체 과정을 직접 재현하고 검증하는 것입니다.

특히 공격 성공 여부 자체보다, 공격이 발생했을 때 어떤 보안 로그가 남는지, 어떤 보안 통제가 먼저 탐지하는지, 탐지 공백은 어디에서 발생하는지를 확인하는 데 중점을 두었습니다.

### 전체 수행 흐름

1. 실제 침해사고 사례 조사 및 비교
2. 워밍업 사례를 통한 AWS 로그 분석 구조 학습
3. 롯데카드 침해사고 기반 메인 시나리오 선정
4. AWS 기반 침해사고 재현 환경 구축
5. Red Team 공격 흐름 안전 재현
6. WAF / Host Detection / Network Detection 조합별 실험
7. 배치 암호화 적용 전후 데이터 반출 상태 비교
8. AI 기반 로그 분석 및 대응 문서화

### 프로젝트 범위

<table><thead><tr><th width="159">구분</th><th>주요 내용</th></tr></thead><tbody><tr><td>사례 분석</td><td>실제 침해사고 사례를 조사하고 재현 가능성, AWS 적용 가능성, 탐지 실험 가능성을 기준으로 비교</td></tr><tr><td>워밍업 실습</td><td>쿠팡 유사 사례를 기반으로 유효한 인증정보를 이용한 대량 데이터 접근 흐름 분석</td></tr><tr><td>메인 시나리오</td><td>롯데카드 침해사고를 기반으로 외부 WAS 침투, 내부 접근, 데이터 수집 및 반출 흐름 재현</td></tr><tr><td>AWS 환경</td><td>VPC, ALB, WAS, Sink, S3, Athena, CloudWatch, CloudTrail 등을 활용한 실습 환경 구성</td></tr><tr><td>보안 실험</td><td>WAF, Host Detection, Network Detection 조합별 탐지 효과 비교</td></tr><tr><td>데이터 보호</td><td>배치 암호화를 적용하여 공격 시점에 따른 평문/암호문 반출 상태 비교</td></tr><tr><td>AI 분석</td><td>실험 로그를 기반으로 공격 타임라인, 탐지 근거, 대응 방향을 정리하는 분석 파이프라인 구성</td></tr></tbody></table>

### 프로젝트 방향성

1차 보고서에서는 프로젝트의 전체 방향과 침해사고 사례 선정 기준을 정리했고, 2차 보고서에서는 쿠팡 워밍업 사례를 통해 AWS에서 어떤 방식으로 침해 행위를 축소 재현할 수 있는지 구체화했습니다.

이후 프로젝트는 워밍업 실습에서 얻은 로그 수집·분석 경험을 바탕으로, 롯데카드 침해사고를 메인 시나리오로 확장하여 Full Stack 공격 재현과 보안 솔루션 조합 실험으로 이어졌습니다.&#x20;

&#x20;

&#x20;

&#x20;

&#x20;

&#x20;

&#x20;

&#x20;
