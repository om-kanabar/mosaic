# AGENTS.md

You are working on a research project called:

***Mosaic: A Novel Data Augmentation Method for Reducing Overfitting in Time-Series Models***

This project is a STEM Fair project with the goal of qualifying for ISEF.

## Project Info

- Language: Python
- Dataset: Tokamark Dataset
  - Repository: https://github.com/UKAEA-IBM-STFC-Fusion-FMs/tokamark_baseline
  - Paper: https://arxiv.org/html/2602.10132v3

## Research Goal

This project investigates whether Mosaic, a novel data augmentation method, can reduce overfitting in time-series machine learning models.

Mosaic creates synthetic training examples by recombining meaningful segments of existing time-series data. The goal is to expose models to additional realistic variations and underrepresented temporal patterns, improving generalization.

## Experimental Design

- Experimental Group
    - Mosaic
- Control Group
    - Regular
    - Dropout
    - Weight Decay
    - Random Recombination

## Research Constraints

- Experiments need to be reproducible
- Use controlled pseudorandomness for all stochastic processes.
    - Record all seeds used for reproducibility.
- Do not modify validation or test data
- Keep baseline comparisons fair
- Ensure augmentation methods do not introduce data leakage or unrealistic time-series behavior.
- For Mosaic ensure the code does not create synthetic data that violates known temporal or physical relationships.
- **Prioritize scientific correctness over optimizing results.**

## Rules

Follow the ISEF 2026 Generative AI Use Guidelines:
https://sspcdn.blob.core.windows.net/files/Documents/SEP/ISEF/2026/Rules/Generative-AI-Use-Table.pdf

Before assisting with research-related tasks, ensure the requested action follows these guidelines.

### Research Integrity
- Do not fabricate, modify, or assume experimental results.
- Do not make scientific claims without supporting evidence.
- Preserve reproducibility by recording random seeds and experiment configurations.
- Keep validation and test data separate from training data.
- Do not optimize only for performance; prioritize understanding and correctness.

### Code Changes
- Prefer simple, readable, and well-documented code.
- Explain significant algorithmic changes before implementing them.
- Avoid unnecessary dependencies and complex abstractions.
- Do not change multiple experimental variables at once unless explicitly requested.
- Preserve previous experiment results and configurations.

### AI Usage
- Assist with coding, debugging, explanations, and brainstorming.
- Do not write the final research paper, abstract, poster, or conclusions.
- Do not replace the researcher's understanding or decision-making.