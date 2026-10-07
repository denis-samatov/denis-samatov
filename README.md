<h1 align="center">Denis Samatov</h1>

<p align="center"><strong>Machine Learning Engineer &amp; Technical Lead · LLM/RAG systems &amp; evaluation · Medical imaging · Scientific ML</strong></p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="readmefile/dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="readmefile/light.svg">
  <img alt="Denis Samatov — Machine Learning Engineer & Technical Lead" src="readmefile/dark.svg" width="100%">
</picture>

> I build ML systems that can be checked: LLM/RAG assistants with release-blocking evaluation, medical image segmentation with patient-level validation, and scientific ML research software with documented reproducibility.

<p align="center">
  <a href="Denis_Samatov_CV_ML_Engineer.pdf"><img height="36" alt="CV (PDF)" src="https://img.shields.io/badge/CV%20(PDF)-0D9488?style=for-the-badge"></a>
  <a href="https://www.linkedin.com/in/denis-samatov/"><img height="36" alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-10B981?style=for-the-badge"></a>
  <a href="https://orcid.org/0009-0000-1821-323X"><img height="36" alt="ORCID" src="https://img.shields.io/badge/ORCID-0D9488?style=for-the-badge&amp;logo=orcid&amp;logoColor=white"></a>
  <a href="https://scholar.google.com/citations?user=GvQy91AAAAAJ"><img height="36" alt="Google Scholar" src="https://img.shields.io/badge/Google%20Scholar-10B981?style=for-the-badge&amp;logo=googlescholar&amp;logoColor=white"></a>
</p>


---

## 🧩 <code>Public projects</code>

| Project | Area | What the repository shows |
|---|---|---|
| [**RuMed ICD benchmark**](https://github.com/denis-samatov/rumed-icd-llm) | Medical NLP / LLM evaluation | Public Russian ICD-10 benchmark: TF-IDF vs zero/few-shot prompting vs retrieval, 822 test cases, bootstrap intervals and recorded token usage. LoRA training and vLLM serving results are pending. |
| [**TBMD**](https://github.com/denis-samatov/tensor-based-modal-decomposition-method) | Scientific ML | Tensor-based modal decomposition and sparse sensor placement library; nested leave-one-scenario-out Brugge benchmark; [reproducibility guide](https://github.com/denis-samatov/tensor-based-modal-decomposition-method/blob/main/REPRODUCIBILITY.md) including an audit of the superseded arXiv v1 results |
| [**NAB / nab-bayes**](https://pypi.org/project/nab-bayes/) | Bayesian inference | Installable Python wheel and source archive for MCMC/Gibbs appraisal over Voronoi cells; development repository is private. |
| [**Yandex Workspace MCP**](https://github.com/denis-samatov/yandex-workspace-mcp) | Agent tooling | MCP server for Yandex Disk & Wiki: 50+ typed tools, read-only by default, permission gates, audit logging, contract tests |
| [**LLM Adviser — case study**](https://github.com/denis-samatov/llm-adviser-case-study) | LLM / RAG architecture | Sanitized architecture of an engineering-knowledge platform in development (team of 5): deterministic ingestion, provenance, traceable retrieval |
| [**mcp-capguard**](https://github.com/denis-samatov/mcp-capguard) | Agent tooling | pytest plugin that asserts which tools each MCP configuration profile exposes |
| [**Agentic architectures**](https://github.com/denis-samatov/agentic-architectures) | LLM agents | 23 educational LangChain/LangGraph agent patterns, grouped by the failure each one addresses |
| [**OCR + LLM document pipeline**](https://github.com/denis-samatov/ocr-llm-document-pipeline) | Document AI | Docling / RapidOCR / Ollama pipeline on a synthetic fixture |


---

## 🔒 <code>Selected private work</code>

Source code is private (institutional or client work); code walkthroughs are available to hiring teams on request. The summaries below are author-reported; public repositories do not independently establish clinical validation or operational deployment.

<table>
<tr><td>

**EPIFAT** — state-registered cardiac CT software (No. 2025610317): Attention U-Net pericardium segmentation, reported Dice 0.91 in a single run with patient-level splitting; GUI + CLI, manual correction and radiomics. Training data and held-out predictions are private; this is a research result, not a clinical qualification claim.

</td></tr>
<tr><td>

**CourseLLM** — source-grounded RAG assistant in use; golden-QA release gate, streaming/queued API, concurrency control. Team project I lead.

</td></tr>
<tr><td>

**Housing knowledge-base RAG assistant** — in use; hybrid BM25 + dense retrieval with reranking, 37-query retrieval regression (Hit@5 1.00, MRR@10 0.89), RAGAS release gate. These scores describe the fixed regression set; broader retrieval quality and operating scale require separate evidence.

</td></tr>
</table>


---

## 🔀 <code>Merged upstream contributions</code>

- [weaviate/weaviate-python-client #2153](https://github.com/weaviate/weaviate-python-client/pull/2153) — generative DigitalOcean integration (merged 2026-09-07).
- [dragonflydb/dragonfly #8199](https://github.com/dragonflydb/dragonfly/pull/8199) — `FT.INFO` missing-index wording for RedisVL compatibility, with a regression test (merged 2026-09-01).
- [wandb/rai-toolkit #24](https://github.com/wandb/rai-toolkit/pull/24) — HR industry preset, dataset selection, docs and tests (merged 2026-09-02).
- [IBM/docling-pipelines #31](https://github.com/IBM/docling-pipelines/pull/31) — side-effect-free dry runs, with regression and control tests (merged 2026-09-09).


---

## 💼 <code>Experience</code>

- **Machine Learning Engineer / Technical Lead** (team of 3–4), Analytics and Machine Learning Department, MSUU — Apr 2024 – Present
- **Data Scientist / Research ML Engineer** (part-time; leads a 5-engineer LLM team), Heriot-Watt TPU Center — Sep 2024 – Present
- **Machine Learning Engineer**, Cardiology Research Institute — Mar 2021 – May 2026


---

## 🔬 <code>Research</code>

- [arXiv:2607.09687](https://arxiv.org/abs/2607.09687) — *Tensor-Based Modal Decomposition and Sparse Sensor Placement for the Brugge Field Simulation Model* (v1; revised manuscript with nested validation in preparation).
- Talks (2026): oral presentations at AI4X Accelerate (Singapore) and the 6th International Workshop on Mathematical Geophysics; presentation at Data Intelligence in the Oil and Gas Industry (Nizhny Novgorod); ePoster at the SPE Annual Caspian Technical Conference.
- Peer-reviewed cardiac MRI radiomics studies: [Digital Diagnostics, 2024](https://jdigitaldiagnostics.com/DD/article/view/630602); Russian Journal of Cardiology, 2026; Siberian Journal of Clinical and Experimental Medicine, 2026.


---

## ⚙️ <code>Stack</code>

<p align="center">
  <img src="readmefile/stack/python.svg" alt="Python" title="Python" width="28" height="28">
  <img src="readmefile/stack/pytorch.svg" alt="PyTorch" title="PyTorch" width="28" height="28">
  <img src="readmefile/stack/sklearn.svg" alt="scikit-learn" title="scikit-learn" width="28" height="28">
  <img src="readmefile/stack/langchain.svg" alt="LangChain" title="LangChain" width="28" height="28">
  <img src="readmefile/stack/langgraph.svg" alt="LangGraph" title="LangGraph" width="28" height="28">
  <img src="readmefile/stack/llamaindex.svg" alt="LlamaIndex" title="LlamaIndex" width="28" height="28">
  <img src="readmefile/stack/mcp.svg" alt="MCP" title="MCP" width="28" height="28">
  <img src="readmefile/stack/ollama.svg" alt="Ollama" title="Ollama" width="28" height="28">
  <img src="readmefile/stack/graphrag.svg" alt="GraphRAG" title="GraphRAG" width="28" height="28">
  <img src="readmefile/stack/bm25.svg" alt="BM25" title="BM25" width="28" height="28">
  <img src="readmefile/stack/ragas.svg" alt="RAGAS" title="RAGAS" width="28" height="28">
  <img src="readmefile/stack/qdrant.svg" alt="Qdrant" title="Qdrant" width="28" height="28">
  <img src="readmefile/stack/pgvector.svg" alt="pgvector" title="pgvector" width="28" height="28">
  <img src="readmefile/stack/postgres.svg" alt="PostgreSQL" title="PostgreSQL" width="28" height="28">
  <img src="readmefile/stack/redis.svg" alt="Redis" title="Redis" width="28" height="28">
  <img src="readmefile/stack/fastapi.svg" alt="FastAPI" title="FastAPI" width="28" height="28">
  <img src="readmefile/stack/docker.svg" alt="Docker" title="Docker" width="28" height="28">
  <img src="readmefile/stack/githubactions.svg" alt="GitHub Actions" title="GitHub Actions" width="28" height="28">
  <img src="readmefile/stack/prometheus.svg" alt="Prometheus" title="Prometheus" width="28" height="28">
  <img src="readmefile/stack/pyradiomics.svg" alt="PyRadiomics" title="PyRadiomics" width="28" height="28">
  <img src="readmefile/stack/ocr.svg" alt="OCR" title="OCR" width="28" height="28">
  <img src="readmefile/stack/tensor.svg" alt="tensor methods" title="tensor methods" width="28" height="28">
  <img src="readmefile/stack/mcmc.svg" alt="MCMC" title="MCMC" width="28" height="28">
</p>


---

## 📫 <code>Contact</code>

> [denissamatov470@gmail.com](mailto:denissamatov470@gmail.com) · Telegram [@SamatovDS](https://t.me/SamatovDS) · Tomsk, Russia — open to remote work and relocation.
