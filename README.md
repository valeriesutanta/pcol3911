# Organophosphate QSAR Model

This repository contains the code and processed data for a QSAR modelling assignment investigating the relationship between organophosphate chemical structure and acetylcholinesterase binding activity.

The original dataset was derived from Veselinović et al. and contains organophosphate structures represented as SMILES strings and Expr values representing log10-transformed human bimolecular rate constants for AChE binding.

## Files

- `1_Get_OP_Data_Generate_FingerPrints.ipynb`: Loads the original SMILES/Expr dataset and converts SMILES into Morgan fingerprint descriptors.
- `organophosphate_fp.csv`: Processed descriptor dataset containing molecular fingerprint bits and the Expr outcome column.
- `2_Making_a_QSAR_model.ipynb`: Trains an initial Random Forest regression model to predict Expr.
- `first_rfr.pkl`: Saved initial Random Forest model.
- `3_Cross_validation.ipynb`: Performs hyperparameter tuning using cross-validation and evaluates the best model on a hold-out test set.
- `best_random_forest_model.pkl`: Saved optimised Random Forest model.
