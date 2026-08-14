BiofilmAI — Multimodal Prediction of Biofilm Formation
BiofilmAI is a scientific machine learning project designed to analyze and predict biofilm formation using differential gene expression data from the GSE87213 dataset.
The project integrates microbiology expertise with modern AI workflows, using a clear, expressive coding philosophy called Vibe Coding.

Project Structure
notebooks/
Contains Jupyter notebooks for preprocessing, feature engineering, and model development.

01_preprocessing.ipynb — loads raw data, cleans gene expression tables, merges differential expression results, and prepares machine learning features.

02_feature_engineering.ipynb — constructs engineered features such as interaction terms, ratios, absolute log fold changes, significance flags, and condition‑specific metrics.

03_model_training.ipynb — trains baseline machine learning models and evaluates predictive performance.

data/gene_expression/
Contains all gene expression files used in the project:

Biofilm differential expression results

Planktonic differential expression results

Biofilm vs planktonic comparison tables

Cleaned differential expression tables

Machine learning feature tables

Dataset: GSE87213
Differential gene expression of Pseudomonas aeruginosa ΔPA14_22470 (ΔPA3225) versus wildtype in planktonic and biofilm conditions.

This dataset provides the biological foundation for BiofilmAI’s predictive modeling pipeline.

Project Goal
To build a machine learning model that predicts biofilm formation using:

log fold changes

adjusted p‑values

condition‑specific gene expression patterns

engineered machine learning features

This project demonstrates how biological insight and AI engineering can be combined to understand complex microbial behaviors.

Vibe Coding — My Scientific Coding Style
Vibe Coding is the coding philosophy used throughout BiofilmAI to improve clarity, readability, and scientific workflow structure.
It transforms each notebook into a guided scientific narrative rather than a block of code.

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
