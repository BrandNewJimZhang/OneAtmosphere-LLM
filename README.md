# OneAtmos-Bench

## 🌍 Introduction

**OneAtmos-Bench** is a benchmark dataset crafted for evaluating large language models (LLMs) within the atmospheric domain. Developed under the **One Atmosphere** framework, it integrates air quality, climate, and pollution control as interconnected elements of a unified atmospheric system.

This benchmark covers six critical subdomains: Atmospheric Mercury, Atmospheric Physics, Atmospheric Chemistry, Climate, Air Quality Model, and Pollution Control. Emphasizing open-ended questions, it provides a comprehensive assessment benchmark for LLMs in the atmospheric domain.

---

## 🏗️ Dataset Overview

- **Total QA pairs**: 994
- **Question types**:
  - True/False: 166
  - Calculation: 33
  - Open-ended: 795
- **Difficulty levels**: simple / medium / hard

### 🌐 Covered Subdomains

The dataset covers six major atmospheric science subdomains:
- **Atmospheric Mercury**
- **Atmospheric Physics**
- **Atmospheric Chemistry**
- **Climate**
- **Air Quality Model**
- **Pollution Control**

---

## 📁 Data File

The main dataset is provided in the following CSV file:

- [`OneAtmos-Bench.csv`](./data/OneAtmos-Bench.csv)

---

## 🧾 Field Descriptions

| Field Name | Description |
|------------|-------------|
| `ID` | Unique identifier for each QA pair. |
| `question` | The question derived from atmospheric domain sources. |
| `answer` | Ground-truth answer, validated by domain experts. |
| `domain` | One of six atmospheric subdomains: Atmospheric Mercury, Atmospheric Physics, Atmospheric Chemistry, Climate, Air Quality Model, Pollution Control. |
| `difficulty` | Estimated difficulty level (simple / medium / hard). |
| `divergence` | This question requires divergent thinking (0 or 1). |
| `qwq-32b` | Response from QWQ-32B model. |
| `qwen2.5-72b-instruct` | Response from Qwen2.5-72B-Instruct model. |
| `qwen2.5-32b-instruct` | Response from Qwen2.5-32B-Instruct model. |
| `qwen2.5-14b-instruct` | Response from Qwen2.5-14B-Instruct model. |
| `qwen2.5-7b-instruct` | Response from Qwen2.5-7B-Instruct model. |
| `deepseek-v3` | Response from DeepSeek-V3 model. |
| `deepseek-r1-distill-qwen-32b` | Response from DeepSeek-R1 model distilled from Qwen-32B. |
| `qwen-max-latest` | Response from the latest Qwen-Max model. |
| `glm-4-plus` | Response from GLM-4-Plus model. |
| `gpt-3.5-turbo` | Response from GPT-3.5-Turbo model. |
| `gpt-4o` | Response from GPT-4o model. |


---

## 📌 Citation

If you use this dataset, please cite:

```bibtex
@article{oneatmosbench2025,
  title={Evaluating the Performance of Large Language Models under the One Atmosphere Framework based on Automated Extracted Datasets},
  author={Shiqin Dai, Qingru Wu, Haowen Zhang, Yan Wang, Shuxiao Wang},
  journal={Under Review},
  year={2025}
}
```

---

## 🙏 Acknowledgements

We thank domain experts from atmospheric physics and chemistry, air pollution, and climate science communities for their contributions to the validation and refinement of this dataset.
