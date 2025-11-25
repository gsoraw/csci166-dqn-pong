# csci166-dqn-pong
Deep Q-Learning Atari Pong project for CSCI 166

This repository contains my implementation and experiments with Deep Q-Learning on the Atari game **Pong**, using the **ALE/Pong-v5** environment from Gymnasium and **PyTorch** in Google Colab.

The project follows a three-run experimental setup:

1. **Run 1 – DQN Baseline**  
2. **Run 2 – DDQN + Dueling DQN**  
3. **Run 3 – Final tuned run** (same architecture as baseline, with a modified learning rate and training configuration)

Each run has:

- A **training curve PNG** in `figures/`
- A **saved model `.dat` file** in `models/`
- Hyperparameter notes in `tuning_log.md`
- Training code and outputs in a Colab notebook under `notebooks/`

---

## Repository Structure

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
    pong_pong_experiments.ipynb     ← exported Colab notebook (name may vary)

videos/
    Early / Random Behavior:
    https://github.com/gsoraw/csci166-dqn-pong/blob/main/videos/pong_random_behavior.mp4
    Later / Trained Behavior:
    https://github.com/gsoraw/csci166-dqn-pong/blob/main/videos/pong_trained_behavior.mp4
tuning_log.md
README.md
