# Awesome Brain Decoding with NSD

본 저장소는 fMRI 기반 Brain Decoding 연구를 정리한 Awesome List로, 특히 **Natural Scenes Dataset (NSD)** 를 활용한 이미지 재구성(**fMRI-to-Image Reconstruction**) 및 멀티모달 뇌 신호 해석 연구를 중심으로 논문, 데이터셋, 벤치마크, 코드 등을 체계적으로 정리한다.

최근 Brain Decoding 연구는 다음과 같은 방향으로 빠르게 발전하고 있다.

- Diffusion 기반 이미지 재구성
- CLIP / Vision-Language 모델과의 정렬
- Brain-to-Text / Brain-to-Caption
- Cross-Subject 일반화
- Retrieval-Augmented Decoding
- Mental Imagery Decoding
- Brain Foundation Model 및 NeuroAI

---

## 📚 목차

- [🧠 데이터셋 및 벤치마크](#-데이터셋-및-벤치마크)
- [📖 서베이 논문](#-서베이-논문)
- [🖼️ fMRI 기반 이미지 재구성](#️-fmri-기반-이미지-재구성)
- [🔥 Diffusion 기반 재구성](#-diffusion-기반-재구성)
- [🔗 Vision-Language / CLIP 기반 디코딩](#-vision-language--clip-기반-디코딩)
- [👥 Cross-Subject 디코딩](#-cross-subject-디코딩)
- [🧾 Brain-to-Text / Brain-to-Caption](#-brain-to-text--brain-to-caption)
- [🧠 Mental Imagery Decoding](#-mental-imagery-decoding)
- [🔎 Retrieval-Augmented Decoding](#-retrieval-augmented-decoding)
- [🎞️ Dynamic / Video Decoding](#️-dynamic--video-decoding)
- [📊 평가 방법](#-평가-방법)
- [🧬 Encoding / Interpretability / NeuroAI](#-encoding--interpretability--neuroai)
- [🏛️ 고전 연구](#️-고전-연구)
- [💻 코드 저장소](#-코드-저장소)
- [📌 TODO](#-todo)

---

## 🧠 데이터셋 및 벤치마크

Brain Decoding 연구에서 데이터셋은 모델 성능과 일반화 가능성을 결정하는 핵심 요소이다. 특히 NSD는 자연 이미지 자극에 대한 고해상도 7T fMRI 반응을 제공하므로, 최근 fMRI-to-image reconstruction 연구의 대표 벤치마크로 활용된다.

| 연도 | 이름 | 유형 | 설명 | 링크 |
|---|---|---|---|---|
| 2022 | **Natural Scenes Dataset (NSD)** | Dataset | 대규모 7T fMRI 기반 자연 이미지 반응 데이터셋 | [Website](https://naturalscenesdataset.org/) / [Paper](https://www.nature.com/articles/s41593-021-00962-x) |
| 2023 | **Algonauts Project 2023 Challenge** | Benchmark | NSD 기반 시각 자극에 대한 brain response prediction 챌린지 | [Paper](https://arxiv.org/abs/2301.03198) |
| 2025 | **NSD-Imagery** | Dataset | Mental imagery decoding을 위한 NSD 확장 데이터셋 | [Paper](https://arxiv.org/abs/2506.06898) |
| 2026 | **NSD-Synthetic** | Dataset | OOD 일반화 평가를 위한 synthetic image 기반 NSD 확장 데이터셋 | [Paper](https://www.nature.com/articles/s41467-026-69345-9) |

---

## 📖 서베이 논문

이 섹션은 Brain Decoding 분야에 처음 진입하는 연구자가 전체 흐름을 빠르게 파악하기 위한 서베이 논문을 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2025 | **A Survey of fMRI to Image Reconstruction** | fMRI-to-image reconstruction 연구 흐름 정리 | [Paper](https://arxiv.org/abs/2502.16861) |
| 2025 | **A Survey on fMRI-based Brain Decoding for Reconstructing Multimodal Stimuli** | 이미지, 텍스트, 비디오 등 멀티모달 brain decoding 연구 정리 | [Paper](https://arxiv.org/abs/2503.15978) |
| 2021 | **Natural Image Reconstruction from fMRI Using Deep Learning: A Survey** | Diffusion 이전 deep learning 기반 reconstruction 연구 정리 | [Paper](https://www.frontiersin.org/articles/10.3389/fnins.2021.795488/full) |

---

## 🖼️ fMRI 기반 이미지 재구성

fMRI-to-image reconstruction은 사람이 본 시각 자극을 뇌 신호로부터 복원하는 과제이다. 최근 연구는 CLIP, diffusion model, vision-language model을 활용하여 의미적 일관성과 시각적 품질을 동시에 높이는 방향으로 발전하고 있다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **MindEye: fMRI-to-Image Reconstruction and Retrieval using Contrastive Learning and Diffusion Priors** | CLIP alignment와 diffusion prior를 활용한 NSD 기반 대표 reconstruction/retrieval 연구 | [Paper](https://arxiv.org/abs/2305.18274) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2024 | **MindEye2: Shared-Subject Models Enable fMRI-to-Image with 1 Hour of Data** | 여러 subject를 활용해 새로운 subject에 적은 데이터로 적응하는 framework | [Paper](https://arxiv.org/abs/2403.11207) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2023 | **High-Resolution Image Reconstruction with Latent Diffusion Models from Human Brain Activity** | Stable Diffusion 기반 고해상도 이미지 재구성 | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Takagi_High-Resolution_Image_Reconstruction_With_Latent_Diffusion_Models_From_Human_Brain_CVPR_2023_paper.html) |
| 2023 | **Brain-Diffuser: Natural Scene Reconstruction from fMRI Signals using Generative Latent Diffusion** | VDVAE와 latent diffusion을 활용한 자연 이미지 재구성 | [Paper](https://www.nature.com/articles/s41598-023-42891-8) |
| 2023 | **MindDiffuser: Controlled Image Reconstruction from Human Brain Activity with Semantic and Structural Diffusion** | semantic diffusion과 structural diffusion을 분리하여 이미지 재구성 | [Paper](https://arxiv.org/abs/2308.04249) |

---

## 🔥 Diffusion 기반 재구성

Diffusion model은 최근 fMRI-to-image reconstruction 성능 향상의 핵심 기술로 활용된다. 이 섹션은 latent diffusion, controllable diffusion, frequency-aware diffusion 등 다양한 diffusion 기반 방법을 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **High-Resolution Image Reconstruction with Latent Diffusion Models from Human Brain Activity** | Stable Diffusion을 활용한 대표적인 brain-to-image reconstruction 연구 | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Takagi_High-Resolution_Image_Reconstruction_With_Latent_Diffusion_Models_From_Human_Brain_CVPR_2023_paper.html) |
| 2023 | **Brain-Diffuser** | Generative latent diffusion 기반 자연 이미지 재구성 | [Paper](https://www.nature.com/articles/s41598-023-42891-8) |
| 2023 | **MindDiffuser** | semantic / structural 정보를 분리한 diffusion 기반 reconstruction | [Paper](https://arxiv.org/abs/2308.04249) |
| 2024 | **NeuralDiffuser** | Primary visual feature guidance를 활용한 controllable reconstruction | [Paper](https://arxiv.org/abs/2402.13809) |
| 2025 | **DynaDiff** | 시간적으로 변화하는 fMRI 신호를 활용한 single-stage image decoding | [Paper](https://arxiv.org/abs/2505.14556) |
| 2025 | **FreqSelect** | 주파수 정보를 활용한 fMRI-to-image reconstruction | [Paper](https://arxiv.org/abs/2505.12552) |
| 2025 | **FgB2I** | Fine-grained text bridge를 활용한 fMRI-to-image reconstruction | [Paper](https://arxiv.org/abs/2505.22150) |

---

## 🔗 Vision-Language / CLIP 기반 디코딩

CLIP 및 Vision-Language Model은 fMRI 표현과 시각/언어 의미 공간을 연결하는 핵심 도구로 사용된다. 이 섹션은 brain signal을 CLIP latent space, text space, multimodal embedding space와 정렬하는 연구를 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **MindEye** | fMRI를 CLIP latent space와 정렬하여 retrieval 및 reconstruction 수행 | [Paper](https://arxiv.org/abs/2305.18274) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2023 | **BrainCLIP: Bridging Brain and Visual-Linguistic Representation via CLIP** | Brain signal과 CLIP 기반 visual-linguistic representation 정렬 | 링크 추가 예정 |
| 2025 | **BrainMCLIP: Brain Image Decoding with Multi-Layer Feature Fusion of CLIP** | CLIP의 multi-layer feature를 활용한 brain image decoding | [Paper](https://arxiv.org/abs/2510.19332) |
| 2026 | **PRISM / Seeing Through the Brain** | fMRI를 structured text space로 변환하여 image reconstruction 수행 | [Paper](https://openreview.net/forum?id=88ZLp7xYxw) |
| 2024 | **CLIP-MUSED** | Multi-subject CLIP-guided semantic decoding | 링크 추가 예정 |

---

## 👥 Cross-Subject 디코딩

Cross-subject decoding은 특정 피험자에게만 과적합된 decoder의 한계를 극복하고, 새로운 피험자에게 일반화 가능한 brain decoding model을 만드는 것을 목표로 한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2024 | **MindEye2** | Shared-subject model을 활용해 적은 데이터로 새로운 subject에 적응 | [Paper](https://arxiv.org/abs/2403.11207) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2024 | **MindBridge: A Cross-Subject Brain Decoding Framework** | 하나의 model로 여러 subject의 fMRI를 decoding하기 위한 framework | [Paper](https://arxiv.org/abs/2404.07850) |
| 2025 | **MindTuner** | Visual fingerprint와 semantic correction을 활용한 cross-subject visual decoding | [Paper](https://arxiv.org/abs/2404.12630) |
| 2026 | **Brain-IT: Image Reconstruction from fMRI via Brain-Interaction Transformer** | Brain-interaction transformer 기반 multi-subject image reconstruction | [Paper](https://openreview.net/forum?id=9KjXqkfbPw) |
| 2026 | **Duala: Dual-Level Alignment for Cross-Subject fMRI Decoding** | Subject-level alignment와 stimulus-level alignment를 함께 고려 | [Paper](https://arxiv.org/abs/2603.07625) |
| 2026 | **PictorialCortex** | Zero-shot cross-subject fMRI-to-image reconstruction | [Paper](https://arxiv.org/abs/2601.15071) |
| 2025 | **ZEBRA** | Zero-shot cross-subject neural decoding | [Paper](https://arxiv.org/abs/2510.27128) |
| 2025 | **BrainX** | Universal brain decoding framework | 링크 추가 예정 |

---

## 🧾 Brain-to-Text / Brain-to-Caption

Brain decoding은 이미지 재구성뿐 아니라, 뇌 신호로부터 사람이 본 장면의 의미를 텍스트로 설명하는 방향으로 확장되고 있다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **Brain Captioning: Decoding Human Brain Activity into Images and Text** | fMRI로부터 이미지와 텍스트를 함께 생성 | [Paper](https://arxiv.org/abs/2305.11560) |
| 2023 | **UniBrain: Unify Image Reconstruction and Captioning from Human Brain Activity** | Image reconstruction과 captioning을 통합한 framework | [Paper](https://arxiv.org/abs/2308.07428) |
| 2024 | **UMBRAE: Unified Multimodal Brain Decoding** | Reconstruction, retrieval, captioning을 통합하는 multimodal brain decoding framework | [Paper](https://arxiv.org/abs/2404.07202) |
| 2025 | **MindLLM** | Subject-agnostic fMRI-to-text decoding framework | 링크 추가 예정 |
| 2025 | **BrainChat** | Multimodal transformer를 활용한 brain-to-image/text decoding | 링크 추가 예정 |
| 2025 | **BrainROI** | Cross-subject soft-ROI fusion 기반 multimodal brain decoding | [Paper](https://arxiv.org/abs/2512.20249) |

---

## 🧠 Mental Imagery Decoding

Mental imagery decoding은 실제로 본 이미지뿐 아니라 사람이 머릿속으로 상상한 이미지의 신경 표현을 decoding하는 과제이다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2025 | **NSD-Imagery** | NSD 기반 mental imagery decoding benchmark | [Paper](https://arxiv.org/abs/2506.06898) |
| 2026 | **Seeing the Imagined** | Latent functional alignment를 활용한 visual imagery decoding | [Paper](https://arxiv.org/abs/2604.15374) |
| 2019 | **Deep Image Reconstruction from Human Brain Activity** | Perceived image와 imagined image reconstruction을 모두 다룬 고전 연구 | [Paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006633) |

---

## 🔎 Retrieval-Augmented Decoding

Retrieval-Augmented Decoding은 brain signal만으로 이미지를 생성하는 대신, 외부 image-text database나 memory를 검색하여 reconstruction 품질을 보강하는 접근이다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2024 | **BrainRAM: Brain Retrieval-Augmented Module for Visual Decoding** | Retrieval-augmented module을 활용한 visual decoding | [Paper](https://openreview.net/forum?id=6iqKhyq1N4) |
| 2023 | **MindEye** | Reconstruction뿐 아니라 retrieval task도 수행 | [Paper](https://arxiv.org/abs/2305.18274) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |

---

## 🎞️ Dynamic / Video Decoding

이 섹션은 정적 이미지 reconstruction을 넘어, 시간적으로 변화하는 fMRI 또는 video stimulus decoding 연구를 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2025 | **DynaDiff** | Continuously evolving fMRI를 활용한 single-stage image decoding | [Paper](https://arxiv.org/abs/2505.14556) |
| 2023 | **MinD-Video / Cinematic Mindscapes** | fMRI 기반 video reconstruction 대표 연구 | [Paper](https://arxiv.org/abs/2305.11675) |
| 2025 | **DecoFuse** | Semantic, spatial, motion decomposition 기반 visual stimulus decoding | [Paper](https://arxiv.org/abs/2504.00432) |

---

## 📊 평가 방법

Brain decoding 결과는 시각적으로 그럴듯해 보여도 실제 의미가 다를 수 있다. 따라서 구조적 유사도, 의미적 일치성, 문맥 일관성, retrieval accuracy 등 다양한 평가 기준이 필요하다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2025 | **Multigranular Evaluation for Brain Visual Decoding** | 구조, 의미, 문맥 수준에서 reconstruction 결과 평가 | [Paper](https://arxiv.org/abs/2507.07993) |
| 2025 | **BASIC Benchmark** | Brain visual decoding 평가 framework | 링크 추가 예정 |
| 2024 | **Spurious Reconstruction from Brain Activity** | Brain decoding 결과의 실패 사례 및 허위 복원 문제 분석 | 링크 추가 예정 |
| 2026 | **NSD-Synthetic** | OOD generalization 평가용 synthetic image benchmark | [Paper](https://www.nature.com/articles/s41467-026-69345-9) |

---

## 🧬 Encoding / Interpretability / NeuroAI

이 섹션은 단순 reconstruction이 아니라, fMRI와 인공신경망 표현 간의 관계를 분석하거나 뇌의 시각 정보처리 구조를 해석하는 연구를 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2022 | **Brain Dissection: fMRI-trained Networks Reveal Spatial Selectivity in the Processing of Natural Images** | fMRI-trained network를 통해 cortical selectivity 분석 | 링크 추가 예정 |
| 2023 | **Brain Diffusion for Visual Exploration** | Generative model을 활용한 cortical discovery | 링크 추가 예정 |
| 2023 | **BrainSCUBA** | Visual cortex selectivity를 natural language caption으로 설명 | 링크 추가 예정 |
| 2025 | **BrainExplore** | fMRI를 활용한 interpretable visual representation discovery | [Paper](https://arxiv.org/abs/2512.08560) |
| 2025 | **LaVCa** | Linear visual concept modeling of fMRI responses | 링크 추가 예정 |
| 2024 | **BrainMAE** | Brain signal을 위한 self-supervised foundation model | 링크 추가 예정 |
| 2025 | **NeuroBind** | Neural signal을 위한 unified multimodal representation | 링크 추가 예정 |

---

## 🏛️ 고전 연구

이 섹션은 diffusion model 이전의 fMRI image reconstruction 연구 흐름을 이해하기 위한 기반 논문을 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2019 | **Deep Image Reconstruction from Human Brain Activity** | DNN feature 기반 image reconstruction의 대표 고전 연구 | [Paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006633) |
| 2019 | **From Voxels to Pixels and Back: Self-Supervision in Natural-Image Reconstruction from fMRI** | Self-supervised learning 기반 natural image reconstruction | [Paper](https://arxiv.org/abs/1907.02431) |
| 2019 | **Reconstructing Perceived Images from Human Brain Activities with Bayesian Deep Multiview Learning** | Bayesian multiview learning 기반 reconstruction | [Paper](https://pubmed.ncbi.nlm.nih.gov/30561354/) |
| 2019 | **Reconstructing Perceived Images by Visually-guided Cognitive Representation and Adversarial Learning** | GAN 기반 perceived image reconstruction | [Paper](https://arxiv.org/abs/1906.12181) |

---

## 💻 코드 저장소

| 이름 | 설명 | 링크 |
|---|---|---|
| **MindEye / MindEye2** | NSD 기반 fMRI-to-image reconstruction 코드 | [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| **NSD Official** | Natural Scenes Dataset 공식 자료 | [Website](https://naturalscenesdataset.org/) |
| **Algonauts 2023** | NSD 기반 challenge 자료 | [Website](http://algonauts.csail.mit.edu/) |

---

## 📌 TODO

- [ ] 각 논문의 공식 code repository 추가
- [ ] Project page 링크 추가
- [ ] 논문별 venue 정보 보강
- [ ] 논문별 task 태그 추가
- [ ] `README_EN.md` 영어 버전 추가
- [ ] Cross-subject decoding 논문 추가 조사
- [ ] Evaluation metric 정리 강화
- [ ] Brain foundation model 관련 논문 확장

---

## 🤝 기여

Pull Request 및 Issue를 통한 기여를 환영합니다.

논문 추가 시 다음 형식을 권장합니다.

```markdown
| 연도 | **논문 제목** | 한 줄 설명 | [Paper](링크) / [Code](링크) |
