<h1 align="left">Samatov Denis</h1>

**Machine Learning Engineer · Applied AI Technical Lead**

<!-- Theme-Sensitive Hero Banner -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="readmefile/dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="readmefile/light.svg">
  <img alt="Denis Samatov — ML Engineer / Applied AI Technical Lead" src="readmefile/dark.svg" width="100%">
</picture>

<br/>

## 🚀 About Me

I'm an **ML Engineer and Applied AI Technical Lead with 5+ years of experience** building RAG and document-intelligence platforms, medical imaging systems, and scientific ML tools. I lead teams of 3–5 engineers end to end — architecture, delivery, code and solution review, and ML engineering quality — and I still write the hard code myself: tensor methods, Bayesian inference, segmentation, radiomics, and production Python/FastAPI systems that run in CI/CD, not just in notebooks.

> If you're evaluating this profile as a recruiter, collaborator, or hiring manager: the short version is — I ship research-grade ML into production, I lead the team that ships it, and I publish/patent what we learn along the way.

**What I bring to a team:**
- 🧭 **Technical leadership** — currently leading architecture and delivery of *three* applied AI platforms simultaneously, coordinating 3–5 engineers per team, owning system boundaries and operational readiness.
- 🔬 **Research-to-production range** — equally comfortable deriving a Bayesian sensor-placement algorithm and shipping the FastAPI service, Redis workers, and CI gates that put it in front of users.
- 📈 **Measurable impact** — e.g. cut CT/MRI segmentation processing time by **40%** with an automated segmentation + manual ROI-correction pipeline.
- 🏛️ **Recognized track record** — 5+ publications (incl. arXiv), one officially registered software product, oral presentations at international conferences (Singapore, China), and multiple AI/ML competition wins.

---

## 🧑‍💻 Experience

**Machine Learning Engineer / Technical Lead** — *Analytics and Machine Learning Department, MSUU*
`Apr 2024 – Present`
- Lead architecture and delivery of three applied AI platforms — **CourseLLM**, **Modular RAG Platform**, and **LLM Adviser** — coordinating teams of 3–5 engineers and owning technical strategy, system boundaries, reviews, and operational readiness.
- Technical Lead for **LLM Adviser**, a five-developer agentic engineering knowledge platform; designed deterministic document processing, traceable outputs, asynchronous execution, and clean domain/infrastructure boundaries.
- Designed reusable ingestion/retrieval components: OCR, provenance preservation, hybrid retrieval, parent-document recovery, GraphRAG, reranking, and source-grounded generation.
- Built the execution layer with FastAPI, async workers, Redis, multi-provider LLM routing, automated evaluation, observability, security controls, and CI quality gates.
- Established repeatable ML/AI engineering practices through mentoring, code reviews, solution reviews, automated testing, and static analysis.

**Data Scientist / Research ML Engineer** — *Heriot-Watt TPU Center*
`Sep 2024 – Present`
- Develop tensor-based reduced-order models for high-dimensional spatiotemporal reservoir data, supporting forecasting and full-field reconstruction from sparse measurements.
- Design QR-based sparse-sensor placement and reconstruction workflows for incomplete observations, including geometry-aware and compressive-sensing variants.
- Published **NAB** as a reusable Python package with API/CLI workflows, automated tests, reproducible benchmarks, Bayesian parameter-space analysis, and convergence diagnostics.

**Machine Learning Engineer** — *Cardiology Research Institute*
`Mar 2021 – May 2025`
- Built an end-to-end CT/MRI segmentation and radiomics application with automated segmentation and manual ROI correction — **reduced processing time by 40%**.
- Trained U-Net and Attention U-Net models for medical image segmentation; applied radiomic texture analysis to support pathology detection and clinician review.
- Led development of **EPIFAT**, cardiac CT analysis software (anonymized preprocessing, segmentation, radiomics, manual ROI correction, validation, artifact tracking, cross-platform delivery) — officially registered as **Software No. 2025610317**.
- Implemented patient-level data separation, corrected metric aggregation, reproducible train/resume/test workflows, and versioned artifact lineage.

---

## 🏗️ Featured Work

**Applied AI platforms I lead in production** (institutional/client work — repos are private, happy to walk through architecture and results in a call):

| Project | What it is | Stack |
|---|---|---|
| **LLM Adviser** | Five-developer agentic engineering knowledge platform — deterministic document processing, traceable outputs, async execution | FastAPI, Redis, multi-provider LLM routing |
| **Modular RAG Platform** | Reusable ingestion/retrieval components — OCR, hybrid retrieval, GraphRAG, reranking, source-grounded generation | Python, hybrid retrieval, GraphRAG |
| **CourseLLM** | Applied AI platform delivered under the same technical leadership umbrella | Python, FastAPI |
| **EPIFAT** | Cardiac CT epicardial fat segmentation & radiomics tool — officially registered software (No. 2025610317) | PyTorch, U-Net / Attention U-Net, radiomics |
| **NAB** | Python package for tensor-based reduced-order modeling & QR sparse-sensor placement, with CLI, tests, and reproducible benchmarks | Python, Tucker/HOSVD, Bayesian inference |

**Public research code** — the methods behind the résumé, actually on GitHub:

- 🔗 [**tensor_based_modal_decomposition_method**](https://github.com/denis-samatov/tensor_based_modal_decomposition_method) — Tucker/HOSVD-based modal decomposition and QR sparse-sensor placement for reservoir field reconstruction; the working code behind the AI4X Singapore 2026 talk and the arXiv preprint.
- 🔗 [**radiomics**](https://github.com/denis-samatov/radiomics) — radiomic texture analysis of cardiac polar maps with ML, the research line that led into EPIFAT.

---

## 📚 Publications & Research

- *"Tensor-Based Modal Decomposition and Sparse Sensor Placement for the Brugge Field Simulation Model."* arXiv preprint, 2026.
- *"Approach to Identifying Key Areas for Further Reservoir Study Using Tensor-Based Modal Decomposition."* Conference paper, 2025.
- *"Automatic Segmentation of Epicardial Fat and Quantitative Evaluation of Radiomic Parameters in Cardiac CT."* Proc. XXI Int'l Conf. "Perspectives of Fundamental Sciences Development," 2024.
- *"Capabilities of Radiomic Analysis of Cardiac MRI Images in Cine Mode for Identifying Post-Infarction Areas."* Digital Diagnostics.
- *"Beam Parameters Restoration at the NICA Accelerator Complex Based on the Beam Position Monitor Data."* Proc. START, JINR, 2023.

## 🏆 Awards, Conferences & Recognition

- 🎤 Oral Presentation — *"Tensor-Based Modal Decomposition with QR Pivoting for Sparse Sensor Placement and Field Reconstruction,"* AI4X – Accelerate Conference, **Singapore**, 2026.
- 🎤 Accepted Presentation — *"Probabilistic Evaluation of Parameter Space Using Neighbourhood Algorithm Bayes,"* Data Intelligence in the Oil and Gas Industry, Nizhny Novgorod, 2026.
- 🌏 Participant, School-Conference on Tensor Methods in Mathematics and AI, **Shenzhen, China**, 2024.
- 🌏 Participant, Skoltech-HIT Summer School, **Harbin, China** (remote), 2025.
- 🥇 **Winner**, FINOdays AI/ML Track — 🏅 Special Nomination, National Technology Olympiad — 🏅 Prize Winner, MIPT AI/Math/Physics Hackathon.
- 🥈 Second-Degree Diploma — Cardiac CT segmentation & radiomics presentation, *Perspectives of Fundamental Sciences Development*, 2024.
- 📜 **Software No. 2025610317** — official state registration for EPIFAT (issued Jan 9, 2025).

## 🎓 Education

**Tomsk Polytechnic University**
- M.S., Applied Mathematics and Computer Science — 2024–2026
- B.S., Applied Mathematics and Computer Science — 2020–2024
- Diploma of Professional Retraining, Data Science and Machine Learning — 2023–2024

**Skoltech (Skolkovo Institute of Science and Technology)**
- Professional Development — Large Language Model-Based Agents, 2025
- Professional Development — Generative Models Based on Adversarial Learning, 2024

---

## 🛠️ Technical Skills

### 🤖 LLM / RAG
![RAG](https://img.shields.io/badge/RAG-0D9488?style=flat-square)
![GraphRAG](https://img.shields.io/badge/GraphRAG-10B981?style=flat-square)
![Hybrid Retrieval](https://img.shields.io/badge/Hybrid_Retrieval-34D399?style=flat-square)
![Vector Search](https://img.shields.io/badge/Vector_Search-0D9488?style=flat-square)
![Reranking](https://img.shields.io/badge/Reranking-10B981?style=flat-square)
![LLM Evaluation](https://img.shields.io/badge/LLM_Evaluation-34D399?style=flat-square)

### 🧠 ML / Computer Vision
![PyTorch](https://img.shields.io/badge/PyTorch-10B981?style=flat-square&logo=pytorch&logoColor=white)
![scikit--learn](https://img.shields.io/badge/scikit--learn-0D9488?style=flat-square&logo=scikitlearn&logoColor=white)
![U-Net](https://img.shields.io/badge/U--Net-34D399?style=flat-square)
![Semantic Segmentation](https://img.shields.io/badge/Semantic_Segmentation-0D9488?style=flat-square)
![Radiomics](https://img.shields.io/badge/Radiomics-10B981?style=flat-square)

### 📐 Scientific ML
![Tensor Decomposition](https://img.shields.io/badge/Tensor_Decomposition-0D9488?style=flat-square)
![Bayesian Inference](https://img.shields.io/badge/Bayesian_Inference-10B981?style=flat-square)
![MCMC](https://img.shields.io/badge/MCMC-34D399?style=flat-square)
![Compressive Sensing](https://img.shields.io/badge/Compressive_Sensing-0D9488?style=flat-square)

### ⚙️ Backend & Infrastructure
![Python](https://img.shields.io/badge/Python-0D9488?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-10B981?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-34D399?style=flat-square&logo=docker&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-0D9488?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-10B981?style=flat-square&logo=postgresql&logoColor=white)
![Git](https://img.shields.io/badge/Git-34D399?style=flat-square&logo=git&logoColor=white)

---

## 📈 GitHub Stats & Metrics

<!-- Theme-sensitive contribution activity graph -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph-eight.vercel.app/graph?username=denis-samatov&bg_color=030712&color=94A3B8&line=10B981&point=34D399&area_color=0D9488&area=true&hide_border=true&radius=12">
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-activity-graph-eight.vercel.app/graph?username=denis-samatov&bg_color=FFFFFF&color=475569&line=0D9488&point=10B981&area_color=E6FFFA&area=true&hide_border=true&radius=12">
    <img alt="Denis's Contribution Activity Graph" src="https://github-readme-activity-graph-eight.vercel.app/graph?username=denis-samatov&bg_color=030712&color=94A3B8&line=10B981&point=34D399&area_color=0D9488&area=true&hide_border=true&radius=12" width="100%" />
  </picture>
</p>

<!-- Theme-sensitive stats + top languages -->
<p align="left">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-stats-extended.vercel.app/api?username=denis-samatov&show_icons=true&hide_border=true&bg_color=030712&title_color=10B981&text_color=94A3B8&icon_color=34D399&border_color=0D9488">
    <source media="(prefers-color-scheme: light)" srcset="https://github-stats-extended.vercel.app/api?username=denis-samatov&show_icons=true&hide_border=true&bg_color=FFFFFF&title_color=0D9488&text_color=475569&icon_color=10B981&border_color=E2E8F0">
    <img alt="Denis's GitHub Stats" src="https://github-stats-extended.vercel.app/api?username=denis-samatov&show_icons=true&hide_border=true&bg_color=030712&title_color=10B981&text_color=94A3B8&icon_color=34D399&border_color=0D9488" width="48%" />
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-stats-extended.vercel.app/api/top-langs/?username=denis-samatov&layout=compact&hide_border=true&bg_color=030712&title_color=10B981&text_color=94A3B8&icon_color=34D399&border_color=0D9488">
    <source media="(prefers-color-scheme: light)" srcset="https://github-stats-extended.vercel.app/api/top-langs/?username=denis-samatov&layout=compact&hide_border=true&bg_color=FFFFFF&title_color=0D9488&text_color=475569&icon_color=10B981&border_color=E2E8F0">
    <img alt="Top Languages" src="https://github-stats-extended.vercel.app/api/top-langs/?username=denis-samatov&layout=compact&hide_border=true&bg_color=030712&title_color=10B981&text_color=94A3B8&icon_color=34D399&border_color=0D9488" width="48%" />
  </picture>
</p>

<!-- Theme-sensitive streak stats -->
<p align="left">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=denis-samatov&theme=dark&background=030712&stroke=0D9488&ring=10B981&fire=34D399&currStreakNum=10B981&currStreakLabel=94A3B8&sideNums=94A3B8&sideLabels=94A3B8&dates=6B7280">
    <source media="(prefers-color-scheme: light)" srcset="https://streak-stats.demolab.com?user=denis-samatov&theme=light&background=FFFFFF&stroke=E2E8F0&ring=0D9488&fire=10B981&currStreakNum=0D9488&currStreakLabel=475569&sideNums=475569&sideLabels=475569&dates=94A3B8">
    <img alt="GitHub Streak" src="https://streak-stats.demolab.com?user=denis-samatov&theme=dark&background=030712&stroke=0D9488&ring=10B981&fire=34D399&currStreakNum=10B981&currStreakLabel=94A3B8&sideNums=94A3B8&sideLabels=94A3B8&dates=6B7280" />
  </picture>
</p>

---

## 🤝 Let's Collaborate

I'm always open to talking about **RAG/LLM systems, medical imaging, scientific ML, and technical leadership roles** — whether that's a full-time role, research collaboration, or consulting.

[![GitHub](https://img.shields.io/badge/GitHub-denis--samatov-10B981?style=flat-square&logo=github&logoColor=white)](https://github.com/denis-samatov)
[![Telegram](https://img.shields.io/badge/Telegram-%40SamatovDS-0D9488?style=flat-square&logo=telegram&logoColor=white)](https://t.me/SamatovDS)
[![Email](https://img.shields.io/badge/Email-denissamatov470%40gmail.com-34D399?style=flat-square&logo=gmail&logoColor=white)](mailto:denissamatov470@gmail.com)
[![Download CV](https://img.shields.io/badge/Download_CV-0D9488?style=flat-square&logo=adobeacrobatreader&logoColor=white)](CV_SamatovDS.pdf)

---

<p align="center">
  ⭐ Thanks for stopping by — if something here is relevant to what you're building, reach out.
</p>
