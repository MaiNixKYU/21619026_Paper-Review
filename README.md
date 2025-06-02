## Paper-Review: Generating Radiology Reports via Memory-driven Transformer (EMNLP 2020)
Zhihong Chen, Yan Song, Tsung-Hui Chang, Xiang Wan
https://arxiv.org/abs/2010.16056
---
# 1. 연구 목적
자동 방사선 판독 보고서 생성을 통한 의료 업무 효율화 도모

장문 및 구조화된 리포트 생성에서의 기존 모델 한계 극복 필요성 제기

# 2. 제안 기법
Relational Memory (RM) 기반 구조 설계

Memory-driven Conditional Layer Normalization (MCLN) 기법 도입

디코더 내부에서의 메모리 기반 정보 통합을 통한 문맥 정보 보존 강화

# 3. 모델 구조
이미지로부터 패치 단위 특성 추출 → 인코더를 통한 시각 정보 임베딩 → RM 및 MCLN을 포함한 디코더에서 문장 생성

기존 Transformer 기반 디코더에 메모리 셀 연동 구조 추가

보고서 문장 내 의학적 키워드 연계 및 장기 의존성 유지에 중점

# 4. 실험 설정
데이터셋: IU X-Ray, MIMIC-CXR

평가지표: BLEU, METEOR, ROUGE-L, CIDEr 등 자연어 생성 지표 + 임상 단위 정확성 평가(CheXpert Labeler)

# 5. 실험 결과
제안 모델의 자연어 지표 및 임상 정확도에서 기존 SOTA 대비 성능 향상 확인

특히 MIMIC-CXR 데이터셋에서 장문 보고서의 구조적 일관성과 의학적 용어 포괄성 개선 효과 입증

# 6. 기여 및 의의
메모리 기반 디코더를 활용한 의료 보고서 생성 정확도 향상

MIMIC-CXR 전체를 활용한 최초의 장문 리포트 생성 연구 수행

Transformer 계열 모델의 의료 도메인 적용 가능성 확장
