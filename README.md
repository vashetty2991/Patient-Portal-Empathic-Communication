# Empathic Communication Classification

This repository contains the analysis code accompanying the manuscript:

> **Evaluating Large Language Models for Measuring Empathic Communication in Patient Portal Messages**

The repository includes notebooks used to train and evaluate supervised transformer models and large language models (LLMs), as well as notebooks used to reproduce the figures presented in the manuscript.

---

## Repository structure

```text
.
├── analysis_notebooks/
│   ├── Empathic_Opportunity_ClinicalBERT_eval.ipynb
│   ├── Empathic_Opportunity_DeBERTa_eval.ipynb
│   ├── Empathic_Opportunity_LLM_eval.ipynb
│   ├── Empathic_Response_ClinicalBERT_eval.ipynb
│   ├── Empathic_Response_DeBERTa_eval.ipynb
│   └── Empathic_Response_LLM_eval.ipynb
│
├── figure_generation/
│   ├── Figure2_code.ipynb
│   ├── Figure3_code.ipynb
│   ├── Figure4_code.ipynb
│   └── Supplementary_Figure1_code.ipynb
│
├── figures/
│
├── README.md
├── LICENSE
├── .gitignore
└── CITATION.cff
```

---

# Analysis notebooks

These notebooks perform the model training and evaluation described in the manuscript.

### Empathic opportunity classification

| Notebook | Description |
|-----------|-------------|
| **Empathic_Opportunity_ClinicalBERT_eval.ipynb** | Fine-tunes and evaluates ClinicalBERT for empathic opportunity classification. |
| **Empathic_Opportunity_DeBERTa_eval.ipynb** | Fine-tunes and evaluates DeBERTaV3-base for empathic opportunity classification. |
| **Empathic_Opportunity_LLM_eval.ipynb** | Queries Llama-3.1 models hosted on Databricks and evaluates LLM performance for empathic opportunity classification. |

### Empathy classification

| Notebook | Description |
|-----------|-------------|
| **Empathic_Response_ClinicalBERT_eval.ipynb** | Fine-tunes and evaluates ClinicalBERT for binary empathy classification. |
| **Empathic_Response_DeBERTa_eval.ipynb** | Fine-tunes and evaluates DeBERTaV3-base for binary empathy classification. |
| **Empathic_Response_LLM_eval.ipynb** | Queries Llama-3.1 models hosted on Databricks and evaluates LLM performance for binary empathy classification. |

---

# Figure generation notebooks

These notebooks reproduce the publication-quality figures included in the manuscript.

| Notebook | Figure |
|-----------|--------|
| **Figure2_code.ipynb** | Figure 2 – LLM performance for empathic opportunity classification |
| **Figure3_code.ipynb** | Figure 3 – Supervised model performance across training set sizes for empathic opportunity classification |
| **Figure4_code.ipynb** | Figure 4 – LLM performance for binary empathy classification |
| **Supplementary_Figure1_code.ipynb** | Supplementary Figure 1 – Supervised model performance across training set sizes for binary empathy classification |

---

# Data availability

The patient portal message data analyzed in this study are not included in this repository. The underlying data contain protected health information (PHI) and are subject to institutional and ethical restrictions on sharing.

To protect participant privacy, this repository does **not** include:

- Patient-level data
- Patient portal message text
- Few-shot prompts containing PHI
- Local institutional file paths
- Credentials or API keys

The figure-generation notebooks rely only on aggregate performance metrics reported in the manuscript.

---

# Requirements

The analysis notebooks require:

- Access to the original study dataset
- Access to Databricks-hosted Llama endpoints (for LLM evaluation notebooks)

These resources are not publicly available.

---

# Accessibility

The figure-generation notebooks produce publication-quality figures designed to improve accessibility by using:

- Readable sans-serif fonts
- Colorblind-accessible color palettes
- Marker shapes and line styles in addition to color
- High-resolution PNG and vector (PDF/SVG) outputs

---

# Citation

If you use or adapt this repository, please cite the associated manuscript.

Citation metadata are provided in **CITATION.cff**.

---

# License

This repository is distributed under the MIT License. See the **LICENSE** file for details.
