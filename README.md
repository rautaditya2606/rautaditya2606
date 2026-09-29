<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=Aditya%20Raut&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=ML%20Engineer%20%C2%B7%20GenAI%20%C2%B7%20Distributed%20Systems&descAlignY=58&descSize=18&descColor=a78bfa" width="100%" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aditya-raut-3b4bba31b)
[![Portfolio](https://img.shields.io/badge/Portfolio-7C3AED?style=for-the-badge&logo=vercel&logoColor=white)](https://aditya-raut-alpha.vercel.app/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rautaditya2606@gmail.com)

<br/>

> *Building production ML systems that actually ship — from edge devices to distributed GPU clusters.*

</div>

---

## About

GenAI Engineer Intern @ **AllCognix AI**, building RAG pipelines and production ML infrastructure on Haystack 2.x.

- **15 merged PRs** across **deepset-ai/haystack** (25k★), **run-llama/llama_index** (40k★), **mlflow**, **pydata/sparse** and **kubeflow/mcp-server**, plus 10 more in review across Haystack, Kubeflow, Jaeger and AiiDA
- Built **ShardFlow**, distributed LLM inference hitting **28.10 TPS** on Qwen2.5-7B across free Kaggle GPUs over public WAN
- Cut RAG latency by **40%** and token costs by **60%** via Haystack 2.x migration + context windowing
- Reduced document ingestion from **70s → 27s** with parallel processing
- Published quantization stability research on Jetson Nano edge hardware: [preprint on Zenodo](https://doi.org/10.5281/zenodo.20776823)

---

## Tech Stack

<div align="center">

**ML / Deep Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)

**MLOps & Deployment**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)

**Backend & Data**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)

</div>

---

## Projects

<table>
<tr>
<td width="50%">

### [ShardFlow](https://github.com/rautaditya2606/Shardflow)

High-performance distributed LLM inference framework. Partitions any HuggingFace transformer across N heterogeneous GPU machines over public internet WAN using neural speculative decoding, zero-copy binary tensor serialization, and a Rust TCP relay on AWS EC2.

`PyTorch` `HuggingFace` `CUDA Graphs` `AWS EC2` `Rust`

**28.10 TPS peak · 5.71x speedup · K=8 speculative decoding · 65% draft accept rate · Qwen2.5-7B across free Kaggle T4s**

</td>

<td width="50%">

### [Haystack Diagnostics Engine](https://github.com/rautaditya2606/haystack-diagnostics)

Observability and diagnostics engine for Haystack 2.x RAG pipelines. Exposes document-store validation, pipeline inspection, retrieval-failure analysis, and structured debug bundle diffing via MCP.

`Haystack 2.x` `Weaviate` `MCP` `Python`

**6-class retrieval-failure taxonomy · 823-chunk live corpus · ~0.95s for 15 concurrent MCP requests**

</td>
</tr>
<tr>
<td width="50%">

### [Wheat Disease Intelligence Platform](https://github.com/rautaditya2606/wheat_detection)

Production ML platform with ConvNeXt-Tiny inference, CLIP-based input validation, OpenCV symptom overlays, GPT-4o mini recommendations, and a human-in-the-loop feedback pipeline.

`FastAPI` `ONNX Runtime` `PostgreSQL` `Docker` `OpenAI`

**88.46% accuracy · 75% model compression · 65ms CPU inference**

</td>

<td width="50%">

### [Rossmann Sales Forecasting](https://github.com/rautaditya2606/Rossman-Deployed)

Time-series sales forecasting on 1M+ rows of Rossmann store data. Feature engineering on promotions, holidays, and store metadata. Containerized and served via FastAPI.

`LightGBM` `FastAPI` `Docker` `Pandas`

**1M+ rows · containerized API · promotion and seasonality features**

</td>
</tr>
</table>

---

## Open Source

## Open Source

**15 merged PRs** across [deepset-ai/haystack](https://github.com/deepset-ai/haystack) (25k★), [run-llama/llama_index](https://github.com/run-llama/llama_index) (40k★), [mlflow/mlflow](https://github.com/mlflow/mlflow), [pydata/sparse](https://github.com/pydata/sparse) and [kubeflow/mcp-server](https://github.com/kubeflow/mcp-server), with 10 more open across Haystack, Kubeflow, Jaeger and AiiDA.

### Merged

| PR | Repo | Change |
|----|------|--------|
| [#12529](https://github.com/deepset-ai/haystack/pull/12529) | haystack | `DocumentSplitter`: new `split_by="token"` mode using tiktoken |
| [#12485](https://github.com/deepset-ai/haystack/pull/12485) | haystack | `ComponentTool` deserialization support in OpenAI and Azure responses chat generators |
| [#12407](https://github.com/deepset-ai/haystack/pull/12407) | haystack | `AzureOpenAIChatGenerator.to_dict()`: `TypeError` when `response_format` is a plain dict |
| [#12387](https://github.com/deepset-ai/haystack/pull/12387) | haystack | `PipelineBase.__eq__`: unhandled `AssertionError` on non-Pipeline comparison |
| [#12206](https://github.com/deepset-ai/haystack/pull/12206) | haystack | `PipelineBase.remove_component`: auto-variadic socket state not restored on removal |
| [#11987](https://github.com/deepset-ai/haystack/pull/11987) | haystack | `EmbeddingBasedDocumentSplitter`: `split_idx_start` metadata not populated |
| [#11847](https://github.com/deepset-ai/haystack/pull/11847) | haystack | `FallbackChatGenerator`: nested chat generators lost on `to_dict()` roundtrip |
| [#11768](https://github.com/deepset-ai/haystack/pull/11768) | haystack | `RecursiveDocumentSplitter`: `split_overlap` ignored on no-separator fallback path |
| [#11711](https://github.com/deepset-ai/haystack/pull/11711) | haystack | `RecursiveDocumentSplitter`: wrong `split_idx_start` with word/token units and overlap |
| [#11419](https://github.com/deepset-ai/haystack/pull/11419) | haystack | `DocumentLanguageClassifier`: crash on docs with `content=None` |
| [#22167](https://github.com/run-llama/llama_index/pull/22167) | llama_index | `SemanticDoubleMergingSplitterNodeParser`: stopword removal now uses word tokenization |
| [#25862](https://github.com/mlflow/mlflow/pull/25862) | mlflow | `set_logged_model_tags`: bulk upsert for SQLite, PostgreSQL and MySQL |
| [#274](https://github.com/kubeflow/mcp-server/pull/274) | kubeflow/mcp-server | Unrestricted access not propagated when inheriting from parent persona |
| [#248](https://github.com/kubeflow/mcp-server/pull/248) | kubeflow/mcp-server | Return `RESOURCE_NOT_FOUND` on missing job in trainer monitoring tools |
| [#279](https://github.com/kubeflow/mcp-server/pull/279) | kubeflow/mcp-server | Make `_inject_trainer_hf_home` thread-safe for concurrent calls |
| [#955](https://github.com/pydata/sparse/pull/955) | pydata/sparse | `sparse.diagonal`: support for negative offsets, rectangular shapes and negative axes |
| [#960](https://github.com/pydata/sparse/pull/960) | pydata/sparse | `save_npz` / `load_npz`: support for CSR, CSC and DOK formats |

### In Review

| PR | Repo | Change |
|----|------|--------|
| [#12990](https://github.com/deepset-ai/haystack/pull/12990) | haystack | `Agent`: schema-constrained structured outputs with a recovery loop |
| [#12824](https://github.com/deepset-ai/haystack/pull/12824) | haystack | Redact `ImageContent` and `FileContent` in `ToolCallResult` trace dicts |
| [#806](https://github.com/kubeflow/sdk/pull/806) | kubeflow/sdk | `get_container_devices`: handle empty and memory-only resource limits |
| [#3175](https://github.com/kubeflow/spark-operator/pull/3175) | kubeflow/spark-operator | `ScheduledSparkApplication`: recover from `FailedValidation` once spec is fixed |
| [#199](https://github.com/kubeflow/pipelines-components/pull/199) | kubeflow/pipelines-components | Handle empty `metadata.yaml` in `check_component_freshness` |
| [#9658](https://github.com/jaegertracing/jaeger/pull/9658) | jaeger | ai-sidecar: point default MCP URL to query port 16686 |
| [#9511](https://github.com/jaegertracing/jaeger/pull/9511) | jaeger | ai-sidecar: join ACP prompt blocks with a delimiter to prevent token fusion |
| [#7598](https://github.com/aiidateam/aiida-core/pull/7598) | aiida-core | `JsonableData`: preserve `@module` and `@class` keys before `from_dict()` |

---

## Currently

- Interning @ **AllCognix AI**: production RAG system on Haystack 2.x, EC2, Weaviate, Redis, Vault
- OSS contributions to **deepset-ai/haystack** (10 merged PRs, more in review) and **Kubeflow** (mcp-server, sdk, spark-operator, pipelines-components)
- Research paper targeting **Computers and Electronics in Agriculture** (Q1 Elsevier)
- Open to **ML Engineer / GenAI roles**: remote, India & international

---

<div align="center">
<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=100&section=footer" width="100%"/>

*Pune, India · B.Tech CSE (AI & Analytics) · MIT ADT University · 2028*

</div>
