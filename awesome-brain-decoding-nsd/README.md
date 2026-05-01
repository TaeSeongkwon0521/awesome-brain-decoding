# Awesome Brain Decoding with NSD

본 저장소는 fMRI 기반 Brain Decoding 연구를 정리한 Awesome List로, 특히 **Natural Scenes Dataset (NSD)** 를 활용한 **이미지 재구성(fMRI-to-Image Reconstruction)** 및 **멀티모달 뇌 신호 해석 연구**를 중심으로 논문, 데이터셋, 벤치마크, 코드 등을 체계적으로 정리한다.

최근 연구 흐름은 다음과 같은 방향으로 빠르게 발전하고 있다:

- Diffusion 기반 이미지 재구성
- CLIP / Vision-Language 모델과의 정렬
- Brain-to-Text / Brain-to-Caption
- Cross-Subject 일반화
- Retrieval-Augmented Decoding
- Mental Imagery Decoding

---

## 📚 목차

- [데이터셋 및 벤치마크](#-데이터셋-및-벤치마크)
- [서베이 논문](#-서베이-논문)
- [fMRI 기반 이미지 재구성](#-fmri-기반-이미지-재구성)
- [Diffusion 기반 재구성](#-diffusion-기반-재구성)
- [Vision-Language / CLIP 기반 디코딩](#-vision-language--clip-기반-디코딩)
- [Cross-Subject 디코딩](#-cross-subject-디코딩)
- [Brain-to-Text / Caption](#-brain-to-text--caption)
- [평가 방법](#-평가-방법)
- [고전 연구](#-고전-연구)

---

## 🧠 데이터셋 및 벤치마크

| 연도 | 이름 | 유형 | 설명 |
|---|---|---|---|
| 2022 | Natural Scenes Dataset (NSD) | Dataset | 대규모 7T fMRI 기반 자연 이미지 반응 데이터 |
| 2025 | NSD-Imagery | Dataset | mental imagery 확장 데이터셋 |
| 2026 | NSD-Synthetic | Dataset | OOD 일반화 평가를 위한 synthetic 데이터 |
| 2023 | Algonauts Challenge | Benchmark | NSD 기반 시각 자극 예측 챌린지 |

---

## 📖 서베이 논문

| 연도 | 논문 | 설명 |
|---|---|---|
| 2025 | A Survey of fMRI to Image Reconstruction | fMRI-to-image 재구성 연구 정리 |
| 2025 | Multimodal Brain Decoding Survey | 이미지, 텍스트 등 멀티모달 디코딩 |
| 2021 | Natural Image Reconstruction Survey | diffusion 이전 연구 흐름 |

---

## 🖼️ fMRI 기반 이미지 재구성

| 연도 | 논문 | 설명 |
|---|---|---|
| 2023 | MindEye | CLIP + diffusion 기반 재구성 및 retrieval |
| 2024 | MindEye2 | 적은 데이터로 subject 적응 |
| 2023 | Latent Diffusion Reconstruction | Stable Diffusion 기반 |
| 2023 | Brain-Diffuser | 자연 이미지 재구성 |
| 2023 | MindDiffuser | semantic + structural diffusion |

---

## 🔥 Diffusion 기반 재구성

| 연도 | 논문 | 설명 |
|---|---|---|
| 2024 | NeuralDiffuser | 저수준 시각 feature 활용 |
| 2025 | DynaDiff | 시간 변화 fMRI 활용 |
| 2025 | FreqSelect | 주파수 기반 분석 |
| 2025 | SEED | 구조 정보 강화 diffusion |

---

## 🔗 Vision-Language / CLIP 기반 디코딩

| 연도 | 논문 | 설명 |
|---|---|---|
| 2023 | BrainCLIP | 뇌 신호와 CLIP 정렬 |
| 2025 | BrainMCLIP | multi-layer feature 활용 |
| 2026 | PRISM | text space 기반 decoding |
| 2024 | CLIP-MUSED | multi-subject CLIP decoding |

---

## 👥 Cross-Subject 디코딩

| 연도 | 논문 | 설명 |
|---|---|---|
| 2024 | MindBridge | cross-subject framework |
| 2025 | MindTuner | semantic correction |
| 2026 | Brain-IT | brain interaction transformer |
| 2026 | Duala | subject + stimulus alignment |
| 2026 | PictorialCortex | zero-shot decoding |
| 2025 | ZEBRA | universal decoding |
| 2025 | BrainX | representation learning |

---

## 🧾 Brain-to-Text / Caption

| 연도 | 논문 | 설명 |
|---|---|---|
| 2023 | Brain Captioning | 이미지 + 텍스트 생성 |
| 2023 | UniBrain | unified framework |
| 2024 | UMBRAE | multimodal decoding |
| 2025 | MindLLM | fMRI-to-text |
| 2025 | BrainChat | multimodal transformer |

---

## 📊 평가 방법

| 연도 | 논문 | 설명 |
|---|---|---|
| 2025 | Multigranular Evaluation | 구조/의미/문맥 평가 |
| 2025 | BASIC Benchmark | 평가 프레임워크 |
| 2024 | Spurious Reconstruction | 실패 사례 분석 |

---

## 🏛️ 고전 연구

| 연도 | 논문 | 설명 |
|---|---|---|
| 2019 | Deep Image Reconstruction | 초기 DNN 기반 방법 |
| 2019 | From Voxels to Pixels | self-supervised |
| 2019 | Bayesian Multiview | 확률 기반 모델 |
| 2019 | GAN Reconstruction | GAN 기반 접근 |

---

## 🚀 목적

이 저장소는 다음을 목표로 한다:

- NSD 기반 Brain Decoding 연구 흐름 정리
- 최신 논문 빠르게 파악
- 연구 아이디어 탐색
- 재현 및 확장 연구 기반 제공

---

## 📌 TODO

- [ ] 논문 링크 추가
- [ ] 코드 링크 추가
- [ ] 카테고리 세분화 (Diffusion / CLIP / Retrieval 등)
- [ ] Survey 정리 강화

---

## 🤝 기여

Pull Request 및 Issue를 통한 기여를 환영합니다.
