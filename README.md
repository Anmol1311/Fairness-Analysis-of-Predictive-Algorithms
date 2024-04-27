# Fairness-Analysis-of-Predictive-Algorithms

## Project Overview and Objective
In recent years, the criminal justice system has increasingly turned to technological advancements to enhance decisionmaking processes. Among these technologies, predictive algorithms stand out as powerful tools designed to estimate the likelihood of an individual reoffending. These algorithms, which are employed at various stages of the criminal process, ncluding parole decisions, sentencing, and notably bail hearings, leverage historical data to generate predictions about future behaviors.

While the use of these predictive algorithms in criminal justice enhances decision-making, it also raises ethical concerns. As these systems are deployed as decision-support tools influencing individual outcomes, it is vital
to address question of fairness of these algorithms.

One such predictive tool is COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) which evaluates the risk of recidivism among criminals. In this project, we utilized the hostorical COMPAS data to evaluate the fairness levels of the prediction algorithm.

## Data Sources
https://www.kaggle.com/datasets/danofer/compass/data

## Findings:

1. African Americans have a higher False Positve Rate, and more individuals from this group may be unjustly subjected to harsher sentences or parole conditions
2. Caucasians have a higher False Negative Rate, which could mean that the system is underestimating the risk of recidivism in this group
3. The predictive alogorithm also fails to meet the 3 criteria (Predictive Parity, Equalized Odds and Demographic Parity) for fairness assessment of the model
   <img width="750" alt="image" src="https://github.com/Anmol1311/Fairness-Analysis-of-Predictive-Algorithms/assets/142256926/eb975475-2050-453b-9c04-a081a1cad65a">

   
## Possible Mitigation Techniques:
Resampling of data to ensure equal representation of all communities
Reweighting the under represented communities to avoid sampling bias
