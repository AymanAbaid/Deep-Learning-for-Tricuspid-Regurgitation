# Cardiovascular AI — Resource Library

A curated, team-maintained index of cardiovascular AI **datasets**, **foundation models**, and **papers**. This file stores links and short notes, not copies of datasets or copyrighted papers.

**Maintainers:** [Team / institution] · **Last reviewed:** YYYY-MM-DD · **Contribute:** Submit a pull request with a brief rationale and a verified original link.

## Navigation

- [Datasets](#1-datasets)
- [Foundation models](#2-foundation-models)
- [Papers](#3-papers)
- [How to add a resource](#4-how-to-add-a-resource)

## 1. Datasets

### ECG and electrophysiology

| Dataset | What it contains / potential use | Access & restrictions | Link |
|---|---|---|---|
| PTB-XL | Labelled 12-lead ECG recordings; classification and benchmarking | Review terms and citation requirements | [PhysioNet](https://physionet.org/content/ptb-xl/1.0.3/) |
| **[Add dataset]** | [Modality, cohort, labels, approximate size] | [Open / registration / credentialed; licence] | [Official dataset](https://example.org) |

### Echocardiography

| Dataset | What it contains / potential use | Access & restrictions | Link |
|---|---|---|---|
| EchoNet-Dynamic | Echocardiography videos with cardiac-function labels | Registration; non-commercial research-use agreement | [Official site](https://echonet.github.io/dynamic/) |
| **[Add dataset]** | [Views, videos, segmentation or outcome labels] | [Terms] | [Official dataset](https://example.org) |

### Cardiac MRI / CT

| Dataset | What it contains / potential use | Access & restrictions | Link |
|---|---|---|---|
| **[Add CMR/CT dataset]** | [Imaging modality, tasks, labels] | [Terms] | [Official dataset](https://example.org) |

### EHR, wearables and multimodal data

| Dataset | What it contains / potential use | Access & restrictions | Link |
|---|---|---|---|
| **[Add dataset]** | [Clinical records / signals / modalities] | [Terms, ethical approval if applicable] | [Official dataset](https://example.org) |

## 2. Foundation models


### Echocardiography foundation models

| Model (code / repository) | Primary echo type | Paper | Pretrained weights |
|---|---|---|---|
| **[EchoCLIP / EchoCLIP-R](https://github.com/echonet/echo_CLIP)** — multimodal vision–language interpretation | TTE (A4C, tissue Doppler, color Doppler) | [Paper](https://arxiv.org/abs/2308.15670) | [Weights / instructions](https://github.com/echonet/echo_CLIP#quickstart) |
| **[EchoFM](https://github.com/SekeunKim/EchoFM)** — generalizable echocardiogram analysis | TTE | [Paper](https://doi.org/10.1109/TMI.2025.3580713) | [Weights / instructions](https://huggingface.co/sekeun/EchoFM) |
| **[EchoApex](https://arxiv.org/abs/2410.11092)** — general-purpose vision foundation model | TTE, TEE, ICE | [Paper](https://arxiv.org/abs/2410.11092) | Not verified |
| **[Echo-Vision-FM](https://github.com/ZiyangZhang0511/Echo-Vison-FM)** — echocardiography video pretraining and fine-tuning | TTE | [Paper](https://doi.org/10.1038/s41467-025-66340-4) | [Weights / instructions](https://github.com/ZiyangZhang0511/Echo-Vison-FM/releases/tag/v1) |
| **[PanEcho](https://github.com/CarDS-Yale/PanEcho)** — multitask echocardiography interpretation | TTE, multiple views | [Paper](https://pmc.ncbi.nlm.nih.gov/articles/PMC12186137/) | [Weights / instructions](https://github.com/CarDS-Yale/PanEcho#model-usage) |
| **[EchoPrime](https://github.com/echonet/EchoPrime)** — multi-video vision–language interpretation | Adult TTE | [Paper](https://github.com/echonet/EchoPrime) | [Weights / instructions](https://github.com/echonet/EchoPrime/releases/tag/v1.0.0) |
| **[EchoFlow](https://huggingface.co/HReynaud/EchoFlow)** — cardiac ultrasound image/video generation | TTE / cardiac ultrasound | [Paper](https://arxiv.org/abs/2503.22357) | [Weights / instructions](https://huggingface.co/HReynaud/EchoFlow/tree/main) |
| **[EchoJEPA](https://github.com/bowang-lab/EchoJEPA)** — latent predictive echocardiography foundation model | Primarily TTE / clinical echo video | [Paper](https://arxiv.org/abs/2602.02603) | [Weights / instructions](https://github.com/bowang-lab/EchoJEPA#echojepa-checkpoints) |
| **[Add echo model](https://example.org)** | [TTE / TEE / ICE] | [Paper](https://example.org) | [Weights](https://example.org) |

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

> **Reusable row templates** (copy a row into the appropriate section):
>
> Dataset: `| [Name] | [Contents / clinical task] | [Access / licence] | [Official link](https://example.org) |`
>
> Foundation model: `| [Name] | [Modalities / task] | [Code](https://example.org) | [Weights](https://example.org) | [Paper](https://example.org) | [Limits / caveats] |`
>
> Paper: `| [Title] | YYYY | [Why it matters] | [DOI](https://example.org) | [Optional code/data] |`

*Placeholder URLs at `example.org` are examples only and should be replaced before publishing.*
