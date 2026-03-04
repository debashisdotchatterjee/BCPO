# BCPO-lite Offline RL Validation 

This zip contains outputs from a *synthetic* offline RL benchmark (tabular gridworld).
In the environment that generated this zip, Gym/Gymnasium/MuJoCo are not installed, so D4RL tasks cannot be run here.
However, the included Colab script shows how to run the same workflow on **D4RL** (Fu et al., 2020) when available,
and falls back to this synthetic benchmark otherwise.

## Summary (this run)
                              model  return_mean  return_std
BCPO-lite (Bayesian pessimism + KL)     0.627816    0.141993
              Behavior Cloning (BC)     0.317548    0.473956
      Naive FQI (MLE, no pessimism)    -0.199036    0.204948

## Key plots
- plot_learning_curves.png
- plot_coverage_vs_uncertainty.png
- plot_state_values_bcpo.png, plot_state_values_fqi.png
- plot_policy_bcpo.png, plot_policy_fqi.png
