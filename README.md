# **CSCI 166 – Deep Q-Learning on Atari Pong**
Implementation and analysis of Deep Q-Learning for **ALE/Pong-v5**, using Gymnasium and PyTorch in Google Colab.

---

## **Overview**
This repository contains my implementation and experiments with Deep Q-Learning on the Atari game **Pong**, following a structured three-run experimental setup:

- **Run 1 – DQN Baseline**
- **Run 2 – DDQN + Dueling DQN**
- **Run 3 – Final tuned run**  
  (same architecture as baseline, but with a modified learning rate and updated training configuration)

Each run includes:

- A **training curve PNG** in `figures/`
- A **saved model `.dat` file** in `models/`
- Hyperparameter notes in `tuning_log.md`
- Colab notebook with full training code in `notebooks/`

---

## **Repository Structure**

```text
models/
    pong_baseline/
        ALE_Pong-v5-baseline_best_-19-20251124-0055.dat

    pong_run2/
        ALE_Pong-v5-best_-19-20251124-0034-test_epsdec150000_rs10000_sync1000.dat

    pong_final/
        ALE_Pong-v5-baseline_best_-19-20251124-0147.dat

figures/
    pong_baseline/
        curve_dqn_baseline.png

    pong_run2/
        curve_pong_ddqn_dueling.png

    pong_final/
        curve_pong_final.png

notebooks/
    pong_pong_experiments.ipynb

videos/
    Early / Random Behavior:
    https://github.com/gsoraw/csci166-dqn-pong/blob/main/videos/pong_random_behavior.mp4

    Later / Trained Behavior:
    https://github.com/gsoraw/csci166-dqn-pong/blob/main/videos/pong_trained_behavior.mp4

tuning_log.md  
README.md
