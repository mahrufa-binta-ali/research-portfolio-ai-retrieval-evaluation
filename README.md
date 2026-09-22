# Research Portfolio: Healthcare AI Evaluation, Multimodal Learning, and Retrieval

I am a prospective PhD applicant in Computer Science interested in **healthcare AI evaluation, multimodal representation learning, contrastive learning, retrieval systems, and model failure analysis**.

My current work is organized around a central question:

> **When does a strong quantitative result actually indicate that an AI system has learned something reliable?**

Rather than treating training loss or a single benchmark score as sufficient evidence, I use controlled experiments to study retrieval quality, supervision quality, semantic false negatives, distribution difficulty, and evidence traceability.

---

## Selected Research Projects

### 1. Clinical RAG Evaluation Framework

**Repository:** [clinical-rag-evaluation-framework](https://github.com/mahrufa-binta-ali/clinical-rag-evaluation-framework)

An evidence-first retrieval evaluation framework for clinical RAG pipelines. The project deliberately evaluates retrieval and source traceability before adding answer generation.

**Methods and evaluation:**

- Sentence-transformer embeddings
- Token-aware document chunking
- ChromaDB vector retrieval
- Optional cross-encoder reranking
- Source Recall@K and MRR
- Keyword hit rate
- Evidence Phrase Recall@K
- Embedding-model comparison
- Reproducible tests and Docker/FastAPI deployment

The current benchmark is intentionally small and uses public/synthetic material; it should be interpreted as a retrieval-evaluation prototype rather than a clinical benchmark.

---

### 2. CXR-Text Bridge Retrieval

**Repository:** [cxr-text-bridge-retrieval](https://github.com/mahrufa-binta-ali/cxr-text-bridge-retrieval)

A controlled multimodal study of when image-text contrastive alignment forms, weakens, or collapses.

**Methods and evaluation:**

- Dual-encoder architecture
- L2-normalized shared embedding space
- Symmetric InfoNCE
- Bidirectional retrieval evaluation
- Recall@K and Lift@K
- Positive-pair similarity
- Controlled easy, shifted, and noisy conditions
- GPU experiments with mixed precision

The current benchmark uses synthetic CXR-like images and report-style embeddings. It is an alignment-behavior study, not a clinical-performance claim.

---

### 3. False-Negative-Aware Contrastive Learning

**Repository:** [fn-aware-contrastive-learning](https://github.com/mahrufa-binta-ali/fn-aware-contrastive-learning)

A controlled study of how semantic false negatives affect contrastive retrieval and how downweighting same-cluster negatives changes model behavior.

**Methods and evaluation:**

- Standard symmetric InfoNCE
- False-negative-aware weighted InfoNCE
- Clean, clustered, and noisy-pair conditions
- Multiple dataset sizes and weighting strengths
- Recall@K and Lift@K
- Positive-pair, same-cluster-negative, and different-cluster-negative similarity

The results are deliberately reported as mixed rather than as a universal improvement: the false-negative-aware objective helps some top-rank metrics in specific clustered settings but is not consistently better across all conditions.

---

### 4. Spectral Geometry Embedding Analysis

**Repository:** [spectral-geometry-embedding-analysis](https://github.com/mahrufa-binta-ali/spectral-geometry-embedding-analysis)

A diagnostic project for studying representation structure beyond aggregate retrieval metrics, including neighborhood preservation, clustering behavior, spectral structure, and failure patterns in embedding spaces.

---

### 5. FT-Transformer EHR Retrieval

**Repository:** [ft-transformer-ehr-retrieval](https://github.com/mahrufa-binta-ali/ft-transformer-ehr-retrieval)

A controlled tabular/EHR-style representation-learning benchmark comparing transformer-style and simpler encoders for retrieval alignment.

---

## Research Themes

### Rigorous Evaluation

I am interested in whether an evaluation protocol measures the capability it claims to measure. This includes distinguishing optimization success from retrieval success, checking evidence-level behavior rather than only source-level success, and identifying when aggregate metrics hide failure cases.

### Multimodal Representation Learning

I study shared representation spaces across image, text, and structured/tabular modalities, with particular interest in healthcare-oriented settings.

### Contrastive Learning Failure Modes

My experiments examine semantic false negatives, noisy supervision, weak pairing, and how loss design interacts with data structure.

### Reliability Under Shift and Noise

I use controlled synthetic experiments to isolate failure modes before making claims on real-world data. These studies are framed as method-behavior analyses, not as clinical validation.

---

## Technical Toolkit

**Programming and ML:** Python, PyTorch, Scikit-learn, NumPy, Pandas  
**Methods:** Contrastive learning, dual encoders, multimodal retrieval, tabular representation learning, embedding diagnostics  
**Evaluation:** Recall@K, Lift@K, MRR, evidence-level retrieval metrics, similarity diagnostics, controlled ablations  
**Engineering:** Git/GitHub, FastAPI, Docker, Hugging Face Spaces, reproducible experiment organization

---

## Research Approach

Across these projects I try to follow the same workflow:

1. Formulate a narrow research question.
2. Define a controlled experimental setup.
3. Establish useful baselines.
4. Separate training objectives from evaluation metrics.
5. Examine failure cases, not only best-case performance.
6. State limitations explicitly and avoid clinical or real-world claims that the experiment does not support.

My goal is to continue developing this direction through PhD research in **healthcare AI, multimodal learning, and rigorous model evaluation**.

---

## GitHub

[github.com/mahrufa-binta-ali](https://github.com/mahrufa-binta-ali)
