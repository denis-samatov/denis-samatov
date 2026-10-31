# Selected engineering and research projects

Six public projects for reviewing my work as an ML Engineer, AI Engineer,
Research Engineer or Software Engineer. The links below identify the source
revision supporting each case study. They separate software contracts, recorded
experiments and operational evidence; none establishes a verified production
service or clinical qualification.

| Project | Best evidence of | Review entry point |
|---|---|---|
| [LocalDesk](#localdesk) | Applied ML, calibration and model lifecycle | Quality gates and immutable registry |
| [mcp-capguard](#mcp-capguard) | A focused typed library with negative controls | Client-visible capability boundary |
| [Yandex Workspace MCP](#yandex-workspace-mcp) | Integration and permission engineering | Authorization and isolation tests |
| [LLM Systems Lab](#llm-systems-lab) | Distributed training and inference mechanisms | Checkpoint and equivalence tests |
| [TBMD](#tbmd) | Numerical methods and scientific reproducibility | Nested validation and claims audit |
| [RuMed ICD benchmark](#rumed-icd-benchmark) | Comparative ML evaluation and negative results | Frozen splits, predictions and metrics |

## LocalDesk

**Problem.** Route text requests while retaining a human-review path for uncertain
predictions and preventing an unqualified model from becoming the active version.

**My contribution.** Task/configuration contracts, CPU classification and calibration,
quality gates, an immutable checksum-verified registry, and CLI/HTTP serving. The
[architecture](https://github.com/denis-samatov/localdesk/blob/50450a331ca3d1e5a33fbd8edbb9f52f7596fe79/docs/ARCHITECTURE.md)
explains the training/serving boundary and atomic promotion.

**Evidence.** The
[public-data CPU comparison](https://github.com/denis-samatov/localdesk/blob/50450a331ca3d1e5a33fbd8edbb9f52f7596fe79/reports/cpu-suite.md)
records accuracy, macro-F1 and abstention trade-offs on four datasets. Registry
and recovery behavior has
[executable tests](https://github.com/denis-samatov/localdesk/blob/50450a331ca3d1e5a33fbd8edbb9f52f7596fe79/tests/test_recovery_acceptance.py),
including rejection of invalid qualification metrics.

**Limits.** These are public benchmark and software-validation results. A target
organization's workload, model drift and operational acceptance require their own
pilot. Historical Qwen results do not establish that the full model is recoverable
or servable on this local CPU host.

**Resume wording.** “Built a local text-classification service with calibrated
abstention, reproducible model versions, promotion gates and recovery tests;
measured quality/coverage trade-offs on public datasets.”

## mcp-capguard

**Problem.** A server refactor can accidentally expose a write or destructive MCP
tool to a read-only configuration without causing an ordinary functional test to fail.

**My contribution.** A typed Python library, pytest plugin and CLI that evaluate
required/forbidden tools for configuration profiles, with an optional closed allowlist.
The
[public interface](https://github.com/denis-samatov/mcp-capguard/tree/411f74939947419c089eeb7ab71bfc3a4f7985b5/src/mcp_capguard)
is deliberately small.

**Evidence.** The
[Atlassian compatibility example](https://github.com/denis-samatov/mcp-capguard/blob/411f74939947419c089eeb7ab71bfc3a4f7985b5/examples/mcp_atlassian_pilot/README.md)
uses a real upstream factory and an in-memory client so the policy checks the
client-visible tool list. Isolated examples include negative controls that enable
an actual forbidden capability. The
[boundary write-up](https://github.com/denis-samatov/mcp-capguard/blob/411f74939947419c089eeb7ab71bfc3a4f7985b5/docs/client-visible-tools.md)
explains why inspecting an internal registry can miss request-time filtering.

**Limits.** Tool exposure tests complement runtime authorization; they do not
execute or authorize tools. Compatibility examples are not independent adoption.
The default source and historical GitHub v0.1.2 wheel have different API coverage;
follow the repository's explicit version boundary until a new release is published.

**Resume wording.** “Developed a typed pytest plugin and CLI for MCP capability
policies, including strict allowlists and isolated upstream compatibility examples
with negative controls.”

## Yandex Workspace MCP

**Problem.** Give agents useful Disk/Wiki access while keeping read, write and
destructive permissions explicit and protecting credentials and resource boundaries.

**My contribution.** Typed tools, configuration and authorization boundaries,
provider adapters, audit logging, bounded background jobs, and testable contracts.
See the
[architecture](https://github.com/denis-samatov/yandex-workspace-mcp/blob/cc2753d12e4235c548e1b4e90a5959cdfac0dce1/docs/architecture.md).

**Evidence.** The
[security test suite](https://github.com/denis-samatov/yandex-workspace-mcp/tree/cc2753d12e4235c548e1b4e90a5959cdfac0dce1/tests/security)
covers permissions, allowed roots, credentials, redirects/operation URLs and error
redaction. The
[permission demo](https://github.com/denis-samatov/yandex-workspace-mcp/blob/cc2753d12e4235c548e1b4e90a5959cdfac0dce1/examples/permission_demo.py)
shows denied writes making zero mocked upstream calls. A separate opt-in workflow
exists for live provider contracts.

**Limits.** Offline contracts and a local Redis acceptance run establish bounded
software behavior. Live provider parity, deployment-specific IAM, load and recovery
need independent qualification. A workflow definition alone proves none of those.

**Resume wording.** “Implemented an MCP integration for Yandex Disk/Wiki with
explicit permission gates, resource allowlisting, audit logging and security
regression tests.”

## LLM Systems Lab

**Problem.** Make distributed training, checkpoint recovery and inference scheduling
mechanisms inspectable and test them against simpler references.

**My contribution.** A small Llama-style model/trainer, single/DDP/FSDP2 execution,
DCP checkpoint handling, and a reference inference engine with paged KV storage,
continuous batching, speculative decoding and quantization experiments.

**Evidence.**
[Distributed equivalence tests](https://github.com/denis-samatov/llm-systems-lab/blob/88fad9674643c655218d11f4a4d1d2f809abaaa4/tests/test_distributed_equivalence.py)
and
[checkpoint tests](https://github.com/denis-samatov/llm-systems-lab/blob/88fad9674643c655218d11f4a4d1d2f809abaaa4/tests/test_checkpoint.py)
exercise actual processes, resume and resharding. The
[recorded CPU benchmark report](https://github.com/denis-samatov/llm-systems-lab/blob/88fad9674643c655218d11f4a4d1d2f809abaaa4/results/REPORT.md)
keeps hardware and workload context; ADRs explain observed failure modes.

**Limits.** CPU process semantics are distinct from multi-GPU scaling. Historical
Xeon/AMX timings do not transfer to Apple Silicon or production serving. The GPU
harness remains unqualified, and the small model is an engineering experiment.

**Resume wording.** “Implemented and tested distributed training/checkpoint and
reference LLM-serving mechanisms, using CPU equivalence, recovery and negative
controls; documented hardware-specific benchmark limits.”

## TBMD

**Problem.** Reconstruct spatiotemporal fields from sparse sensors while evaluating
the accuracy/compression trade-off without choosing parameters on held-out scenarios.

**My contribution.** Research software for Tucker/HOSVD decomposition, tensor QR
sensor selection and sparse reconstruction; the repository identifies the
collaborative paper's coauthors rather than treating the whole study as sole work.

**Evidence.** The
[Brugge study](https://github.com/denis-samatov/tensor-based-modal-decomposition-method/blob/f32502a5d3d8a8ef968dd43cc5e0e611ff5d5805/studies/brugge_sparse_sensing/README.md)
documents nested leave-one-scenario-out validation and competing formulations.
The
[reproducibility guide](https://github.com/denis-samatov/tensor-based-modal-decomposition-method/blob/f32502a5d3d8a8ef968dd43cc5e0e611ff5d5805/REPRODUCIBILITY.md)
and
[original numerical-claims audit](https://github.com/denis-samatov/tensor-based-modal-decomposition-method/blob/f32502a5d3d8a8ef968dd43cc5e0e611ff5d5805/docs/paper/audit/A1_original_numerical_claims_audit.md)
explicitly supersede unreproducible arXiv v1 quantitative results. Stored artifacts
and fresh algorithm execution are separate validation boundaries.

**Limits.** Original simulation exports require permitted access and have documented
provenance gaps. A checksum verifier is not an independent physical-data rerun.
The evidence does not support universal superiority, forecasting generalization
or production-service claims.

**Resume wording.** “Developed tensor-decomposition and sparse-reconstruction
research software; contributed nested scenario validation, competing baselines
and an explicit reproducibility/claims audit.”

## RuMed ICD benchmark

**Problem.** Compare medical coding approaches on the same Russian complaint
benchmark, including simple baselines and methods that fail to transfer well.

**My contribution.** Benchmark/evaluation pipelines for TF-IDF, prompted/retrieval
methods and local-model experiments; pinned data checksums, saved predictions,
bootstrap intervals and replay verifiers.

**Evidence.** The
[results table](https://github.com/denis-samatov/rumed-icd-llm/blob/5eb70676ea37eb1283c998244bfd2eba87da1d30/README.md#results)
reports TF-IDF Hit@1 **49.03%** and Hit@3 **72.63%** on **822** test records, ahead
of the recorded local-model methods. These are retrieval/coding hits, not macro-F1.
The
[Kev study](https://github.com/denis-samatov/rumed-icd-llm/blob/5eb70676ea37eb1283c998244bfd2eba87da1d30/docs/kev_research.md)
retains the negative transfer result. The
[replay acceptance guide](https://github.com/denis-samatov/rumed-icd-llm/blob/5eb70676ea37eb1283c998244bfd2eba87da1d30/docs/reproduction_acceptance.md)
separates saved-score verification from new inference.

**Limits.** The public holdout is reused. Record-level splits do not establish
patient-disjoint or external-institution validation. No clinical utility,
independent confirmation dataset, new paid API run or fresh GPU evaluation is
claimed by these case studies.

**Resume wording.** “Built a reproducible Russian ICD-coding benchmark with frozen
splits, paired baseline comparisons and bootstrap intervals; reported negative
LLM transfer results and clinical-validation limits.”

## How to read the evidence

Source links are frozen review anchors. Check each repository's current README
and CI before installing a newer revision. Model/provider behavior, operating
performance and clinical claims need evidence beyond code and stored reports.
Upstream contributions are listed separately in the profile README; linking an
upstream repository does not claim authorship of its implementation.
