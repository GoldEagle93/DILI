03_Cmax.ipynb
1. Load and clean up data.
2. Reduce number of features by variance threshold (VT) on train data (Train_data_liv_tox_12133)
3. Filter all data for only the features selected after VT reduction.
4. Generate features for Cmax molecules
5. Combine Cmax labels with selected features from training data. C_total: median pMolar total plasma concentration; C_unbound: median pMolar unbound plasma concentration.
6. Train Cmax models (unbound and total)
7. Add predicted Cmax values for Goldstandard data
8. Train a new model on Goldstandard with only Cmax feature.
9. Test if Cmax features are good for predicting DILI toxicity.
10. Train individual models based on data from each source.
11. Test against test data and save the best model.
12. Repeat steps 11 and 12 with different combination of features (mfps, mordered, MACCS, Cmax, Liv models, etc.)