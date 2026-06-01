# Research Portfolio: AI Retrieval, Multimodal Learning, and Model Evaluation

I am a prospective PhD applicant in Computer Science interested in multimodal learning, retrieval systems, representation learning, contrastive learning, and evaluation of model behavior.

This repository connects my research-oriented GitHub projects into one clear portfolio. The goal is to show not only what I built, but also what research questions I explored, what experiments I ran, what metrics I measured, and what I learned from the results.

---

## Research Direction

My current work focuses on one broad question:

> How can we build and evaluate AI systems that learn meaningful alignment across different types of data?

I explore this through controlled experiments on:

- multimodal retrieval
- contrastive learning
- false negatives in representation learning
- noisy and weakly matched pairs
- tabular and medical-data representation learning
- embedding-space geometry
- evaluation beyond simple accuracy

---

## Main Research Questions

### 1. Multimodal Alignment

How do models learn shared representations between different data types such as images, text, and tabular clinical features?

Related projects:

- [CXR-Text Bridge Retrieval](https://github.com/subhaaniii/cxr-text-bridge-retrieval)
- [FT-Transformer EHR Retrieval](https://github.com/subhaaniii/ft-transformer-ehr-retrieval)

---

### 2. Pair Quality and Weak Supervision

How does the quality of positive pairs affect contrastive retrieval performance?

In many real-world settings, perfectly matched pairs are expensive or unavailable. I study how pseudo-pairs, noisy pairs, and weak matching strategies affect retrieval behavior.

Related project:

- [Propensity Matching for Multimodal Pairs](https://github.com/subhaaniii/propensity-matching-multimodal-pairs)

---

### 3. False Negatives in Contrastive Learning

What happens when contrastive learning treats semantically similar samples as negatives?

This question is important because false negatives can damage representation quality, especially in medical, tabular, and multimodal datasets where similarity is not always obvious from labels.

Related project:

- [False-Negative-Aware Contrastive Learning](https://github.com/subhaaniii/fn-aware-contrastive-learning)

---

### 4. Embedding Geometry and Model Diagnostics

Can embedding-space geometry reveal failures that retrieval metrics alone may hide?

I study whether model embeddings are well-structured, collapsed, noisy, over-separated, or distorted using spectral and geometric diagnostics.

Related project:

- [Spectral Geometry Embedding Analysis](https://github.com/subhaaniii/spectral-geometry-embedding-analysis)

---

### 5. Applied AI System Building

Alongside research experiments, I also build applied AI systems to strengthen my software engineering ability and end-to-end product thinking.

Related project:

- [Sumora](https://github.com/subhaaniii/sumora)

---

## Portfolio Map

| Research Theme | Project | Main Question | Methods / Tools | Evaluation |
|---|---|---|---|---|
| Multimodal image-text retrieval | [CXR-Text Bridge Retrieval](https://github.com/subhaaniii/cxr-text-bridge-retrieval) | Can contrastive learning align chest X-ray images and text reports? | Dual encoder, contrastive learning, retrieval evaluation | Recall@K, Lift@K, positive-pair similarity |
| Tabular-medical retrieval | [FT-Transformer EHR Retrieval](https://github.com/subhaaniii/ft-transformer-ehr-retrieval) | Does a transformer-style tabular encoder improve retrieval alignment? | FT-Transformer-style encoder, MLP baseline, synthetic EHR setup | Recall@K, Lift@K, sample-size analysis |
| Weak pair construction | [Propensity Matching for Multimodal Pairs](https://github.com/subhaaniii/propensity-matching-multimodal-pairs) | How does pair quality affect contrastive retrieval? | Propensity matching, pseudo-pairs, noisy pairs | Pair precision, group precision, Recall@K, Lift@K |
| Contrastive learning failure modes | [False-Negative-Aware Contrastive Learning](https://github.com/subhaaniii/fn-aware-contrastive-learning) | How do false negatives affect representation learning? | Contrastive loss variants, controlled experiments | Retrieval metrics, similarity behavior |
| Embedding diagnostics | [Spectral Geometry Embedding Analysis](https://github.com/subhaaniii/spectral-geometry-embedding-analysis) | Can geometry reveal hidden representation failures? | Spectral analysis, embedding visualization, diagnostic metrics | Geometry metrics, failure-mode analysis |
| Applied AI system | [Sumora](https://github.com/subhaaniii/sumora) | Can I build a usable AI-assisted movie discovery platform? | Next.js, TypeScript, TMDB, OMDb, chatbot interface | Product functionality, search quality, UI behavior |

---

## Skills Demonstrated

### Research Skills

- Formulating research questions
- Designing controlled experiments
- Comparing baselines
- Running ablation-style studies
- Evaluating retrieval systems
- Analyzing model failure modes
- Writing research-style documentation
- Connecting experiments to broader research problems

### Machine Learning Skills

- Contrastive learning
- Dual-encoder retrieval
- Multimodal representation learning
- Tabular representation learning
- Embedding-space analysis
- Evaluation with Recall@K and Lift@K
- Synthetic data generation for controlled experiments
- Medical AI experimentation

### Engineering Skills

- Python
- PyTorch
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Next.js
- TypeScript
- Git and GitHub
- Reproducible experiment organization

---

## How These Projects Connect

These projects are not separate random repositories. They form one connected research direction.

The central idea is:

> Retrieval models can look successful from one metric but still fail because of noisy pairs, weak supervision, false negatives, poor architecture choice, or distorted embedding geometry.

My portfolio studies this problem from different angles:

1. **Data pairing**  
   How reliable are the positive pairs used for training?

2. **Model architecture**  
   Does the encoder architecture improve alignment?

3. **Loss behavior**  
   How does contrastive learning behave when negatives are imperfect?

4. **Evaluation**  
   Are Recall@K and Lift@K enough, or do we need deeper diagnostics?

5. **Geometry**  
   What does the learned embedding space actually look like?

Together, these experiments help me build a stronger foundation for future PhD research in multimodal learning, medical AI, and trustworthy model evaluation.

---

## Current Research Interests

I am especially interested in:

- multimodal learning
- medical AI
- contrastive representation learning
- retrieval systems
- weak supervision
- noisy labels and noisy pairs
- embedding-space diagnostics
- trustworthy AI evaluation
- AI for healthcare and scientific data

---

## Future Work

My next planned improvements are:

- Apply the retrieval pipeline to a real public multimodal dataset
- Add stronger baselines and ablation studies
- Compare different contrastive loss variants
- Add more visualization of embedding spaces
- Improve reproducibility with fixed experiment scripts
- Write paper-style reports for the strongest projects
- Study uncertainty, robustness, and failure detection in multimodal retrieval

---

## Selected Projects

### 1. CXR-Text Bridge Retrieval

Repository: [cxr-text-bridge-retrieval](https://github.com/subhaaniii/cxr-text-bridge-retrieval)

This project studies image-text retrieval using chest X-ray images and associated text representations. It uses contrastive learning to test whether a model can learn a shared embedding space between visual and textual medical information.

Main focus:

- multimodal retrieval
- image-text alignment
- contrastive learning
- Recall@K and Lift@K evaluation

---

### 2. FT-Transformer EHR Retrieval

Repository: [ft-transformer-ehr-retrieval](https://github.com/subhaaniii/ft-transformer-ehr-retrieval)

This project studies whether a transformer-style tabular encoder can improve retrieval alignment compared with simpler baselines.

Main focus:

- tabular representation learning
- EHR-style synthetic data
- FT-Transformer-style encoder
- model comparison

---

### 3. Propensity Matching for Multimodal Pairs

Repository: [propensity-matching-multimodal-pairs](https://github.com/subhaaniii/propensity-matching-multimodal-pairs)

This project studies how pseudo-pair construction affects contrastive retrieval. It explores whether better pair matching can improve downstream retrieval behavior.

Main focus:

- weak supervision
- pseudo-pair construction
- noisy positive pairs
- retrieval robustness

---

### 4. False-Negative-Aware Contrastive Learning

Repository: [fn-aware-contrastive-learning](https://github.com/subhaaniii/fn-aware-contrastive-learning)

This project studies a common problem in contrastive learning: some samples treated as negatives may actually be semantically similar.

Main focus:

- false negatives
- contrastive learning failure modes
- representation quality
- similarity analysis

---

### 5. Spectral Geometry Embedding Analysis

Repository: [spectral-geometry-embedding-analysis](https://github.com/subhaaniii/spectral-geometry-embedding-analysis)

This project studies embedding-space geometry to understand whether learned representations are well-structured or distorted.

Main focus:

- embedding diagnostics
- spectral analysis
- representation geometry
- model failure analysis

---

### 6. Sumora

Repository: [sumora](https://github.com/subhaaniii/sumora)

This is an applied AI/software project: a movie discovery system with search, filtering, external APIs, and chatbot-style interaction.

Main focus:

- applied AI
- full-stack development
- search interface
- product-oriented engineering

---

## Contact

GitHub: [subhaaniii](https://github.com/subhaaniii)

I am currently preparing for fully funded PhD applications in Computer Science, with a focus on multimodal learning, retrieval systems, medical AI, and trustworthy model evaluation.
