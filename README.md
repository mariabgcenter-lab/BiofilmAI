# BiofilmAI — Multimodal Prediction of Biofilm Formation

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Scientific Computing](https://img.shields.io/badge/SciPy-Ecosystem-green.svg)](https://scipy.org/)
[![Microbiology](https://img.shields.io/badge/Microbiology-Biofilms-red.svg)](https://en.wikipedia.org/wiki/Biofilm)

**BiofilmAI** is an open-source scientific machine learning research project dedicated to predicting, modeling, and analyzing biofilm formation. This repository houses the core computational research, exploratory data analysis notebooks, and machine learning model training pipelines.

The research framework is built as a multi-phase modular pipeline designed to scale from single-modality studies to unified multimodal predictions:
1. **Project A (Genomic Profiling):** Predictive modeling using differential transcriptomics.
2. **Project B (BiofilmNN):** High-throughput computer vision analysis of microbial microscopy images.
3. **Project C (Multimodal Fusion):** Dual-channel feature alignment linking genomic profiles and bioimage phenotypes for integrated biofilm prediction.

---

## 🔬 Multi-Phase Research Roadmap & Modules

### 🧬 Phase 1: Project A — Transcriptomic Machine Learning (Active)
Predicts biofilm formation thresholds using gene expression data from the public **GSE87213** dataset, studying *Pseudomonas aeruginosa* ΔPA14_22470 (ΔPA3225) versus wildtype strains across planktonic and biofilm conditions.
*   **01_preprocessing.ipynb** — Ingests raw differential expression profiles, resolves missing values, and aligns transcript data.
*   **02_feature_engineering.ipynb** — Engineers biological interaction terms, significance flags ($|logFC| > 1.5$, $p < 0.05$), and mutant-to-wildtype ratio metrics.
*   **03_model_training.ipynb** — Trains classification systems (Random Forests, Gradient Boosting) and maps machine learning feature importances back to biochemical pathways.

### 📸 Phase 2: Project B — BiofilmNN Deep Learning (In Development / Upcoming)
A convolutional deep learning pipeline designed to analyze Confocal Laser Scanning Microscopy (CLSM) and fluorescence images.
*   *Upcoming Notebooks:* Preprocessing dual-channel image files, segmenting multicellular biomass, and extracting cell count, live/dead ratios, and surface roughness as numerical features.

### 🔗 Phase 3: Project C — Multimodal Fusion Hub (Planned / Upcoming)
A unified early- and late-stage fusion framework combining transcriptomic features with microscopy-derived morphological features.
*   *Upcoming Notebooks:* Feature vector concatenation, cross-modal normalization, and comparative evaluation of multimodal classifiers versus single-modality predictors to enhance biofilm classification accuracy.

---

## 🗂️ Proposed Directory Structure

To support ongoing development across all three projects, the repository directory is organized as follows:

```directory
BiofilmAI/
├── notebooks/
│   ├── project_a_genomics/            # Phase 1: Gene Expression Pipelines
│   │   ├── 01_preprocessing.ipynb
│   │   ├── 02_feature_engineering.ipynb
│   │   └── 03_model_training.ipynb
│   ├── project_b_biofilmnn/           # Phase 2: Microscopy Computer Vision (Upcoming)
│   │   └── 01_image_segmentation.ipynb
│   └── project_c_multimodal/          # Phase 3: Cross-Modal Fusion (Upcoming)
│       └── 01_feature_alignment.ipynb
├── data/
│   ├── gene_expression/               # GSE87213 differential expression csv files
│   │   ├── biofilm_diff_expr.csv
│   │   ├── planktonic_diff_expr.csv
│   │   └── ml_feature_tables.csv
│   ├── microscopy_images/             # Raw microscopy and mask files (Upcoming)
│   └── fused_features/                # Aligned cross-modal training sets (Upcoming)
└── README.md
🧪 "Vibe Coding" — My Scientific Coding Philosophy
All computational work in this repository follows Vibe Coding, a deliberate, narrative-driven scientific programming style. Rather than presenting static, dense blocks of code, this approach structures each Jupyter Notebook as an active, guided scientific journal entry.
Core Principles of Scientific Vibe Coding
Narrative-Driven Steps: Every block of code is preceded by a markdown cell explaining why the step is being taken, what biological assumptions are being made, and how the output feeds into the next stage of the pipeline.
Domain-Friendly Naming: Variable names, function parameters, and dataframe columns are named after their biological or statistical realities (e.g., is_significantly_upregulated, biofilm_logfc_p_value_ratio) rather than generic placeholders like df1 or x.
Intermediate Visual Intuition: We visualize data distributions, pipeline check-points, and intermediate calculations instantly using plots and data previews to confirm that our transformations align with biological logic.
Purpose-Driven Code Blocks: Functions are kept small, highly modular, and single-purpose to maximize readability and testing ease for both data scientists and molecular biologists.
Scientific Closures: Every notebook ends with a retrospective "Summary of Discoveries" block that highlights data dimensions, statistical findings, or modeling results to maintain continuity across experimental phases.
🛠️ Installation & Usage
1. Clone the Repository
git clone https://github.com/mariabgcenter-lab/BiofilmAI.git
cd BiofilmAI
2. Create and Activate a Virtual Environment
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
3. Install Dependencies
pip install -r requirements.txt
4. Run the Notebooks
Launch Jupyter Lab or Jupyter Notebook to step through the pipeline:
jupyter lab
📬 Academic & Professional Profiles
Explore my peer-reviewed publications, open-source code repositories, and professional networks:
ORCID: 0000-0002-7525-4262
Google Scholar: Maria BG Profile
LinkedIn: maria-burgos-garay
Portfolio Showcase: Maria BG Scientific Portfolio
© 2026 Maria BG Scientific. Developed under an agile, open-science model at the intersection of advanced microbiology and AI-driven biological discovery.

***
