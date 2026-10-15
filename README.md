# Improving BacTermFinder: Extending Its Field of Vision and Identifying Predicted Terminator Types

### Key Highlights

- **Improved model recall by 15%** on a bioinformatics sequence-classification task through systematic experimentation with extended **200-nucleotide sequence inputs**.
- **Built a tree-based classifier in Python achieving an 85% F1 score** using nucleotide-based feature engineering, cross-validation, and rigorous evaluation of model generalization.
- **Extended BacTermFinder's capabilities** to distinguish between intrinsic and Rho-dependent transcription terminators, addressing limitations in the original model.

## Overview

Transcription termination is a crucial phase of gene expression in bacteria, where the emerging transcript and the RNA polymerase are released from each other and from the DNA template. Transcription termination occurs through two mechanisms: intrinsic and factor-dependent terminators. Intrinsic terminators function independently of external proteins, relying instead on specific signals encoded in the DNA template and emerging transcript. In contrast, factor-dependent terminators require the Rho protein, which binds ribosome-free RNA at designated Rho utilization sites (RUT).

BacTermFinder, a recently published computational tool, effectively predicts transcription terminators; however, it has two major limitations. First, its training data mostly exclude the RUT region, and second, it is unable to classify terminators by their type. To address these limitations, this study presents an approach involving retraining BacTermFinder by extending its input sequences to 200 nucleotides, thus improving recall over a set of validation data. Additionally, we introduce a tree-based classifier capable of distinguishing between intrinsic and factor-dependent terminators based on nucleotide-derived features. This classification model provides deeper insights into bacterial gene regulatory mechanisms and contributes to the understanding of transcription termination complexity.
