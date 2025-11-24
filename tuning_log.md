# Tuning Log – ALE/Pong-v5

This file documents the three main runs used in this project.

---

## Run 1 – DQN Baseline

- **Run ID:** pong_baseline
- **Model path:**  
  `models/pong_baseline/ALE_Pong-v5-baseline_best_-19-20251124-0055.dat`
- **Figure path:**  
  `figures/pong_baseline/curve_dqn_baseline.png`
- **Episodes:** 300
- **Algorithm:** DQN
- **Notes:**  
  Baseline run to compare later experiments. Improves slightly from −21 to about −20.

---

## Run 2 – DDQN + Dueling DQN

- **Run ID:** pong_run2
- **Commit hash:** 9cc549e
- **Model path:**  
  `models/pong_run2/ALE_Pong-v5-best_-19-20251124-0034-test_epsdec150000_rs10000_sync1000.dat`
- **Figure path:**  
  `figures/pong_run2/curve_pong_ddqn_dueling.png`
- **Episodes:** 300
- **Algorithm:** Double DQN + Dueling DQN
- **Notes:**  
  More stable training due to DDQN. Better state representation due to dueling head.

---

## Run 3 – Final Tuned Run

- **Run ID:** pong_final
- **Model path:**  
  `models/pong_final/ALE_Pong-v5-baseline_best_-19-20251124-0147.dat`
- **Figure path:**  
  `figures/pong_final/curve_pong_final.png`
- **Episodes:** 300
- **Algorithm:** DQN (tuned)
- **Hyperparameter change:**  
  Learning rate reduced for stability.
- **Notes:**  
  Produces smoother training dynamics compared to baseline.
