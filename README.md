# POBS: Preference, Opinion, and Belief Survey

This repository contains the POBS dataset and model responses to the dataset:  
**"Think Again! The Effect of Test-Time Compute on Preferences, Opinions, and Beliefs of Large Language Models"**  
(Published in ACL 2025 - Industry Track*).

## 📦 Contents

- **POBS Dataset**  
  A benchmark of 20 topics containing over 500 Likert-style questions designed to assess subjective preferences, opinions, and beliefs expressed by LLMs across:
  - Societal and cultural issues (e.g., LGBTQ+ rights, Free Speech, Immigration)
  - Ethical dilemmas (e.g., AI risk, adoption, surrogacy)
  - Personal preferences (e.g., profession, geography, sports)

- **Model Responses**  
  Collected responses from **10 prominent LLMs**, both open- and closed-source, evaluated using three prompting methods:
  - **Direct prompting**
  - **Chain-of-Thought reasoning**
  - **Self-reflection and reconsideration**

- **Declarative POBS**  
  A simplified version of the benchmark containing a single, direct question per polar topic to assess models’ self-declared stances.
  It serves to compare the model's declarative stance with its actual stance inferred from POBs.

## 📁 File Structure

```
pobs/
├── POBS_v11.json                    # Original POBS prompts (Likert-style questions)
├── POBS_v11_declarative.json       # Direct view1/view2 preference questions (Declarative POBS)
├── POBS_v11_model_responses/       # Model responses to POBS_v11 across prompting styles
│   ├── POBS_V11_direct/            # Responses to direct prompts
│   ├── POBS_V11_reasoning_reflection/  # Responses to reasoning + reflection prompts
├── POBS_v11_declarative_responses/ # Model responses to Declarative POBS
│   ├── POBS_V11_direct/            # Declarative direct responses
│   ├── POBS_V11_reasoning_reconsider/ # Declarative reasoning + reconsideration responses
├── README.md                       # This file

```

## 🔬 Purpose

The dataset is designed to support the evaluation of LLMs in terms of:

- **Bias and subjectivity** across controversial and personal topics
- **Reliability**: Consistency across repeated prompts
- **Neutrality**: Tendency to avoid extreme stances
- **Consistency**: Topical agreement across related questions
- **Impact of test-time compute**: Assessing whether reasoning and self-reflection reduce bias

## 📑 Paper Contributions

As described in the accompanying paper, this dataset enabled us to:

1. Introduce a **reference-free benchmark** for probing subjective tendencies in LLMs  
2. Propose and evaluate **metrics** like the *Non-Neutrality Index (NNI)* and *Topical Consistency Index (TCI)*  
3. Analyze **opinion shifts** and *ideological trends* across prompting strategies and model versions  
4. Highlight that **reasoning and reflection**, while helpful in other domains, offer only **limited gains** in improving neutrality and consistency on subjective topics

## Citation:
@article{kour2025think,
  title={Think Again! The Effect of Test-Time Compute on Preferences, Opinions, and Beliefs of Large Language Models},
  author={Kour, George and Nakash, Itay and Anaby-Tavor, Ateret and Shmueli-Scheuer, Michal},
  journal={arXiv preprint arXiv:2505.19621},
  year={2025}
}
