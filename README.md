BiofilmAI — Multimodal Prediction of Biofilm Formation
--Image of: --Python --Image of: --Jupyter --Image of: --Scientific Computing --Image of: --Microbiology

BiofilmAI is an open-source scientific machine learning research project dedicated to predicting, modeling, and analyzing biofilm formation [11]. This repository serves as your core computational research and ML development sandbox, housing raw experimental notebooks, preprocessing pipelines, and biological feature engineering frameworks.

🚀 Live Interactive App Deployment
To interact with these models through a user-friendly, web-based clinical dashboard, visit the live deployment repository:

Live App Link: Launch the BiofilmAI Lab Suite (beta)
Deployment Codebase: lab-ai-compliance-suite
🔬 Multi-Phase Research Roadmap & Notebooks
The research framework is built as a multi-phase modular pipeline designed to scale from single-modality studies to unified multimodal predictions [1]:

🧬 Phase 1: Project A — Transcriptomic Machine Learning (Active)
Predicts biofilm formation thresholds using gene expression data from the public GSE87213 dataset, studying Pseudomonas aeruginosa ΔPA14_22470 (ΔPA3225) versus wildtype strains across planktonic and biofilm conditions [1].

01_preprocessing.ipynb — Ingests raw differential expression profiles, resolves missing values, and aligns transcript data [1].
02_feature_engineering.ipynb — Engineers biological interaction terms, significance flags ($|logFC| > 1.5$, $p < 0.05$), and mutant-to-wildtype ratio metrics [1].
03_model_training.ipynb — Trains classification systems (Random Forests, Gradient Boosting, Logistic Regression) and maps machine learning feature importances back to biochemical pathways [1].
04_feature_importance.ipynb — Analyzes SHAP values and model parameters to determine the biological driving forces behind predictions.
05_gene_level_predictions.ipynb — Implements scaled model pipeline inference for targeted single-gene predictions.
📸 Phase 2: Project B — BiofilmNN Deep Learning (In Development / Upcoming)
A convolutional deep learning pipeline designed to analyze Confocal Laser Scanning Microscopy (CLSM), SEM, and fluorescence images [1, 3].

Upcoming Notebooks: Preprocessing dual-channel image files, segmenting multicellular biomass, and extracting cell count, live/dead ratios, and surface roughness as numerical features [1].
🔗 Phase 3: Project C — Multimodal Fusion Hub (Planned / Upcoming)
A unified early- and late-stage fusion framework combining transcriptomic features with microscopy-derived morphological features [1].

Upcoming Notebooks: Feature vector concatenation, cross-modal normalization, and comparative evaluation of multimodal classifiers versus single-modality predictors to enhance biofilm classification accuracy [1].
🗂️ Repository Directory Structure
BiofilmAI/
├── notebooks/                         # Core ML Development Sandbox
│   ├── 01_preprocessing.ipynb          # Raw DE transcript cleanup & alignment
│   ├── 02_feature_engineering.ipynb    # Biological interaction & ratio metrics
│   ├── 03_model_training.ipynb         # Classifier training
│   ├── 04_feature_importance.ipynb    # Model parameter & pathway relevance mapping
│   └── 05_gene_level_predictions.ipynb # Scaled single-gene pipeline inference
├── data/
│   ├── gene_expression/               # GSE87213 differential expression csv files
│   │   ├── biofilm_diff_expr.csv
│   │   ├── planktonic_diff_expr.csv
│   │   └── ml_feature_tables.csv
│   ├── microscopy_images/             # Raw microscopy and mask files (Upcoming)
│   └── fused_features/                # Aligned cross-modal training sets (Upcoming)
├── models/                            # Saved trained model and scaler files (.pkl)
├── src/                               # Helper utility python scripts
└── README.md
🧪 "Vibe Coding" — My Scientific Coding Philosophy
All computational work in this repository follows Vibe Coding, a deliberate, narrative-driven scientific programming style. Rather than presenting static, dense blocks of code, this approach structures each Jupyter Notebook as an active, guided scientific journal entry.

Core Principles of Scientific Vibe Coding
Narrative-Driven Steps: Every block of code is preceded by a markdown cell explaining why the step is being taken, what biological assumptions are being made, and how the output feeds into the next stage of the pipeline.
Domain-Friendly Naming: Variable names, function parameters, and dataframe columns are named after their biological or statistical realities (e.g., is_significantly_upregulated, biofilm_logfc_p_value_ratio) rather than generic placeholders like df1 or x.
Intermediate Visual Intuition: We visualize data distributions, pipeline check-points, and intermediate calculations instantly using plots and data previews to confirm that our transformations align with biological logic.
Purpose-Driven Code Blocks: Functions are kept small, highly modular, and single-purpose to maximize readability and testing ease for both data scientists and molecular biologists.
Scientific Closures: Every notebook ends with a retrospective "Summary of Discoveries" block that highlights data dimensions, statistical findings, or modeling results to maintain continuity across experimental phases.
💡 Conceptual Bio-AI Portfolios
This repository also serves as the intellectual showcase for several innovative, planned, and conceptual biological AI architectures [1]:

BiofilmNN — AI for Microbial Imaging: A conceptual deep-learning system designed to analyze CLSM, SEM, and fluorescence microscopy images. BiofilmNN explores how AI can support microbial imaging workflows by extracting diagnostic features directly from pixel-level biological data [3].
Automated PCR Optimizer — AI for Molecular Assay Development: A Python-based concept tool using Bayesian optimization to streamline PCR protocol development. This project explores how AI can reduce validation time, improve assay robustness, and support molecular diagnostics across diverse laboratory workflows [3].
AMR Prediction Framework — AI for Antimicrobial Resistance Diagnostics: A proposed AI model integrating FISH-based imaging and gene expression profiles to support antimicrobial resistance testing. This framework investigates how multimodal data can improve early AMR detection and clinical decision-making [5].
Microbiome Visualization Tools: A planned suite of AI-assisted dashboards designed to visualize polymicrobial community dynamics. These tools aim to make microbiome behavior interpretable through interactive visualizations, supporting ecological modeling and diagnostic insight [5].
🛠️ Local Installation & Usage
To set up your environment and run the notebooks locally:

1. Clone the Repository
git clone https://github.com/mariabgcenter-lab/BiofilmAI.git
cd BiofilmAI
2. Create and Activate a Virtual Environment
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
3. Install Jupyter & Dependencies
pip install jupyterlab pandas numpy matplotlib seaborn scikit-learn joblib
4. Launch Jupyter Lab
jupyter lab
📬 Academic & Professional Profiles
Explore my peer-reviewed publications, open-source code repositories, and professional networks [4, 9]:

Portfolio Showcase: Maria BG Scientific Portfolio
ORCID: 0000-0002-7525-4262
Google Scholar: Maria BG Profile
LinkedIn: maria-burgos-garay
GitHub: mariabgcenter-lab
© 2026 Maria BG Scientific. Developed under an agile, open-science model at the intersection of advanced microbiology, clinical data standards, and AI-driven biological discovery.
