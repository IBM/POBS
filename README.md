# POBS: Preference, Opinion, and Belief Survey

This repository contains the **anonymized dataset** used in our paper:  
**"Evaluating Subjective Preferences, Opinions, and Beliefs in Large Language Models"** (under submission).

## 📦 Dataset Contents

The repository includes:

- **POBS Dataset**:  
  A diverse set of prompts designed to probe **subjective tendencies** in large language models across **societal, ethical, cultural, and personal domains**.

- **Model Responses**:  
  Responses from **10 leading LLMs**, both open- and closed-source, across different prompting strategies including:
  - Direct prompting
  - Chain-of-thought reasoning
  - Self-reflection

Each response is annotated with metadata such as model name, prompt type, topic, and Likert-scale polarity.

## 📊 Purpose

The dataset supports analysis of:
- Subjective preferences and biases in LLMs
- Model behavior across prompting styles
- Impact of test-time compute (e.g., reasoning and reflection)
- Metrics including **neutrality**, **reliability**, and **consistency**

## 📁 File Structure

```
pobs/
├── POBS_v11.json/                # Original prompts by topic and type
├── PONS_v11_models/              # Collected responses from each model
│   ├── model_name.json    # One file per model
├── README.md               # This file
```
