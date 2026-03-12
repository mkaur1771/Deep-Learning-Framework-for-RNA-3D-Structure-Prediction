# NeuralRNAFold
## Deep Learning Framework for RNA 3D Structure Prediction

NeuralRNAFold is a deep learning framework designed to predict the **three-dimensional structure of RNA molecules directly from nucleotide sequences**. The project was developed in the context of the **Stanford RNA 3D Folding Challenge (Kaggle)** and explores how neural networks can learn structural patterns governing RNA folding.

RNA molecules play critical roles in biological systems including **gene regulation, catalysis, and RNA-based therapeutics**. However, determining RNA structures experimentally using methods such as **X-ray crystallography, cryo-electron microscopy, or NMR spectroscopy** is expensive and time-consuming.

NeuralRNAFold explores how **machine learning can infer RNA spatial structure directly from sequence data**, offering a scalable computational alternative.

---

# 📌 Problem Statement

Predict the **3D coordinates of each nucleotide residue**.

For the Kaggle challenge the system must generate:

- **Five candidate 3D structures** per RNA sequence
- Predicted coordinates for every residue
- Structures evaluated using **TM-score**

---

# 🗂️ Project Pipeline

```text
.
RNA Sequence
↓
Token Encoding
↓
Embedding Layer
↓
Transformer Feature Learning
↓
Coordinate Prediction
↓
3D Structure Reconstruction
↓
Multi-Structure Sampling
```

---

# Dataset

Dataset from:

**Stanford RNA 3D Folding Challenge — Kaggle**

The dataset includes:

- RNA nucleotide sequences  
- Multiple sequence alignments (MSA)  
- Experimentally solved RNA structures  
- Residue-level atomic coordinates  

Goal: predict **RNA folding structures for unseen sequences**.

---
# Repository Structure
```text
NeuralRNAFold
│
├── README.md
├── requirements.txt
│
├── notebooks
│ └── stanford_rna_3d_folding_pipeline.ipynb
│
├── src
│ ├── data_processing.py
│ ├── model.py
│ ├── training.py
│ └── inference.py
│
├── visualization
│ ├── training_curves.py
│ ├── structure_projection.py
│
├── results
│ ├── training_loss_plot.png
│ ├── structure_projection.png
│ └── distance_matrix.png
│
└── docs
└── project_overview.md
```

# 🔮Future Work

Potential improvements include:

- Secondary structure-aware modeling
- Graph neural networks for residue interactions
- MSA attention mechanisms
- Distance-map based structural learning
- Ensemble prediction strategies

These directions aim to move toward **state-of-the-art RNA folding models**.

Dataset and challenge provided by:

**Stanford RNA 3D Folding Challenge — Kaggle**

