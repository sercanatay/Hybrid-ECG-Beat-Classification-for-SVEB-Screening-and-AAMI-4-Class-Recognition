Implemented an end-to-end machine learning pipeline for ECG beat/arrhythmia classification
using the MIT-BIH Supraventricular Arrhythmia Database (SVDB).

Key additions:
- Dataset ingestion utilities for SVDB (Kaggle/PhysioNet source)
- Preprocessing steps (signal cleaning, optional bandpass, normalization)
- Beat/segment construction logic (fixed-length windows around annotated beats)
- Label handling and class mapping (project-specific label schema)
- Train/validation/test split strategy and reproducible random seeds
- Model training script/notebook + evaluation (confusion matrix, F1, ROC/PR metrics)
- Saved artifacts (trained model weights + metrics export)

Notes:
- Raw ECG data is NOT committed. Data directory is gitignored.
- SVDB is an open dataset (PhysioNet). See dataset pages for licensing/terms.

Dataset references:
- Kaggle: protobioengineering/mit-bih-supraventricular-arrhythmia-database
- PhysioNet: MIT-BIH Supraventricular Arrhythmia Database (svdb)
