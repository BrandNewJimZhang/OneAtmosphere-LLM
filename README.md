# OneAtmos-Bench

[![Paper](https://img.shields.io/badge/Environ.%20Sci.%20Technol.-10.1021%2Facs.est.5c10297-blue)](https://doi.org/10.1021/acs.est.5c10297)
[![Dataset](https://img.shields.io/badge/dataset-994%20QA%20pairs-green)](./OneAtmos-Bench.csv)

## 🌍 Introduction

**OneAtmos-Bench** is a benchmark dataset for evaluating large language models (LLMs) in the atmospheric science domain. It is the core dataset of our paper published in *Environmental Science & Technology*:

> Dai, S.; Wu, Q.; Zhang, H.; Wang, Y.; Wang, S. Evaluating the Performance of Large Language Models for One Atmosphere Using Automated Extracted Datasets. *Environ. Sci. Technol.* **2026**, *60* (1), 725–735. https://doi.org/10.1021/acs.est.5c10297

Developed under the **One Atmosphere** framework, the benchmark treats air quality, climate, and pollution control as interconnected elements of a unified atmospheric system. It covers six critical subdomains and — unlike most existing multiple-choice benchmarks — emphasizes **open-ended questions**, providing a comprehensive assessment of LLM capability in atmospheric science.

The dataset ships with the responses of 11 LLMs evaluated in the paper, so results can be reproduced and re-scored without re-running the models.

## 🏗️ Dataset Overview

- **Total QA pairs**: 994
- **Question types**:
  - Open-ended: 795
  - True/False: 166
  - Calculation: 33
- **Difficulty levels**: simple / medium / hard
- **Divergent-thinking flag**: each question is annotated with whether it requires divergent thinking

### 🌐 Covered Subdomains

- **Atmospheric Mercury**
- **Atmospheric Physics**
- **Atmospheric Chemistry**
- **Climate**
- **Air Quality Model**
- **Pollution Control**

## 📁 Data File

The full dataset — questions, expert-validated answers, annotations, and the responses of all 11 evaluated LLMs — is provided as a single CSV file:

- [`OneAtmos-Bench.csv`](./OneAtmos-Bench.csv)

## 🧾 Field Descriptions

| Field Name | Description |
|------------|-------------|
| `ID` | Unique identifier for each QA pair. |
| `question` | The question, automatically extracted from atmospheric-domain sources and refined by domain experts. |
| `answer` | Ground-truth answer, validated by domain experts. |
| `domain` | One of six atmospheric subdomains: Atmospheric Mercury, Atmospheric Physics, Atmospheric Chemistry, Climate, Air Quality Model, Pollution Control. |
| `difficulty` | Estimated difficulty level (simple / medium / hard). |
| `divergence` | Whether the question requires divergent thinking (0 or 1). |
| `qwq-32b` | Response from QwQ-32B. |
| `qwen2.5-72b-instruct` | Response from Qwen2.5-72B-Instruct. |
| `qwen2.5-32b-instruct` | Response from Qwen2.5-32B-Instruct. |
| `qwen2.5-14b-instruct` | Response from Qwen2.5-14B-Instruct. |
| `qwen2.5-7b-instruct` | Response from Qwen2.5-7B-Instruct. |
| `deepseek-v3` | Response from DeepSeek-V3. |
| `deepseek-r1-distill-qwen-32b` | Response from DeepSeek-R1-Distill-Qwen-32B. |
| `qwen-max-latest` | Response from Qwen-Max (latest). |
| `glm-4-plus` | Response from GLM-4-Plus. |
| `gpt-3.5-turbo` | Response from GPT-3.5-Turbo. |
| `gpt-4o` | Response from GPT-4o. |

## 📌 Citation

If you use this dataset, please cite:

```bibtex
@article{dai2026oneatmosbench,
  title   = {Evaluating the Performance of Large Language Models for One Atmosphere Using Automated Extracted Datasets},
  author  = {Dai, Shiqin and Wu, Qingru and Zhang, Haowen and Wang, Yan and Wang, Shuxiao},
  journal = {Environmental Science \& Technology},
  year    = {2026},
  volume  = {60},
  number  = {1},
  pages   = {725--735},
  doi     = {10.1021/acs.est.5c10297}
}
```

## 🙏 Acknowledgements

We thank domain experts from the atmospheric physics and chemistry, air pollution, and climate science communities for their contributions to the validation and refinement of this dataset.
