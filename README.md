# Cardiovascular AI — Resource Library

A curated, team-maintained index of cardiovascular AI **datasets**, **foundation models**, and **papers**. This file stores links and short notes, not copies of datasets or copyrighted papers.

**Maintainers:** [Team / institution] · **Last reviewed:** YYYY-MM-DD · **Contribute:** Submit a pull request with a brief rationale and a verified original link.

## Navigation

- [Datasets](#1-datasets)
- [Foundation models](#2-foundation-models)
- [Papers](#3-papers)
- [How to add a resource](#4-how-to-add-a-resource)
- [Interesting Papers](#5-interesting-papers)


## 1. Datasets


## 2. Foundation models


### Echocardiography foundation models

| Model | Primary echo type | Paper | Pretrained weights |
|---|---|---|---|
| **EchoCLIP / EchoCLIP-R** — multimodal vision–language interpretation | TTE (A4C, tissue Doppler, color Doppler) | [Paper](https://www.nature.com/articles/s41591-024-02959-y) | [Weights / instructions](https://github.com/echonet/echo_CLIP#quickstart) |
| **EchoFM** — generalizable echocardiogram analysis | TTE | [Paper](https://doi.org/10.1109/TMI.2025.3580713) | [Checkpoint](https://huggingface.co/sekeun/EchoFM) |
| **EchoApex** — general-purpose vision foundation model | TTE, TEE, ICE | [Paper](https://arxiv.org/abs/2410.11092) | Not Available |
| **Echo-Vision-FM** — echocardiography video pretraining and fine-tuning | TTE | [Paper](https://doi.org/10.1038/s41467-025-66340-4) | [Checkpoint release](https://github.com/ZiyangZhang0511/Echo-Vison-FM/releases/tag/v1) |
| **PanEcho** — multitask echocardiography interpretation | TTE, multiple views | [Paper](https://jamanetwork.com/journals/jama/fullarticle/2835630) | [Model and loading instructions](https://github.com/CarDS-Yale/PanEcho) |
| **EchoPrime** — multi-video vision–language interpretation | Adult TTE | [Paper](https://doi.org/10.1038/s41586-025-09850-x) | [Official weights and setup](https://github.com/echonet/EchoPrime) |
| **EchoFlow** — cardiac ultrasound image/video generation | Cardiac ultrasound / TTE | [Paper](https://arxiv.org/abs/2503.22357) | [Model files](https://huggingface.co/HReynaud/EchoFlow/tree/main) |
| **EchoJEPA** — latent predictive echocardiography foundation model | Clinical echocardiography video, primarily TTE | [Paper](https://arxiv.org/abs/2602.02603) | [Checkpoint instructions](https://github.com/bowang-lab/EchoJEPA#echojepa-checkpoints) |
| **EchoVLM (MoE)** — dynamic mixture-of-experts vision–language model for general ultrasound | Multi-organ ultrasound (not TTE-specific) | [Paper](https://aclanthology.org/2026.acl-long.494/) | [Model weights](https://huggingface.co/chaoyinshe/EchoVLM) |
| **EchoVLM (measurement-grounded)** — multimodal learning for echocardiography | Echocardiographic images / views | [Paper](https://arxiv.org/abs/2512.12107) | Not Available |
| **Add echo model** | [TTE / TEE / ICE] | [Paper URL] | [Weights URL or availability] |



**Weight status convention:** **Yes** = official model files or loading instructions listed; **Not verified** = no official checkpoint confirmed; **Listed, download reliability uncertain** = checkpoint described but access may be unreliable. Listing does not establish clinical readiness or unrestricted reuse.


### ECG and physiological signals

| Model | Task / modalities | Code | Weights | Paper | Notes |
|---|---|---|---|---|---|
| ECG-FM | Pretrained ECG representation learning | [GitHub](https://github.com/bowang-lab/ecg-fm) | [See repository](https://github.com/bowang-lab/ecg-fm#-model) | [See repository](https://github.com/bowang-lab/ecg-fm) | Check model licence, preprocessing and external validation before reuse |
| **[Add model]** | [Signals / ECG / wearable] | [Code](https://example.org) | [Weights](https://example.org) | [Paper](https://example.org) | [Strengths, limitations] |

### Cardiovascular imaging

| Model | Task / modalities | Code | Weights | Paper | Notes |
|---|---|---|---|---|---|
| **[Add model]** | [Echo / CMR / CT] | [Code](https://example.org) | [Weights](https://example.org) | [Paper](https://example.org) | [Pretraining, transfer tasks] |

### Multimodal and clinical language models

| Model | Task / modalities | Code | Weights | Paper | Notes |
|---|---|---|---|---|---|
| **[Add model]** | [Images + ECG + EHR / text] | [Code](https://example.org) | [Weights](https://example.org) | [Paper](https://example.org) | [Scope and validation] |

## 3. Papers

### Reviews and perspectives

| Paper | Year | Why it matters | Link | Related code/data |
|---|---|---|---|---|
| Foundation models for electrocardiogram interpretation: clinical implications | 2026 | Comparison and clinical implications of ECG foundation-model approaches | [PubMed](https://pubmed.ncbi.nlm.nih.gov/41568699/) | [Add associated resources] |
| **[Add review]** | YYYY | [One-sentence takeaway] | [DOI / PubMed](https://example.org) | [Optional] |

### ECG AI

| Paper | Year | Why it matters | Link | Related code/data |
|---|---|---|---|---|
| **[Add paper]** | YYYY | [Method, cohort, key result or limitation] | [DOI / PubMed](https://example.org) | [Code / dataset](https://example.org) |

### Echocardiography and imaging AI

| Paper | Year | Why it matters | Link | Related code/data |
|---|---|---|---|---|
| Video-based AI for beat-to-beat assessment of cardiac function | 2020 | Example of video-based assessment of cardiac function | [DOI](https://doi.org/10.1038/s41586-020-2145-8) | [EchoNet-Dynamic code](https://github.com/echonet/dynamic) |
| **[Add paper]** | YYYY | [Key insight] | [DOI / PubMed](https://example.org) | [Optional] |

### Multimodal, EHR and clinical prediction

| Paper | Year | Why it matters | Link | Related code/data |
|---|---|---|---|---|
| **[Add paper]** | YYYY | [Key insight] | [DOI / PubMed](https://example.org) | [Optional] |

### Validation, fairness and deployment

| Paper | Year | Why it matters | Link | Related code/data |
|---|---|---|---|---|
| **[Add paper]** | YYYY | [External validation / robustness / reporting] | [DOI / PubMed](https://example.org) | [Optional] |

## 4. How to add a resource

1. Add the item under the best-fit heading (create a new heading if needed).
2. Prefer **official** dataset pages, original paper DOI/PubMed links, and authors' code repositories.
3. Include a **one-sentence description** plus access/licensing constraints where relevant.
4. Check that the URL works and avoid duplicates. Record the last review date when maintaining an entry.
5. Never commit patient-level data, access tokens, credentials or restricted files to this repository.

## 5. Interesting Papers

Wang, D., Zhou, T., Gao, S., & Yang, J. (2025). Echo Flow-Induced Temporal Correlation Learning for Ultrasound Video Object Segmentation. IEEE Transactions on Biomedical Engineering.
