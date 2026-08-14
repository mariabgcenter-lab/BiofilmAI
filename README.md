# BiofilmAI — Multimodal Prediction of Biofilm Formation

BiofilmAI is a scientific machine learning project designed to analyze and predict biofilm formation using gene expression data from the GSE87213 dataset.

## Project Structure

### notebooks/
Contains Jupyter notebooks for preprocessing, feature engineering, and model development.
- 01_preprocessing.ipynb — loads raw data, cleans gene expression tables, merges differential expression results, and prepares machine learning features.
- 02_feature_engineering.ipynb — constructs engineered features such as absolute log fold changes, significance flags, and condition-specific metrics.
- 03_model_training.ipynb — trains baseline machine learning models and evaluates predictive performance.

### data/gene_expression/
Contains all gene expression files used in the project:
- Biofilm differential expression results  
- Planktonic differential expression results  
- Biofilm vs planktonic comparison tables  
- Cleaned differential expression tables  
- Machine learning feature tables  

## Dataset: GSE87213
Differential gene expression of *Pseudomonas aeruginosa* ΔPA14_22470 (ΔPA3225) versus wildtype in planktonic and biofilm conditions.

## Project Goal
To build a machine learning model that predicts biofilm formation using:
- log fold changes  
- adjusted p-values  
- condition-specific gene expression patterns  
- engineered machine learning features  

## Coding Style: Vibe Coding Module
The Vibe Coding module is used throughout Project A to improve clarity, readability, and scientific workflow structure.

### Purpose
To develop clean, intuitive, and expressive coding habits while working through preprocessing, feature engineering, and model training.

### Principles
- Write code in clear narrative steps  
- Use microbiology-friendly variable names  
- Visualize intermediate results for intuition  
- Maintain consistent formatting and structure  
- Keep functions small, readable, and purposeful  

### Applied In
- 01_preprocessing.ipynb  
- 02_feature_engineering.ipynb  
- 03_model_training.ipynb  

## Next Steps
- Expand model training notebook  
- Add evaluation metrics and visualizations  
- Integrate coding style improvements (Vibe Coding)  
- Prepare features for multimodal integration  
