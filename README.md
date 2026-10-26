# FIFA 21 player classification

Aadil Ali Vagh and Nicodemus Ong

Predict whether a FIFA 21 outfield player is attacking or defensive, then cluster the players. The write-up is a short R notebook with the saved plots from the original analysis.

## Result

- 8,004 attacking and 8,900 defensive players, after goalkeepers are removed
- Null-model AUC 0.50. Interceptions alone reach an AUC of about 0.93
- A decision tree and 10-nearest neighbours both land near 0.91 accuracy on a 30% holdout
- Four clusters: a higher-rated defensive-leaning group, a defensive group, an attacking group that does not hold up under bootstrap resampling, and a younger group

Open [fifa21-player-classification.ipynb](fifa21-player-classification.ipynb). GitHub renders the notebook and the figures. Re-running it needs R and the [FIFA 21 messy raw dataset](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring) (`fifa21_raw_data.csv`).

Dashboard walkthrough: https://youtu.be/tlGLk1NIcFU
