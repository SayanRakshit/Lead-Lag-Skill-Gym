# Lead–Lag Skill Gym

A reinforcement-learning framework for adaptive lead–lag discovery in time-series data.

## Overview

The framework combines **9 statistical experts, Mamba, Mixture of Experts (MoE), and Actor–Critic PPO** to predict directional relationships and time delays between two time series.

## Key Features

- Synthetic data generation across 9 families (F1–F9).
- Nine statistical experts with four-class probability calibration.
- Mamba encoder and MoE-based expert weighting.
- **12 RL actions:** 9 expert selections, Extend, Transform, and Declare.
- PPO training with cost-aware rewards.
- Regret-guided adversarial curriculum learning.
- Evaluation of accuracy, NLL, lag error, and computational cost.

## How to Run

1. Open `LeadLag_Skill_Gym.ipynb` in Google Colab.
2. Enable GPU acceleration.
3. Mount Google Drive.
4. Run all cells sequentially.

Models and results are saved to:

`MyDrive/Gym/skill_gym_full/`

## Preliminary Results

| Metric | PPO |
|---|---:|
| Balanced Accuracy | 66.88% |
| NLL | 0.9608 |
| Average Experts | 1.41 |
| Average Extend Actions | 1.89 |
