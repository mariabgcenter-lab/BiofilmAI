BiofilmAI — Machine Learning Research Sandbox & Notebooks
--Image of: --Python --Image of: --Jupyter --Image of: --Scientific Computing --Image of: --Microbiology

BiofilmAI is an open-source scientific machine learning research project dedicated to predicting, modeling, and analyzing biofilm formation. This repository houses the core computational research, exploratory data analysis notebooks, and machine learning model training pipelines.

To see these models packaged into a live interactive web app with clinical compliance assistants, visit the companion repository: lab-ai-compliance-suite.

🗂️ Computational Directory Structure
This repository is dedicated entirely to data pipelines, model sandbox development, and scientific exploration:

BiofilmAI/
├── notebooks/                         # Core ML Development Sandbox
│   ├── 01_preprocessing.ipynb          # Raw DE transcript cleanup & alignment
│   ├── 02_feature_engineering.ipynb    # Biological interaction & ratio metrics
│   ├── 03_model_training.ipynb         # Classifier training (RF, Logistic Regression)
│   ├── 04_feature_importance.ipynb    # Model parameter & pathway relevance mapping
│   └── 05_gene_level_predictions.ipynb # Scaled single-gene pipeline inference
├── data/                              # Structured Research Datasets
│   ├── gene_expression/               # GSE87213 differential expression csv files
│   │   ├── biofilm_diff_expr.csv
│   │   ├── planktonic_diff_expr.csv
│   │   └── ml_feature_tables.csv
│   └── microscopy_images/             # Raw microscopy images (Upcoming)
├── models/                            # Saved trained model files (.pkl)
├── src/                               # Helper utility python scripts
└── README.md                          # Repository documentation
🧬 Scientific Research Roadmap
Phase 1: Project A — Transcriptomic Machine Learning (Active)
Predicts biofilm formation thresholds using gene expression data from the public GSE87213 dataset, studying Pseudomonas aeruginosa ΔPA14_22470 (ΔPA3225) versus wildtype strains across planktonic and biofilm conditions.

01_preprocessing.ipynb — Ingests raw differential expression profiles, resolves missing values, and aligns transcript data.
02_feature_engineering.ipynb — Engineers biological interaction terms, significance flags ($|logFC| > 1.5$, $p < 0.05$), and mutant-to-wildtype ratio metrics.
03_model_training.ipynb — Trains classification systems (Random Forests, Gradient Boosting) and maps machine learning feature importances back to biochemical pathways.
04_feature_importance.ipynb — Analyzes SHAP values and model parameters to determine biological driving forces behind predictions.
05_gene_level_predictions.ipynb — Implements scaled model pipeline inference for targeted single-gene predictions.
Phase 2: Project B — BiofilmNN Deep Learning (In Development / Upcoming)
A convolutional deep learning pipeline designed to analyze Confocal Laser Scanning Microscopy (CLSM), SEM, and fluorescence images.

Upcoming Notebooks: Preprocessing dual-channel image files, segmenting multicellular biomass, and extracting cell count, live/dead ratios, and surface roughness as numerical features.
Phase 3: Project C — Multimodal Fusion (Planned / Upcoming)
A unified early- and late-stage fusion framework combining transcriptomic features with microscopy-derived morphological features.

Upcoming Notebooks: Feature vector concatenation, cross-modal normalization, and comparative evaluation of multimodal classifiers versus single-modality predictors to enhance biofilm classification accuracy.
🧪 "Vibe Coding" — My Scientific Coding Philosophy
All computational work in this repository follows Vibe Coding, a deliberate, narrative-driven scientific programming style. Rather than presenting static, dense blocks of code, this approach structures each Jupyter Notebook as an active, guided scientific journal entry.

Core Principles of Scientific Vibe Coding
Narrative-Driven Steps: Every block of code is preceded by a markdown cell explaining why the step is being taken, what biological assumptions are being made, and how the output feeds into the next stage of the pipeline.
Domain-Friendly Naming: Variable names, function parameters, and dataframe columns are named after their biological or statistical realities (e.g., is_significantly_upregulated, biofilm_logfc_p_value_ratio) rather than generic placeholders like df1 or x.
Intermediate Visual Intuition: We visualize data distributions, pipeline check-points, and intermediate calculations instantly using plots and data previews to confirm that our transformations align with biological logic.
Purpose-Driven Code Blocks: Functions are kept small, highly modular, and single-purpose to maximize readability and testing ease for both data scientists and molecular biologists.
Scientific Closures: Every notebook ends with a retrospective "Summary of Discoveries" block that highlights data dimensions, statistical findings, or modeling results to maintain continuity across experimental phases.
🛠️ Local Installation & Environment
To set up a local Python environment and run these research notebooks:

1. Clone the Repository
git clone https://github.com/mariabgcenter-lab/BiofilmAI.git
cd BiofilmAI
2. Create and Activate Environment
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
3. Install Dependencies
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn joblib
4. Launch Jupyter Lab
jupyter lab
📬 Academic & Professional Profiles
Explore my peer-reviewed publications, open-source code repositories, and professional networks:




