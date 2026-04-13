# Blooms Taxonomy Classifier for ITEE

This repository contains the prompts, model configurations, and supporting materials for the automated classification of cognitive process levels in Japan's Information Technology Engineers Examinations (ITEE) based on the revised Bloom's Taxonomy.

## Overview

This project explores various automated approaches to classify exam questions into four cognitive levels: Remember, Understand, Apply, and Analyze. We compare traditional machine learning (BERT), single-agent LLM prompting (Gemini), and a novel **Multi-Agent Deliberation Framework** implemented with Claude.

This repository is maintained to ensure the reproducibility of the results presented in our research.

## Publication

If you find this work useful, please cite our conference paper:

**Toshiyo Seto, Brendan Flanagan, Yiling Dai, Masako Okamoto, and Hiroaki Ogata. "Automated Classification of Bloom's Taxonomy Levels for Japan's Information Technology Engineers Examinations." In Proceedings of the 2nd International Conference on Learning Evidence and Analytics (ICLEA) at TBICS 2026, Kumamoto, Japan, June 2026.**

## Contents

- `/prompts`: Full text of the system and user prompts for both single-agent and multi-agent configurations.
  - `gemini_prompts.md`: Zero-shot and few-shot prompts for Gemini.
  - `claude_prompts.md`: Single-agent and Multi-agent prompts for Claude.

## Key Findings

1. **Cognitive Consistency:** Manual analysis revealed that cognitive complexity remains consistent across all ITEE proficiency levels, suggesting that exam difficulty is driven by domain knowledge depth.
2. **Binary vs. Four-class:** While four-class classification is challenging (max accuracy 0.710), binary classification (LOTS vs. HOTS) achieves high accuracy (up to 0.879).
3. **Multi-Agent Advantage:** Structured deliberation among specialized AI agents outperforms single-agent LLM prompting for nuanced cognitive assessment.

## Repository Versioning

The version of the prompts used for the TBICS 2026 camera-ready submission is tagged as `v1.0-TBICS2026`. Future updates for journal submissions will be managed through new release tags.

## Acknowledgements

This work was supported by JSPS Grant-in-Aid for Scientific Research (B) JP20H01722 and JP23H01001, (Exploratory) JP21K19824, (A) JP23H00505, and NEDO JPNP20006. It was also supported by the MEXT Project for Training Experts in Statistical Sciences.
