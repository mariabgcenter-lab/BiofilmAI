BiofilmAI — Machine Learning Research Sandbox & Notebooks
BiofilmAI is an open‑source scientific machine learning research project dedicated to predicting, modeling, and analyzing biofilm formation.
This repository contains the core computational research, exploratory data analysis notebooks, and machine learning model training pipelines.

To see these models packaged into a live interactive web app with clinical workflow assistants, visit the companion repository: lab-ai-compliance-suite.

Computational Directory Structure
This repository is dedicated entirely to data pipelines, model sandbox development, and scientific exploration:

BiofilmAI/
notebooks/ — Core machine learning development sandbox

01_preprocessing.ipynb — Transcript cleanup, normalization, alignment

02_feature_engineering.ipynb — Biological interaction, ratio, significance metrics

03_model_training.ipynb — ML training (Logistic Regression, Random Forest)

04_feature_importance.ipynb — SHAP + model parameter interpretation

05_gene_level_predictions.ipynb — Single‑gene probability inference pipeline

data/ — Structured research datasets

gene_expression/ — GSE87213 transcriptomic tables

biofilm_diff_expr.csv

planktonic_diff_expr.csv

ml_feature_tables.csv

microscopy_images/ — Raw microscopy images (future expansion)

models/ — Saved trained model files (.pkl)

src/ — Helper utility scripts (future expansion)

README.md — Repository documentation

Scientific Research Roadmap
Phase 1 — Transcriptomic Machine Learning (Active)
Machine learning models predict biofilm formation thresholds using differential gene expression data.

Notebook functions:

01_preprocessing.ipynb — Clean raw differential expression profiles and align transcript data

02_feature_engineering.ipynb — Engineer biological interaction terms, significance flags, ratio metrics

03_model_training.ipynb — Train classifiers and map feature importance to pathways

04_feature_importance.ipynb — Analyze SHAP values and model parameters

05_gene_level_predictions.ipynb — Scaled pipeline inference for targeted single‑gene predictions

Phase 2 — BiofilmNN Deep Learning (Upcoming)
A convolutional deep learning pipeline for analyzing CLSM, SEM, and fluorescence microscopy images.

Planned notebooks:

Dual‑channel preprocessing

Biomass segmentation

Live/dead ratio extraction

Surface roughness quantification

Phase 3 — Multimodal Fusion (Planned)
A unified early‑ and late‑stage fusion framework combining transcriptomic features with microscopy‑derived morphological features.

Planned notebooks:

Feature vector concatenation

Cross‑modal normalization

Comparative multimodal classifier evaluation

🧪 Scientific Notebook Philosophy (“Vibe Coding”)
BiofilmAI uses a narrative‑driven scientific coding style:

Narrative‑Driven Steps — Markdown explains biological assumptions and pipeline logic

Domain‑Friendly Naming — Variables reflect biological meaning

Intermediate Visual Intuition — Frequent plots and previews validate transformations

Purpose‑Driven Code Blocks — Small, modular, readable functions

Scientific Closures — Each notebook ends with a “Summary of Discoveries”
