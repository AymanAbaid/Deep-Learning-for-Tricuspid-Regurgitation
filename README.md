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
**Echocardiography datasets potentially useful for tricuspid regurgitation (TR) research.** TR utility may be direct (TR severity) or indirect (right-ventricular phenotyping, view classification, segmentation, and representation learning). Dataset sizes use the units specified in the notes; **publicly described does not always mean unrestricted download**.

| Dataset / source | Year | Echo type | Views / acquisition | Size | Availability |
|---|---|---|---|---|---|
| **[EchoNet-TR — paper](https://doi.org/10.1001/jamacardio.2025.0498)** | 2025 | TTE | A4C, tricuspid colour Doppler | 2,079,898 (reported scale; confirm unit in paper) | **Not publicly released**; paper only |
| **[MIMIC-IV-Echo](https://physionet.org/content/mimic-iv-echo/1.0.1/)** | 2023; updated 2026 | TTE and other echo records | Multi-view DICOM; linked clinical measurements | 524,137 DICOMs (7,228 studies) in v1.0.1 | **Credentialed PhysioNet access** |
| **[ECHOVIEW](https://physionet.org/content/echoview/0.1/)** | 2026 | TTE | 23 machine-predicted view categories; includes PLAX, PSAX, A2C–A5C, RV inflow, subcostal | 29,196 video-level classifications | **Credentialed**; view annotations, source videos in MIMIC-IV-Echo |
| **[MIMIC-IV-ECHO-Ext-LVVOLUMES-A4C-ROI](https://physionet.org/content/mimic-iv-echo-ext-lvvol-a4c/1.0.0/)** | 2026 | TTE | A4C; ROI masks and LV volume labels | 1,064 videos | **Credentialed PhysioNet access** |
| **[RVENet](https://rvenet.github.io/dataset/)** | 2023 | TTE | A4C, 2D video with 3D-derived RVEF targets | 3,583 videos | **Public dataset portal** |
| **[EchoNet-Dynamic](https://echonet.github.io/dynamic/)** | 2020 | TTE | A4C | 10,030 videos | **Available subject to research-use terms** |
| **[EchoNet-LVH](https://echonet.github.io/lvh/)** | 2022 | TTE | PLAX | 12,000 videos | **Dataset portal; review terms** |
| **[EchoNet-Pediatric](https://echonet.github.io/pediatric/)** | 2023 | TTE | A4C and PSAX | 7,643 videos | **Dataset portal; review terms** |
| **[CAMUS](https://www.creatis.insa-lyon.fr/Challenge/camus/databases.html)** | 2019 | TTE | A2C and A4C | 500 patients | **Public download** |
| **[HMC-QU](https://www.kaggle.com/datasets/aysendegerli/hmcqu-dataset)** | 2021 | TTE | A2C and A4C; low-quality MI imaging | 322 (user-supplied count; definitions vary by paper) | **Public Kaggle resource** |
| **[CardiacNet-PAH](https://github.com/xmed-lab/CardiacNet)** | 2024 | TTE | A4C | 496 cases | **Download guidance in repository** |
| **[SegRWMA](https://github.com/XiaoweiXu/Segment-level-Assessment-of-Regional-Wall-Motion-Abnormality-from-Echocardiography-Images)** | 2023 | TTE | A2C, A3C, A4C | 1,782 (user-supplied image count; 198 patients reported) | **Dataset / instructions via GitHub** |
| **[TMED-2](https://tmed.cs.tufts.edu/tmed_v2.html)** | 2022 | TTE | PLAX, PSAX, A2C, A4C, other | 599 labelled studies | **Public dataset portal** |
| **[EchoSlicer 3D dataset](https://github.com/echonet/3d-echo/releases/download/v1.0/dataset.zip)** | 2025 | 3D TTE | 3D volumes; extract A2C, A3C, A4C, A5C, PLAX and PSAX | 29 3D videos | **Public [code and description](https://github.com/echonet/3d-echo)** |
| **[MITEA](https://www.cardiacatlas.org/mitea/)** | 2023 | 3D TTE | 3D LV volumes with MRI-informed labels | 268 (user-supplied count; confirm split) | **Dataset portal; review access terms** |
| **[Add echo dataset](https://example.org)** | YYYY | TTE / TEE / 3D | [Views] | [Number + unit] | [Open / request / credentialed / unavailable] |


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
