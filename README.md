<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║  ADITYA RAUT                                             ║
║  GenAI Engineer · OSS Contributor · Edge AI Researcher   ║
║  rautaditya2606@gmail.com                                ║
╚══════════════════════════════════════════════════════════╝
```

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aditya-raut-3b4bba31b)
[![Portfolio](https://img.shields.io/badge/Portfolio-7C3AED?style=flat-square&logo=vercel&logoColor=white)](https://aditya-raut-alpha.vercel.app/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rautaditya2606@gmail.com)

</div>

---

## What I actually build

Production RAG systems and ML pipelines — not tutorials, not toy datasets. Currently a GenAI Engineer Intern at **AllCognix AI** working on a multi-tenant document intelligence product built on Haystack 2.x, running on EC2 with Weaviate, Redis, RabbitMQ, Vault, and Cloudflare.

Three merged PRs in [deepset-ai/haystack](https://github.com/deepset-ai/haystack) (25k★) — crash fixes and silent-corruption bugs in core components, each caught via production use.

---

## Production impact @ AllCognix AI

```
metric                   before          after           delta
─────────────────────────────────────────────────────────────
RAG query latency        ~7.7s           ~4.6s           -40%
prompt tokens / query    ~5,000          ~2,000          -60%
batch ingestion time     ~70s            ~27s            -61%
```

**What drove the numbers:**
- Migrated from Verba to Haystack 2.x + GPT-4o with context windowing
- `ThreadPoolExecutor` parallelization across the ingestion pipeline
- Tesseract OCR preprocessing to eliminate vision token overhead on PDFs

---

## OSS: deepset-ai/haystack

| PR | Component | Fix |
|----|-----------|-----|
| [#11419](https://github.com/deepset-ai/haystack/pull/11419) | `DocumentLanguageClassifier` | Crash on `content=None` (blob-only docs) — uncaught `TypeError` replaced with graceful fallback |
| [#11711](https://github.com/deepset-ai/haystack/pull/11711) | `RecursiveDocumentSplitter` | Silent metadata corruption — `split_idx_start` miscalculated when `split_unit="word"/"token"` with overlap; replaced unit-count arithmetic with actual overlap string length |
| [#11768](https://github.com/deepset-ai/haystack/pull/11768) | `RecursiveDocumentSplitter` | Silent overlap loss — `split_overlap` ignored on no-separator fallback path in `_chunk_text()` |

All three found through production use, not code review.

---

## Projects

**[haystack-diagnostics](https://github.com/rautaditya2606/haystack-diagnostics)**
Observability engine for Haystack 2.x RAG pipelines. MCP-exposed tools for document-store validation, pipeline inspection, and retrieval-failure analysis with structured debug bundle diffing.
- Validated against live Weaviate corpus: 823 chunks, surfaced 195 duplicates (23.7%), 14 metadata inconsistencies, 8 anomalous chunks invisible during normal execution
- 6-class retrieval-failure taxonomy using `include_outputs_from` for single-pass diagnostics
- ~0.95s for 15 concurrent graph-inspection requests over MCP

`Haystack 2.x` `Weaviate` `MCP` `Python`

---

**[Wheat Disease Intelligence Platform](https://github.com/rautaditya2606/wheat_detection)** · [Live](https://wheat-detection.vercel.app/)
Production ML platform with ConvNeXt-Tiny (88.46% accuracy), CLIP-based input validation, OpenCV heuristic overlays, GPT-4o mini recommendations, and a human-in-the-loop feedback pipeline.
- INT8 ONNX quantization: 109MB → 27MB (75% compression), 0.18% accuracy drop, 65ms CPU inference
- Neon PostgreSQL + Cloudinary feedback loop; Dockerized for deployment

`PyTorch` `ONNX` `FastAPI` `Docker` `PostgreSQL` `OpenAI`

---

**[Edge AI Quantization Research](https://github.com/rautaditya2606/research_paper)** · [Preprint](https://zenodo.org/records/15307668)
Systematic quantization stability study across MobileNetV3-L, ResNet50, and ConvNeXt-Tiny on Jetson Nano.
- Audited 14,154-image wheat benchmark via MD5 + pHash deduplication — eliminated 11.6% cross-split leakage
- Recovered MobileNetV3 INT8 accuracy from 31.0% → 82.5% via entropy-calibrated TensorRT
- HardSwish/LayerNorm deployment patches for stable FP16/INT8; proposed DES metric; 54.5 FPS real-time inference

`PyTorch` `TensorRT` `ONNX Runtime` `OpenVINO` `Jetson Nano`

---

**[NYC Taxi Fare Prediction](https://github.com/rautaditya2606/FastAPI_NYC)**
LightGBM on 55M rows with Haversine distance and spatial-temporal features. Containerized and served via FastAPI.

`LightGBM` `FastAPI` `Docker`

---

## Stack

```
inference & training   PyTorch · ONNX Runtime · TensorRT · OpenVINO · Scikit-learn
genai / rag            Haystack 2.x · LangChain · OpenAI API · Anthropic API · Weaviate
backend                FastAPI · Flask · Python · PostgreSQL
infra / mlops          Docker · EC2 · Redis · RabbitMQ · HashiCorp Vault · Cloudflare · GitHub Actions
```

---

<div align="center">

B.Tech CSE (AI & Analytics) · MIT ADT University · 2028 · Pune, India

</div>
