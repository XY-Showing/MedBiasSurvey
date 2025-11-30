# Bias in Large AI Models for Medicine and Healthcare: Survey and Challenges

[![Paper](https://img.shields.io/badge/Paper-PDF-red)](./MedLLM_Bias_Survey.pdf)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📖 Overview

This repository contains the resources, taxonomy, and data associated with our survey paper: **"Bias in Large AI Models for Medicine and Healthcare: Survey and Challenges"**.

Large AI models (including LLMs, LVMs, and LMMs) are transforming healthcare, yet they risk perpetuating or amplifying medical biases. This project provides a comprehensive synthesis of **55 representative studies**, organizing the literature into a clear taxonomy of bias, detection methods, and mitigation strategies.

### 🎯 Key Contributions
* **Taxonomy:** A dual taxonomy categorizing bias by **Medical Scenarios** (e.g., triage, education) and **Clinical Specialties** (e.g., cardiology, oncology).
* **Resources:** A structured index of **Large AI Models** and **Datasets** used in bias research.
* **Methodology:** A review of current techniques for **Bias Detection** (e.g., counterfactual testing) and **Mitigation** (pre-, in-, and post-processing).
* **Future Directions:** Identification of open problems such as the fairness-accuracy trade-off and global health inequities.

---

## 🧩 Taxonomy of Medical Bias

We categorize medical bias along two principal axes to facilitate precise identification and mitigation.

### 1. Bias Across Medical Scenarios
* **Clinical Decision Support:** Disparities in diagnostic reasoning or treatment planning.
* **Patient Communication:** Biased triage advice or health counseling via chatbots.
* **Medical Documentation:** Stereotypes or hallucinations in report generation and summarization.
* **Medical Education:** Misrepresentation in generated case vignettes or training materials.

### 2. Bias Across Clinical Specialties
Our survey covers biases identified in specific domains, including:
* 🫀 **Cardiology**
* 🫁 **Pulmonology**
* 🦀 **Oncology**
* 🦠 **Infectious Disease**
* 👁️ **Ophthalmology**
* 🧠 **Mental Health & Psychiatry**

---

## 🛠️ Resources

### 🤖 Large AI Models for Medical Bias Research
Below are selected models analyzed in the survey.

| Model Name | Family | Parameter Size | Open Source? |
| :--- | :--- | :--- | :--- |
| **Med-PaLM 2** | PaLM 2 | ≥ 175B | No |
| **Meditron** | LlaMa-2 | 70B-175B | Yes |
| **PMC-LlaMa** | LlaMa | 10B-70B | Yes |
| **BioGPT** | GPT | < 1B | Yes |
| **LLaVA-Med** | LLaVA | 1B-10B | Yes |
| **ClinicalBERT** | ClinicalBERT | < 1B | Yes |

### 📊 Datasets for Bias Detection
We have compiled datasets across three modalities: Text, Image, and Multimodal.

* **Text:** MedQA, PubMedQA, MIMIC-IV, AMQA, BiasMD.
* **Image:** CheXpert, MIMIC-CXR, HAM10000, ODIR, Fitzpatrick17k.
* **Multimodal:** LLaVA-Med, ROCO, PMC-OA.

---

## ⚙️ Methodology

### Bias Detection Techniques
* **Input Generation:** Creating synthetic patients or mutating existing clinical vignettes (e.g., changing "Male" to "Female").
* **Evaluation Metrics:**
    * *Answer Consistency:* Measuring robustness across demographic changes.
    * *Fairness Metrics:* Demographic Parity, Equalized Odds.
    * *Human Expert Assessment:* Physician review for complex scenarios.

### Bias Mitigation Strategies
1.  **Pre-processing:** Data augmentation and rebalancing before training.
2.  **In-processing:** Model fine-tuning (e.g., FairCLIP), loss function modification.
3.  **Post-processing:** Prompt engineering (Chain-of-Thought), output rewriting, and ensembling.

---

## 🚀 Open Problems & Opportunities

Based on our analysis, we highlight the following urgent research directions:
1.  **Unified Foundations:** Defining "medical fairness" distinct from general AI fairness.
2.  **Standardized Benchmarks:** Moving beyond ad-hoc testing to rigorous, scalable benchmarks.
3.  **Real-World Validation:** Continuous monitoring of models in deployed clinical settings.
4.  **Global Health Equity:** Addressing the lack of representation for non-Western populations and languages.
5.  **Fairness-Accuracy Trade-off:** Investigating how debiasing affects diagnostic performance.

---

## 📝 Citation

If you find this survey or repository helpful, please cite our work:

```bibtex
@article{xiao2025bias,
  title={Bias in Large AI Models for Medicine and Healthcare: Survey and Challenges},
  author={Xiao, Ying and Chen, Zhenpeng and Huang, Jen-tse and Chen, Wenting and Liu, Yepang and Li, Kezhi and Mousavi, Mohammad Reza and Dobson, Richard and Zhang, Jie M.},
  journal={arXiv preprint},
  year={2025}
}
