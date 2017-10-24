#GPU training scripts

Scripts to run GPU versions of XGBoost, LightGBM, CatBoost, compute quality metrics (and their plots) for trained models and extract learning time from logs.

run_experiment_*.py scrips just perform training with different values of regularization (shrinkage/step) and use auto-stop to find best iteration (round). After that scrips measure time which we need to learn ensemble of desired size and computes table with columns (best_tree_count, score, time_to_learn_best_tree_count). 

exctract_scores_*.py scrips were used to parse one experiment logs and take time/quality statistics from them
