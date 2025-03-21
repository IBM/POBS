# POBS: Preference, Opinion, and Belief Survey

This repository contains the **anonymized dataset** used in our paper:  
**"Think Again! The effect of test-time compute on Preferences, Opinions, and Beliefs of Large Language Models"** (under review to ACL Industry track).

## 📦 Contents

- **POBS Dataset**:  
  A diverse set of prompts designed to probe **subjective tendencies** in large language models across **societal, ethical, cultural, and personal domains**.


## 📊 Purpose

The dataset supports analysis of:
- Subjective preferences and biases in LLMs
- Impact of test-time compute (e.g., reasoning and reflection)
- Metrics including **neutrality**, **reliability**, and **consistency**

- **Model Responses**:  
  Responses from **10 leading LLMs**, both open- and closed-source, across the different prompting.


## 📁 File Structure

```
pobs/
├── POBS_v11.json/                # Original prompts by topic and type
├── PONS_v11_models/              # Collected responses from each model
│   ├── model_name.json    # One file per model
├── README.md               # This file
```
