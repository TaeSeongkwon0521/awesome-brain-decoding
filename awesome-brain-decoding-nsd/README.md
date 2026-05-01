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
- [✅ Reading Checklist](#-reading-checklist)
- [🆕 Recent Core Papers: 2025–2026](#-recent-core-papers-20252026)
- [📌 Additional Candidates](#-additional-candidates)
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

## ✅ Reading Checklist

이 섹션은 논문을 읽었는지 관리하기 위한 체크리스트이다.  
논문을 읽은 뒤 `[ ]`를 `[x]`로 바꾸면 된다.

### Priority 0: 먼저 읽을 논문

- [ ] **Natural Scenes Dataset (NSD)**
- [ ] **MindEye**
- [ ] **High-Resolution Image Reconstruction with Latent Diffusion Models from Human Brain Activity**
- [ ] **Brain-Diffuser**
- [ ] **MindEye2**
- [ ] **MindBridge**
- [ ] **Brain Captioning**
- [ ] **UMBRAE**
- [ ] **PRISM / Seeing Through the Brain**
- [ ] **Multigranular Evaluation for Brain Visual Decoding / BASIC**

### Recent 2026 Papers

- [ ] **Brain-IT: Image Reconstruction from fMRI via Brain-Interaction Transformer**
- [ ] **PRISM / Seeing Through the Brain: Image Reconstruction of Visual Perception from Human Brain Signals**
- [ ] **SynMind: Reducing Semantic Hallucination in fMRI-to-Image Reconstruction**
- [ ] **PictorialCortex: Zero-Shot Cross-Subject fMRI-to-Image via Compositional Latent Modeling**
- [ ] **Duala: Dual-Level Alignment for Cross-Subject fMRI Decoding**
- [ ] **Seeing the Imagined: Latent Functional Alignment for Visual Imagery Decoding**

### Recent 2025 Papers

- [ ] **NSD-Imagery: A Benchmark Dataset for Extending Image Reconstruction Models to Mental Imagery**
- [ ] **ZEBRA: In-Context and Generative Pretraining for Zero-Shot Cross-Subject Neural Decoding**
- [ ] **BrainX: Learning to See Again — Universal Brain Decoding with Neuro-Geometric Representation Learning**
- [ ] **BrainMCLIP: Visual Decoding via Multi-layer Feature Guided CLIP**
- [ ] **DynaDiff: Single-stage Decoding of Images from Continuously Evolving fMRI**
- [ ] **FreqSelect: Frequency-Aware fMRI-to-Image Reconstruction**
- [ ] **FgB2I: Fine-grained Text Bridging for fMRI-to-Image Reconstruction**
- [ ] **MindTuner: Cross-Subject Visual Decoding with Visual Fingerprint and Semantic Correction**
- [ ] **Multigranular Evaluation for Brain Visual Decoding**
- [ ] **Exploring the Visual Feature Space for Multimodal Neural Decoding**
- [ ] **BrainROI: Unified Multimodal Brain Decoding via Cross-Subject Soft-ROI Fusion**
- [ ] **BrainExplore: Discovering Interpretable Visual Representations with fMRI**

### Additional Candidates

- [ ] **A 7T fMRI Dataset of Synthetic Images for Out-of-Distribution Modeling of Vision**
- [ ] **VoxelFormer: Reconstructing Stimuli from fMRI with Masked Autoencoder and Diffusion Model**
- [ ] **NeuroSwift: Enhancing fMRI-to-Image Reconstruction with Straight-Through Diffusion**
- [ ] **HI-DREAM: High-Resolution Image Reconstruction with Detailed Brain Visual Decoding**
- [ ] **MoRE-Brain: Multi-object Region Enhanced Brain Visual Decoding**
- [ ] **TROI: Text-Guided Reconstruction of Visual Stimuli from Human Brain Activity**
- [ ] **LaVCa: Linear Visual Concept Modeling of fMRI Responses**
- [ ] **SEED: Toward Efficient Image Reconstruction from fMRI via Structure-enhanced Denoising Diffusion**
- [ ] **MindLLM: A Subject-Agnostic and Training-Free Framework for fMRI-to-Text Decoding**
- [ ] **BrainChat: Decoding fMRI Brain Activity into Images and Text using Multimodal Transformers**
- [ ] **BRAINGUARD: Distilling Integrated Features for Robust Brain Decoding**
- [ ] **BOLDreams: Generative fMRI-to-Image Synthesis through Activation Guidance**
- [ ] **Scaling Laws for Neural Representation in fMRI Image Reconstruction**
- [ ] **SynBrain: Artificial Visual Cortex Enables Image Reconstruction from Brain Activity**
- [ ] **Rest2Visual: Reconstruction of Natural Visual Perception from Resting-State fMRI**

---

---

## 🆕 Recent Core Papers: 2025–2026

최근 NSD 기반 Visual Brain Decoding 연구는 단순한 subject-specific image reconstruction을 넘어, cross-subject 일반화, structured text space, semantic hallucination 완화, mental imagery decoding, dynamic fMRI decoding으로 확장되고 있다.

### 2026

| 연도 | 논문 | 키워드 | 추천 위치 | 설명 |
|---|---|---|---|---|
| 2026 | **Brain-IT: Image Reconstruction from fMRI via Brain-Interaction Transformer** | multi-subject, brain interaction transformer, image reconstruction, 1-hour adaptation | Cross-Subject / Multi-Brain Decoding | 여러 피험자의 fMRI를 함께 활용하는 Brain Interaction Transformer를 제안하고, 적은 fMRI 데이터로도 새로운 피험자에 적응하는 방향의 연구 |
| 2026 | **PRISM / Seeing Through the Brain: Image Reconstruction of Visual Perception from Human Brain Signals** | fMRI-to-image, structured text space, object-centric diffusion, semantic decoding | VLM/LLM-assisted Decoding | fMRI를 순수 vision feature가 아닌 structured text 또는 multimodal language space와 연결하는 연구 |
| 2026 | **SynMind: Reducing Semantic Hallucination in fMRI-to-Image Reconstruction** | semantic hallucination, sentence-level semantic description, diffusion | Semantic Alignment / Hallucination Reduction | diffusion 기반 brain reconstruction에서 발생하는 의미적 환각 문제를 완화하기 위한 연구 |
| 2026 | **PictorialCortex: Zero-Shot Cross-Subject fMRI-to-Image via Compositional Latent Modeling** | zero-shot, cross-subject, compositional latent | Zero-Shot / Cross-Subject Decoding | 피험자별 fine-tuning 없이 cross-subject fMRI-to-image decoding을 목표로 하는 연구 |
| 2026 | **Duala: Dual-Level Alignment for Cross-Subject fMRI Decoding** | cross-subject, stimulus alignment, subject alignment, retrieval | Cross-Subject Decoding | stimulus-level alignment와 subject-level alignment를 동시에 고려해 cross-subject decoding을 개선 |
| 2026 | **Seeing the Imagined: Latent Functional Alignment for Visual Imagery Decoding** | mental imagery, NSD-Imagery, latent alignment | Mental Imagery Decoding | 실제로 본 이미지뿐 아니라 머릿속으로 상상한 이미지에 대한 fMRI decoding 연구 |

### 2025

| 연도 | 논문 | 키워드 | 추천 위치 | 설명 |
|---|---|---|---|---|
| 2025 | **NSD-Imagery: A Benchmark Dataset for Extending Image Reconstruction Models to Mental Imagery** | NSD extension, mental imagery, benchmark | Datasets / Benchmarks | 기존 NSD의 perceived image decoding을 mental imagery decoding으로 확장하기 위한 벤치마크 |
| 2025 | **ZEBRA: In-Context and Generative Pretraining for Zero-Shot Cross-Subject Neural Decoding** | zero-shot, cross-subject, generative pretraining | Zero-Shot / Cross-Subject Decoding | 피험자별 적응 없이 새로운 피험자에게 일반화하는 zero-shot cross-subject brain decoding |
| 2025 | **BrainX: Learning to See Again — Universal Brain Decoding with Neuro-Geometric Representation Learning** | universal brain decoding, feature disentanglement, neuro-geometric learning | Universal Brain Decoding | 피험자 간 차이를 줄이고 공통적인 brain representation을 학습하는 universal decoding 계열 연구 |
| 2025 | **BrainMCLIP: Visual Decoding via Multi-layer Feature Guided CLIP** | CLIP, multi-layer alignment, parameter-efficient | CLIP-based Decoding | 저수준·고수준 시각 영역을 CLIP의 서로 다른 layer feature와 정렬하려는 연구 |
| 2025 | **DynaDiff: Single-stage Decoding of Images from Continuously Evolving fMRI** | time-resolved fMRI, single-stage diffusion, dynamic decoding | Time-Resolved / Dynamic Decoding | 정적인 평균 fMRI 표현이 아니라 시간에 따라 변화하는 fMRI 신호를 이미지 재구성에 활용 |
| 2025 | **FreqSelect: Frequency-Aware fMRI-to-Image Reconstruction** | frequency filtering, adaptive frequency selection, interpretability | Signal Processing / Frequency-Aware Decoding | fMRI 신호의 주파수 특성을 decoding에 반영 |
| 2025 | **FgB2I: Fine-grained Text Bridging for fMRI-to-Image Reconstruction** | fine-grained text, VLM caption, semantic bridge | Text-Bridge / VLM-assisted Decoding | fMRI와 이미지 사이에 세밀한 텍스트 표현을 bridge로 활용 |
| 2025 | **MindTuner: Cross-Subject Visual Decoding with Visual Fingerprint and Semantic Correction** | cross-subject, visual fingerprint, semantic correction | Cross-Subject Decoding | 새로운 피험자에 대해 제한된 fMRI 데이터만으로 decoding을 수행 |
| 2025 | **Multigranular Evaluation for Brain Visual Decoding** | evaluation, BASIC benchmark, structural, semantic, contextual | Evaluation / Benchmarking | brain visual decoding 결과를 구조적·의미적·문맥적 수준에서 평가 |
| 2025 | **Exploring the Visual Feature Space for Multimodal Neural Decoding** | MLLM, visual feature space, VINDEX, multimodal decoding | Feature Space / Multimodal Decoding | MLLM의 visual component가 fMRI decoding에 제공하는 feature space를 분석 |
| 2025 | **BrainROI: Unified Multimodal Brain Decoding via Cross-Subject Soft-ROI Fusion** | soft ROI, cross-subject, captioning, multimodal | ROI-based / Multimodal Decoding | subject 간 ROI 차이를 soft-ROI fusion으로 완화하고 image/caption decoding을 통합 |
| 2025 | **BrainExplore: Discovering Interpretable Visual Representations with fMRI** | interpretability, visual representation, natural-language explanation | Interpretability / Encoding Analysis | fMRI를 이용해 모델 내부 시각 표현의 의미를 해석 |

---

---

## 📌 Additional Candidates

아래 논문들은 최신 연구 흐름을 따라가기 위한 추가 후보 논문이다. 링크와 코드 저장소는 추후 보강한다.

| 논문 | 추천 위치 | 설명 |
|---|---|---|
| **A 7T fMRI Dataset of Synthetic Images for Out-of-Distribution Modeling of Vision** | Datasets / OOD Generalization | NSD와 연결되는 synthetic image 기반 OOD visual encoding/decoding 데이터셋 |
| **VoxelFormer: Reconstructing Stimuli from fMRI with Masked Autoencoder and Diffusion Model** | MAE / Transformer-based Decoding | Masked Autoencoder와 diffusion model을 활용한 fMRI stimulus reconstruction |
| **NeuroSwift: Enhancing fMRI-to-Image Reconstruction with Straight-Through Diffusion** | Diffusion-based Reconstruction | Straight-through diffusion 기반 fMRI-to-image reconstruction |
| **HI-DREAM: High-Resolution Image Reconstruction with Detailed Brain Visual Decoding** | High-Resolution Reconstruction | 세밀한 시각 정보를 반영하는 고해상도 brain visual decoding |
| **MoRE-Brain: Multi-object Region Enhanced Brain Visual Decoding** | Object-centric Decoding | 여러 객체 및 영역 정보를 강화한 brain visual decoding |
| **TROI: Text-Guided Reconstruction of Visual Stimuli from Human Brain Activity** | Text-Guided Decoding | 텍스트 정보를 활용한 visual stimulus reconstruction |
| **LaVCa: Linear Visual Concept Modeling of fMRI Responses** | Concept-based Encoding / Decoding | fMRI response를 시각 개념 단위로 모델링 |
| **SEED: Toward Efficient Image Reconstruction from fMRI via Structure-enhanced Denoising Diffusion** | Efficient Diffusion Decoding | 구조 정보를 강화한 denoising diffusion 기반 효율적 이미지 재구성 |
| **MindLLM: A Subject-Agnostic and Training-Free Framework for fMRI-to-Text Decoding** | Brain-to-Text / LLM-based Decoding | subject-agnostic, training-free fMRI-to-text decoding |
| **BrainChat: Decoding fMRI Brain Activity into Images and Text using Multimodal Transformers** | Brain-to-Image-and-Text | multimodal transformer 기반 image/text decoding |
| **BRAINGUARD: Distilling Integrated Features for Robust Brain Decoding** | Robust Decoding | robust brain decoding을 위한 feature distillation |
| **BOLDreams: Generative fMRI-to-Image Synthesis through Activation Guidance** | Generative Reconstruction | activation guidance 기반 fMRI-to-image synthesis |
| **Scaling Laws for Neural Representation in fMRI Image Reconstruction** | Scaling Laws | fMRI image reconstruction에서 model/data scaling law 분석 |
| **SynBrain: Artificial Visual Cortex Enables Image Reconstruction from Brain Activity** | Artificial Visual Cortex / Model-based Decoding | artificial visual cortex를 활용한 brain activity image reconstruction |
| **Rest2Visual: Reconstruction of Natural Visual Perception from Resting-State fMRI** | Resting-State to Visual Decoding | resting-state fMRI에서 natural visual perception을 재구성하려는 연구 |

---

## 🧠 데이터셋 및 벤치마크

Brain Decoding 연구에서 데이터셋은 모델 성능과 일반화 가능성을 결정하는 핵심 요소이다. 특히 NSD는 자연 이미지 자극에 대한 고해상도 7T fMRI 반응을 제공하므로, 최근 fMRI-to-image reconstruction 연구의 대표 벤치마크로 활용된다.

| 연도 | 이름 | 유형 | 설명 | 링크 |
|---|---|---|---|---|
| 2022 | **Natural Scenes Dataset (NSD)** | Dataset | 대규모 7T fMRI 기반 자연 이미지 반응 데이터셋 | [Website](https://naturalscenesdataset.org/) / [Paper](https://www.nature.com/articles/s41593-021-00962-x) |
| 2023 | **Algonauts Project 2023 Challenge** | Benchmark | NSD 기반 시각 자극에 대한 brain response prediction 챌린지 | [Paper](https://arxiv.org/abs/2301.03198) / [Challenge](https://algonautsproject.com/2023/index.html) / [Code](https://github.com/gifale95/algonauts_2023) |
| 2025 | **NSD-Imagery** | Dataset | Mental imagery decoding을 위한 NSD 확장 데이터셋 | [Paper](https://arxiv.org/abs/2506.06898) |
| 2026 | **NSD-Synthetic** | Dataset | OOD 일반화 평가를 위한 synthetic image 기반 NSD 확장 데이터셋 | [Paper](https://www.nature.com/articles/s41467-026-69345-9) / [Code](https://github.com/gifale95/NSD-synthetic) |

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
| 2024 | **MindEye2: Shared-Subject Models Enable fMRI-to-Image with 1 Hour of Data** | 여러 subject를 활용해 새로운 subject에 적은 데이터로 적응하는 framework | [Paper](https://arxiv.org/abs/2403.11207) / [Project](https://medarc-ai.github.io/mindeye2/) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2023 | **High-Resolution Image Reconstruction with Latent Diffusion Models from Human Brain Activity** | Stable Diffusion 기반 고해상도 이미지 재구성 | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Takagi_High-Resolution_Image_Reconstruction_With_Latent_Diffusion_Models_From_Human_Brain_CVPR_2023_paper.html) / [Project](https://sites.google.com/view/stablediffusion-with-brain/) / [Code](https://github.com/yu-takagi/StableDiffusionReconstruction) |
| 2023 | **Brain-Diffuser: Natural Scene Reconstruction from fMRI Signals using Generative Latent Diffusion** | VDVAE와 latent diffusion을 활용한 자연 이미지 재구성 | [Paper](https://www.nature.com/articles/s41598-023-42891-8) / [Code](https://github.com/ozcelikfu/brain-diffuser) |
| 2023 | **MindDiffuser: Controlled Image Reconstruction from Human Brain Activity with Semantic and Structural Diffusion** | semantic diffusion과 structural diffusion을 분리하여 이미지 재구성 | [Paper](https://arxiv.org/abs/2308.04249) / [Code](https://github.com/ReedOnePeck/MindDiffuser) |
| 2026 | **PRISM / Seeing Through the Brain: New Insights from Decoding Visual Stimuli with fMRI** | fMRI를 structured text space로 변환한 뒤 object-centric diffusion으로 이미지 재구성 | [Paper](https://openreview.net/forum?id=88ZLp7xYxw) |

---

## 🔥 Diffusion 기반 재구성

Diffusion model은 최근 fMRI-to-image reconstruction 성능 향상의 핵심 기술로 활용된다. 이 섹션은 latent diffusion, controllable diffusion, text-bridge, structured text space 등을 활용한 diffusion 기반 brain decoding 방법을 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **High-Resolution Image Reconstruction with Latent Diffusion Models from Human Brain Activity** | Stable Diffusion을 활용한 대표적인 brain-to-image reconstruction 연구 | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Takagi_High-Resolution_Image_Reconstruction_With_Latent_Diffusion_Models_From_Human_Brain_CVPR_2023_paper.html) / [Code](https://github.com/yu-takagi/StableDiffusionReconstruction) |
| 2023 | **Brain-Diffuser** | Generative latent diffusion 기반 자연 이미지 재구성 | [Paper](https://www.nature.com/articles/s41598-023-42891-8) / [Code](https://github.com/ozcelikfu/brain-diffuser) |
| 2023 | **MindDiffuser** | semantic / structural 정보를 분리한 diffusion 기반 reconstruction | [Paper](https://arxiv.org/abs/2308.04249) / [Code](https://github.com/ReedOnePeck/MindDiffuser) |
| 2026 | **PRISM / Seeing Through the Brain** | structured text space와 object-centric diffusion을 활용한 image reconstruction | [Paper](https://openreview.net/forum?id=88ZLp7xYxw) |

---

## 🔗 Vision-Language / CLIP 기반 디코딩

CLIP 및 Vision-Language Model은 fMRI 표현과 시각/언어 의미 공간을 연결하는 핵심 도구로 사용된다. 이 섹션은 brain signal을 CLIP latent space, text space, multimodal embedding space와 정렬하는 연구를 정리한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **BrainCLIP: Bridging Brain and Visual-Linguistic Representation via CLIP for Generic Natural Visual Stimulus Decoding** | CLIP을 brain-image-text 연결 공간으로 활용한 task-agnostic brain decoding | [Paper](https://arxiv.org/abs/2302.12971) / [Code](https://github.com/YulongBonjour/BrainCLIP) |
| 2023 | **MindEye** | fMRI를 CLIP latent space와 정렬하여 retrieval 및 reconstruction 수행 | [Paper](https://arxiv.org/abs/2305.18274) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2025 | **BrainMCLIP: Brain Image Decoding with Multi-Layer Feature Fusion of CLIP** | CLIP의 intermediate/final layer를 fMRI visual hierarchy와 정렬 | [Paper](https://arxiv.org/abs/2510.19332) |
| 2026 | **PRISM / Seeing Through the Brain** | fMRI를 vision-only feature가 아닌 structured text space와 연결 | [Paper](https://openreview.net/forum?id=88ZLp7xYxw) |

---

## 👥 Cross-Subject 디코딩

Cross-subject decoding은 특정 피험자에게만 과적합된 decoder의 한계를 극복하고, 새로운 피험자에게 일반화 가능한 brain decoding model을 만드는 것을 목표로 한다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2024 | **MindEye2: Shared-Subject Models Enable fMRI-to-Image with 1 Hour of Data** | Shared-subject model을 활용해 적은 데이터로 새로운 subject에 적응 | [Paper](https://arxiv.org/abs/2403.11207) / [Project](https://medarc-ai.github.io/mindeye2/) / [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| 2024 | **MindBridge: A Cross-Subject Brain Decoding Framework** | 하나의 model로 여러 subject의 fMRI를 decoding하기 위한 framework | [Paper](https://arxiv.org/abs/2404.07850) / [Project](https://littlepure2333.github.io/MindBridge) / [Code](https://github.com/littlepure2333/mindbridge) |
| 2025 | **MindTuner: Cross-Subject Visual Decoding with Visual Fingerprint and Semantic Correction** | visual fingerprint와 semantic correction을 활용한 cross-subject visual decoding | [Paper](https://arxiv.org/abs/2404.12630) |
| 2026 | **Brain-IT: Image Reconstruction from fMRI via Brain-Interaction Transformer** | Brain Interaction Transformer 기반 multi-subject image reconstruction | [Paper](https://openreview.net/forum?id=9KjXqkfbPw) |
| 2026 | **Duala: Dual-Level Alignment of Subjects and Stimuli for Cross-Subject fMRI Decoding** | stimulus-level consistency와 subject-level alignment를 함께 고려 | [Paper](https://arxiv.org/abs/2603.07625) / [Code](https://github.com/ShumengLI/Duala) |
| 2026 | **The Pictorial Cortex: Zero-Shot Cross-Subject fMRI-to-Image Reconstruction via Compositional Latent Modeling** | unseen subject에 대한 zero-shot cross-subject fMRI-to-image reconstruction | [Paper](https://arxiv.org/abs/2601.15071) |
| 2025 | **ZEBRA: Towards Zero-Shot Cross-Subject Generalization for Universal Brain Visual Decoding** | subject-specific adaptation 없이 unseen subject로 일반화하는 zero-shot visual decoding | [Paper](https://arxiv.org/abs/2510.27128) / [Code](https://github.com/xmed-lab/ZEBRA) |
| 2025 | **BrainX: A Universal Brain Decoding Framework with Feature Disentanglement and Neuro-Geometric Representation Learning** | subject-agnostic universal brain decoding framework | [Paper](https://dl.acm.org/doi/10.1145/3746252.3761402) / [Code](https://github.com/WENXUYUN/BrainX) |

---

## 🧾 Brain-to-Text / Brain-to-Caption

Brain decoding은 이미지 재구성뿐 아니라, 뇌 신호로부터 사람이 본 장면의 의미를 텍스트로 설명하는 방향으로 확장되고 있다.

| 연도 | 논문 | 설명 | 링크 |
|---|---|---|---|
| 2023 | **Brain Captioning: Decoding Human Brain Activity into Images and Text** | fMRI로부터 이미지와 텍스트를 함께 생성 | [Paper](https://arxiv.org/abs/2305.11560) |
| 2023 | **UniBrain: Unify Image Reconstruction and Captioning All in One Diffusion Model from Human Brain Activity** | Image reconstruction과 captioning을 하나의 diffusion framework로 통합 | [Paper](https://arxiv.org/abs/2308.07428) |
| 2024 | **UMBRAE: Unified Multimodal Brain Decoding** | Reconstruction, retrieval, captioning을 통합하는 multimodal brain decoding framework | [Paper](https://arxiv.org/abs/2404.07202) / [Project](https://weihaox.github.io/UMBRAE/) / [Code](https://github.com/weihaox/UMBRAE) |

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
| 2025 | **Multigranular Evaluation for Brain Visual Decoding / BASIC** | 구조, 의미, 문맥 수준에서 reconstruction 결과를 평가하는 multigranular benchmark | [Paper](https://arxiv.org/abs/2507.07993) / [Code](https://github.com/weihaox/BASIC) |
| 2025 | **Spurious Reconstruction from Brain Activity** | text-guided brain reconstruction의 일반화 한계와 hallucination 문제 분석 | [Paper](https://www.sciencedirect.com/science/article/pii/S0893608025003946) / [arXiv](https://arxiv.org/abs/2405.10078) |

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
| 2019 | **Deep Image Reconstruction from Human Brain Activity** | DNN feature 기반 image reconstruction의 대표 고전 연구 | [Paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006633) / [Code](https://github.com/KamitaniLab/DeepImageReconstruction) |

---

## 💻 코드 저장소

| 이름 | 설명 | 링크 |
|---|---|---|
| **MindEye / MindEye2** | NSD 기반 fMRI-to-image reconstruction 및 retrieval 코드 | [Code](https://github.com/MedARC-AI/fMRI-reconstruction-NSD) |
| **Stable Diffusion Reconstruction** | Takagi & Nishimoto CVPR 2023 reproduction code | [Code](https://github.com/yu-takagi/StableDiffusionReconstruction) |
| **Brain-Diffuser** | VDVAE + latent diffusion 기반 fMRI-to-image reconstruction 코드 | [Code](https://github.com/ozcelikfu/brain-diffuser) |
| **MindDiffuser** | semantic/structural diffusion 기반 reconstruction 코드 | [Code](https://github.com/ReedOnePeck/MindDiffuser) |
| **UMBRAE** | Unified multimodal brain decoding 코드 | [Code](https://github.com/weihaox/UMBRAE) |
| **MindBridge** | Cross-subject brain decoding 코드 | [Code](https://github.com/littlepure2333/mindbridge) |
| **Duala** | Dual-level cross-subject alignment 코드 | [Code](https://github.com/ShumengLI/Duala) |
| **ZEBRA** | Zero-shot cross-subject brain visual decoding 코드 | [Code](https://github.com/xmed-lab/ZEBRA) |
| **BrainX** | Universal brain decoding framework 코드 | [Code](https://github.com/WENXUYUN/BrainX) |
| **BASIC** | Multigranular evaluation framework 코드 | [Code](https://github.com/weihaox/BASIC) |
| **Deep Image Reconstruction** | Kamitani Lab 고전 reconstruction 코드 | [Code](https://github.com/KamitaniLab/DeepImageReconstruction) |
| **NSD Official** | Natural Scenes Dataset 공식 자료 | [Website](https://naturalscenesdataset.org/) |
| **Algonauts 2023 Devkit** | NSD 기반 Algonauts Challenge 코드 | [Code](https://github.com/gifale95/algonauts_2023) |

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
