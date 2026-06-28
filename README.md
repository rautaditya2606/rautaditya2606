<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=Aditya%20Raut&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=ML%20Engineer%20%C2%B7%20GenAI%20%C2%B7%20Edge%20AI&descAlignY=58&descSize=18&descColor=a78bfa" width="100%" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aditya-raut-3b4bba31b)
[![Portfolio](https://img.shields.io/badge/Portfolio-7C3AED?style=for-the-badge&logo=vercel&logoColor=white)](https://aditya-raut-alpha.vercel.app/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rautaditya2606@gmail.com)

<br/>

> *Building production ML systems that actually ship — from edge devices to cloud APIs.*

</div>

---

## About

GenAI Engineer Intern @ **AllCognix AI**, building RAG pipelines and production ML infrastructure on Haystack 2.x.

- 3 merged PRs in **deepset-ai/haystack** (25k★) — bugs caught through production use, not code review
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
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)

**Backend & Data**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)

</div>

---

## Open Source — deepset-ai/haystack

| PR | Fix |
|----|-----|
| [#11419](https://github.com/deepset-ai/haystack/pull/11419) | `DocumentLanguageClassifier` crash on blob-only docs (`content=None`) — uncaught `TypeError` replaced with graceful unmatched fallback |
| [#11711](https://github.com/deepset-ai/haystack/pull/11711) | `RecursiveDocumentSplitter` silent metadata corruption — `split_idx_start` miscalculated when `split_unit="word"/"token"` with overlap enabled; replaced unit-count arithmetic with actual overlap string character length |
| [#11768](https://github.com/deepset-ai/haystack/pull/11768) | `RecursiveDocumentSplitter` silent overlap loss — `split_overlap` ignored on no-separator fallback path in `_chunk_text()` |

---

## Featured Projects

<table>
<tr>
<td width="50%">

### [Haystack Diagnostics Engine](https://github.com/rautaditya2606/haystack-diagnostics)

Observability and diagnostics engine for Haystack 2.x RAG pipelines. Exposes document-store validation, pipeline inspection, retrieval-failure analysis, and structured debug bundle diffing via MCP.

`Haystack 2.x` `Weaviate` `MCP` `Python`

**6-class retrieval-failure taxonomy · 823-chunk live corpus · ~0.95s for 15 concurrent MCP requests**

</td>

<td width="50%">

### [Wheat Disease Intelligence Platform](https://github.com/rautaditya2606/wheat_detection)

Production ML platform with ConvNeXt-Tiny inference, CLIP-based input validation, OpenCV symptom overlays, GPT-4o mini recommendations, and a human-in-the-loop feedback pipeline.

`FastAPI` `ONNX Runtime` `PostgreSQL` `Docker` `OpenAI`

**88.46% accuracy · 75% model compression · 65ms CPU inference**

</td>
</tr>
<tr>
<td width="50%">

### [Edge-AI Wheat Disease Research](https://github.com/rautaditya2606/research_paper) · [Preprint](https://doi.org/10.5281/zenodo.20776823)

Quantization stability study across MobileNetV3-L, ResNet50, ConvNeXt-Tiny on Jetson Nano. Audited 14,154-image benchmark (11.6% cross-split leakage), recovered INT8 accuracy from 31.0% → 82.5%, proposed DES metric.

`PyTorch` `TensorRT` `ONNX Runtime` `OpenVINO` `Jetson Nano`

**54.5 FPS edge inference · entropy-calibrated TensorRT · leakage-audited benchmark**

</td>

<td width="50%">

### [NYC Taxi Fare Prediction](https://github.com/rautaditya2606/FastAPI_NYC)

Geospatial ML on 55M rows with Haversine distance features. Containerized and served via FastAPI.

`LightGBM` `FastAPI` `Docker`

**55M rows · containerized API**

</td>
</tr>
</table>

---

## Currently

- Interning @ **AllCognix AI** — production RAG system on Haystack 2.x, EC2, Weaviate, Redis, Vault
- OSS contributions to **deepset-ai/haystack** — 3 merged PRs, ongoing
- Research paper targeting **Computers and Electronics in Agriculture** (Q1 Elsevier)
- Open to **ML Engineer / GenAI roles** — remote, India & international

---

<div align="center">
<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=100&section=footer" width="100%"/>

*Pune, India · B.Tech CSE (AI & Analytics) · MIT ADT University · 2028*

</div>
