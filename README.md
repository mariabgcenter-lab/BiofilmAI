BiofilmAI — Multimodal Prediction of Biofilm Formation
BiofilmAI is a scientific machine learning research project focused on predicting biofilm formation using differential gene expression data from the GSE87213 dataset.
The project integrates microbiology expertise with modern AI workflows and follows a clear, narrative‑driven coding philosophy called Vibe Coding.

This repository contains the research sandbox: preprocessing, feature engineering, exploratory analysis, and model development.

🗂️ Project Structure
notebooks/ — Core machine learning development sandbox
01_preprocessing.ipynb — Loads raw data, cleans gene expression tables, merges differential expression results, and prepares machine‑learning features.

02_feature_engineering.ipynb — Constructs engineered features such as interaction terms, ratios, absolute log fold changes, significance flags, and condition‑specific metrics.

03_model_training.ipynb — Trains baseline machine‑learning models and evaluates predictive performance.

data/gene_expression/ — Gene expression datasets
Includes all transcriptomic files used in the project:

Biofilm differential expression results

Planktonic differential expression results

Biofilm vs planktonic comparison tables

Cleaned differential expression tables

Machine‑learning feature tables

🧬 Dataset Overview: GSE87213
Differential gene expression of Pseudomonas aeruginosa ΔPA14_22470 (ΔPA3225) versus wildtype in planktonic and biofilm conditions.

This dataset provides the biological foundation for BiofilmAI’s predictive modeling pipeline, enabling exploration of:

biofilm‑specific transcriptional changes

planktonic vs biofilm contrasts

mutant vs wildtype regulatory patterns

🎯 Project Goal
BiofilmAI aims to build machine‑learning models that predict biofilm formation using:

log fold changes

adjusted p‑values

condition‑specific gene expression patterns

engineered biological + statistical features

The project demonstrates how biological insight and AI engineering can be combined to understand complex microbial behaviors.

🎨 Vibe Coding — Scientific Notebook Philosophy
BiofilmAI uses Vibe Coding, a narrative‑driven scientific coding style that transforms each notebook into a guided scientific journal entry rather than a block of code.

Purpose
To develop clean, intuitive, and expressive coding habits while working through preprocessing, feature engineering, and model training.

Core Principles
Write code in clear narrative steps

Use microbiology‑friendly variable names

Visualize intermediate results for intuition

Maintain consistent formatting and structure

Keep functions small, readable, and purposeful

End each notebook with a summary block

Make the workflow accessible to scientists learning AI

Applied In
01_preprocessing.ipynb

02_feature_engineering.ipynb

03_model_training.ipynb
