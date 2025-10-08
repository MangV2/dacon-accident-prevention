

## 프로젝트 개요

건설 현장 사고 데이터를 기반으로 재발 방지 대책 및 향후 조치 계획을 자동으로 생성하는 AI 시스템입니다. 
RAG(Retrieval-Augmented Generation) 기반으로 104개의 건설안전지침 문서를 활용하여 
현장 맞춤형 안전 대책을 제공합니다.

## 주요 기능

- **데이터 증강**: BERT 기반 Random Masking Replacement로 훈련 데이터 확장
- **LLM 파인튜닝**: Ko-Gemma-2-9B 모델을 QLoRA로 효율적 학습
- **RAG 시스템**: FAISS 벡터 스토어 + Cross-Encoder 재순위화
- **자동 답변 생성**: 건설 현장 사고에 대한 맞춤형 안전 대책 생성

### 사용한 모델 
- **LLM**: `rtzr/ko-gemma-2-9b-it` (4-bit 양자화)
- **Embeddings**: `jhgan/ko-sbert-sts`
- **Cross-Encoder**: `bongsoo/albert-small-kor-cross-encoder-v1`
- **Data Augmentation**: `monologg/koelectra-base-v3-generator`
