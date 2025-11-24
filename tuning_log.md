# Tuning Log

This file will contain all hyperparameter changes and small experiments.

(Example entries will be added after training begins.)
## Run 1 – Pong baseline DQN

- Environment: ALE/Pong-v5
- Episodes: 300
- Discount (gamma): 0.99
- Optimizer: Adam, learning rate 1e-4
- Replay buffer: 10,000; batch size: 32
- Target network sync: every 1,000 frames
- Epsilon schedule: 1.0 → 0.01 over 150,000 frames
- Result: mean return over last 100 episodes improved from about −21.0 to about −20.0
- Saved model: `models/ALE_Pong-v5-baseline_best_-19-20251124-0055.dat`
- Learning curve: `figures/curve_dqn_baseline.png`
## Run 2 — DDQN + Dueling
- Date: 2025-11-24
- Commit: <paste your commit hash>
- Model file: ALE_Pong-v5-DDQN-dueling-best.dat
- Curve image: figures/curve_pong_ddqn_dueling.png
- Episodes: 300
- Best reward: (whatever your best was, e.g., -19)
- Notes:
  - Added Dueling architecture + DDQN update rule.
  - Training slightly slower than baseline.
  - Reward improved slightly compared to baseline.
