# Bandit Bounds Simulation

Simulation code for the review paper **"Upper and Lower Reward Bounds in 
Reinforcement Learning: From Multi-Armed to Linear Bandits"**.

## Reproducing the figures

1. Install dependencies: `pip install -r requirements.txt`
2. Run: `python bandits_simulation.py`
3. Outputs: `ucb1_regret.pdf`, `oful_regret.pdf`

## What the code does

- **UCB1**: simulates the UCB1 algorithm (Auer et al., 2002) on a 5-armed 
  Bernoulli bandit and plots the cumulative regret alongside the theoretical 
  upper bound `8 Σ ln(n)/Δ²`.
- **OFUL**: simulates the OFUL algorithm (Abbasi-Yadkori et al., 2011) on a 
  3-dimensional linear bandit with 20 random actions on the unit sphere, 
  and plots the empirical regret alongside the theoretical bound.

## References

- Auer, Cesa-Bianchi, Fischer (2002). *Finite-time Analysis of the 
  Multiarmed Bandit Problem*. Machine Learning, 47(2–3), 235–256.
- Abbasi-Yadkori, Pál, Szepesvári (2011). *Improved Algorithms for Linear 
  Stochastic Bandits*. NIPS 24.
