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

- **8 merged PRs** across **deepset-ai/haystack** (25k★) and **run-llama/llama_index** (40k★)
- Built **ShardFlow** — distributed LLM inference hitting **28.10 TPS** on Qwen2.5-7B across free Kaggle GPUs over public WAN
- Cut RAG latency by **40%** and token costs by **60%** via Haystack 2.x migration + context windowing
- Reduced document ingestion from **70s → 27s** with parallel processing
- Published quantization stability research on Jetson Nano edge hardware — [preprint on Zenodo](https://doi.org/10.5281/zenodo.20776823)

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

### [Rossmann Sales Forecasting](https://github.com/rautaditya2606/rossmann)

Time-series sales forecasting on 1M+ rows of Rossmann store data. Feature engineering on promotions, holidays, and store metadata. Containerized and served via FastAPI.

`LightGBM` `FastAPI` `Docker` `Pandas`

**1M+ rows · containerized API · promotion and seasonality features**

</td>
</tr>
</table>

---

## Open Source

**8 merged PRs** across [deepset-ai/haystack](https://github.com/deepset-ai/haystack) (25k★) and [run-llama/llama_index](https://github.com/run-llama/llama_index) (40k★)

| PR | Repo | Fix |
|----|------|-----|
| [#11419](https://github.com/deepset-ai/haystack/pull/11419) | haystack | `DocumentLanguageClassifier` crash on blob-only docs — uncaught `TypeError` replaced with graceful fallback |
| [#11711](https://github.com/deepset-ai/haystack/pull/11711) | haystack | `RecursiveDocumentSplitter` silent metadata corruption — `split_idx_start` miscalculated with overlap enabled |
| [#11768](https://github.com/deepset-ai/haystack/pull/11768) | haystack | `RecursiveDocumentSplitter` overlap loss — `split_overlap` ignored on no-separator fallback path |
| [#11847](https://github.com/deepset-ai/haystack/pull/11847) | haystack | `FallbackChatGenerator` serialization — fallback chains lost on `to_dict()` roundtrip |
| [#11987](https://github.com/deepset-ai/haystack/pull/11987) | haystack | `EmbeddingBasedDocumentSplitter` — `split_idx_start` metadata inconsistency |
| [#12206](https://github.com/deepset-ai/haystack/pull/12206) | haystack | `PipelineBase.remove_component` — auto-variadic socket flag not reset on removal |
| [#12387](https://github.com/deepset-ai/haystack/pull/12387) | haystack | `PipelineBase.__eq__` — inverted `isinstance` check raised unhandled `AssertionError` on non-Pipeline comparison |
| [#12407](https://github.com/deepset-ai/haystack/pull/12407) | haystack | `AzureOpenAIChatGenerator.to_dict()` — `TypeError` when `response_format` is a plain dict |
| [#22167](https://github.com/run-llama/llama_index/pull/22167) | llama_index | `SemanticDoubleMergingSplitterNodeParser` — incorrect stopword removal |

---

## Currently

- Interning @ **AllCognix AI** — production RAG system on Haystack 2.x, EC2, Weaviate, Redis, Vault
- OSS contributions to **deepset-ai/haystack** — 8 merged PRs, ongoing
- Research paper targeting **Computers and Electronics in Agriculture** (Q1 Elsevier)
- Open to **ML Engineer / GenAI roles** — remote, India & international

---

<div align="center">
<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=100&section=footer" width="100%"/>

*Pune, India · B.Tech CSE (AI & Analytics) · MIT ADT University · 2028*

</div>
