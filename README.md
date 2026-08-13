# BiofilmAI — Multimodal Prediction of Biofilm Formation

BiofilmAI is a scientific machine learning project designed to analyze and predict biofilm formation using gene expression data from the GSE87213 dataset.

## Project Structure

### notebooks/
Contains Jupyter notebooks for preprocessing and analysis.
- 01_preprocessing.ipynb — loads raw data, cleans gene expression tables, merges differential expression results, and prepares machine learning features.

### data/gene_expression/
Contains all gene expression files used in the project:
- Biofilm differential expression results
- Planktonic differential expression results
- Biofilm vs planktonic comparison tables
- Cleaned differential expression tables
- Machine learning feature tables

## Dataset: GSE87213
Differential gene expression of Pseudomonas aeruginosa ΔPA14_22470 (ΔPA3225) versus wildtype in planktonic and biofilm conditions.

## Project Goal
To build a machine learning model that predicts biofilm formation using:
- log fold changes
- adjusted p-values
- condition-specific gene expression patterns
- engineered machine learning features

## Next Steps
- Add model training notebook
- Add evaluation metrics
- Add visualization outputs
