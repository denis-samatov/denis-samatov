<picture>
  <source media="(prefers-color-scheme: dark)" srcset="readmefile/dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="readmefile/light.svg">
  <img alt="Denis Samatov — machine learning engineer and technical lead working on applied AI, document systems, and scientific ML" src="readmefile/dark.svg" width="100%">
</picture>

# Denis Samatov

**Machine Learning Engineer & Technical Lead · Applied AI · Document Intelligence · Scientific ML**

I build software that makes complex documents and scientific data easier to work with. My public projects focus on permission-aware MCP integrations, traceable document workflows, and research code that others can inspect and reproduce.

[Explore the projects](#featured-projects) · [Research](#research) · [Contributions](#open-source-contributions) · [Get in touch](#connect)

## Featured projects

### MCP integrations and testing

- **[Yandex Workspace MCP](https://github.com/denis-samatov/yandex-workspace-mcp)** — tools for Yandex Disk and Wiki, with read-only defaults and explicit permission gates. Try the [offline permission demo](https://github.com/denis-samatov/yandex-workspace-mcp/blob/main/examples/permission_demo.py) without connecting an account.
- **[mcp-capguard](https://github.com/denis-samatov/mcp-capguard)** — a pytest plugin and CLI that check which tools an MCP server exposes under each configuration. The [FastMCP example](https://github.com/denis-samatov/mcp-capguard/tree/main/examples/fastmcp_example) shows a permission regression you can reproduce.

### Research and system design

- **[Tensor-Based Modal Decomposition](https://github.com/denis-samatov/tensor-based-modal-decomposition-method)** — tensor methods and sparse sensor placement for reservoir field reconstruction. Start with the [synthetic run](https://github.com/denis-samatov/tensor-based-modal-decomposition-method/blob/main/docs/examples/synthetic-run.md); the [reproducibility guide](https://github.com/denis-samatov/tensor-based-modal-decomposition-method/blob/main/REPRODUCIBILITY.md) separates public checks from data-dependent study runs.
- **[LLM Adviser case study](https://github.com/denis-samatov/llm-adviser-case-study)** — a sanitized account of document processing, retrieval, evaluation, and reliability decisions in an engineering knowledge system. It explains the architecture and its evidence limits; the application source is private.

For a smaller document-processing example, see the [OCR + LLM pipeline](https://github.com/denis-samatov/ocr-llm-document-pipeline). Its synthetic fixture demonstrates the workflow; real-document accuracy is not established there.

## Open-source contributions

Selected changes made upstream:

- [DragonflyDB #8199](https://github.com/dragonflydb/dragonfly/pull/8199) — RedisVL-compatible `FT.INFO` error wording and a regression test.
- [W&B RAI Toolkit #24](https://github.com/wandb/rai-toolkit/pull/24) — an HR industry preset, dataset selection, documentation, and focused tests.
- [Docling Pipelines #31](https://github.com/IBM/docling-pipelines/pull/31) — offline, side-effect-free dry runs for example tests.

Each pull request shows the exact change and review history.

## Research

- [Tensor-based modal decomposition and sparse sensor placement](https://arxiv.org/abs/2607.09687) — preprint and related public research software.
- [Cardiac MRI radiomics research](https://jdigitaldiagnostics.com/DD/article/view/630602) — publication record; medical code and data are not part of this public portfolio.
- [ORCID](https://orcid.org/0009-0000-1821-323X) — research identity and publication list.

## Connect

[LinkedIn](https://www.linkedin.com/in/denis-samatov/) · [ORCID](https://orcid.org/0009-0000-1821-323X) · [Telegram](https://t.me/SamatovDS) · [Email](mailto:denissamatov470@gmail.com) · [CV (PDF)](Denis_Samatov_Resume_ML_Engineer.pdf)

Issues and pull requests are welcome in the relevant project repository, especially for reproducibility problems and concrete tool-permission bugs.
