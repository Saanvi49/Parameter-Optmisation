# Parameter-Optmisation

 Experiment on SVM Parameter Optimization
This document describes an experiment on optimizing the parameters of a Support Vector Machine (SVM) classifier.

Objective:

Investigate the impact of parameter tuning on SVM performance for a multi-class classification task.
Data:

Source: UCI Machine Learning Repository - Dry Beans Dataset
Description: This dataset contains images of 13,611 dry beans from 7 different varieties. Each data point has 16 features, including 12 dimensional measurements and 4 shape descriptors.
Size: The dataset has a moderate size, falling between 5,000 and 30,000 data points.
Methodology:

Data Split: Divide the dataset into training (70%) and testing (30%) sets. Repeat this split process 10 times to create 10 independent samples.

SVM Training: Train a separate SVM model on each of the 10 training sets.

Parameter Optimization:

For each training run:
Perform 100 iterations of parameter optimization to find the best combination of hyperparameters for the SVM model.
The specific hyperparameters to be optimized will be determined later (e.g., regularization parameter (C), kernel coefficient (gamma)).
Evaluation:

Evaluate the performance (e.g., accuracy) of each trained SVM model on its corresponding testing set.
Identify the sample that achieves the highest overall accuracy.
Convergence Analysis:

Plot the convergence graph for the model with the highest accuracy. This graph will visualize how the model's performance improves with each iteration of parameter optimization.
Reporting:

Summarize the best hyperparameter values found for each of the 10 training

Comparative performance of Optimised-SVM with different samples
Sample	Best Accuracy	Best Kernel	Best Nu	Best Epsilon
S1	0.2738	poly	0.0042	0.0584
S2	0.2738	rbf	0.5005	0.2004
S3	0.2689	rbf	0.8394	0.9629
S4	0.2372	rbf	0.2994	0.4927
S5	0.2567	rbf	0.1199	0.4537
S6	0.1516	poly	0.9484	0.9200
S7	0.2249	rbf	0.2923	0.4514
S8	0.2200	rbf	0.1372	0.4763
S9	0.2836	poly	0.9883	0.1702
S10	0.0293	sigmoid	0.1866	0.8548
Convergence Graph
line-plot.png

The last iteration seems to be an anomaly which we can ignore.


Saanvi Sharma 
102103699
