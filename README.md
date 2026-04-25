# Autonomous Driving Decision Simulator

This is a browser-based simulator for probabilistic decision making in autonomous driving.  
Given the current vehicle state, lane information, and obstacles ahead, the simulator computes a probability distribution and expected value (EV) for each possible action, then selects one action such as going straight, decelerating, changing lanes, or performing an emergency stop.

## Overview

The main goal of this project is not just to show the final behavior of an autonomous vehicle, but to **visualize the internal decision-making process**:

- Generate candidate actions
- Evaluate each action with a probability and expected value
- Select the most reasonable action based on risk and reward
- Log and visualize the result over time

On the simulation screen you can monitor:

- Current speed, lane, and obstacle status
- Probability distribution for each action
- Expected value (EV) for each action
- Selected action at each decision step
- Cumulative statistics (distance, obstacle avoidance, lane changes, risky events)
- Decision logs

## Key Features

- Probabilistic decision-making simulation
- Expected value (EV) calculation for each action
- Intuitive web-based visualization
- Cumulative statistics and decision logs
- Start / reset controls and simulation speed control

## Decision Flow

1. Read the current vehicle state (speed, lane) and environment (obstacle ahead).
2. Generate candidate actions:
   - Go straight
   - Decelerate
   - Change lane (left / right)
   - Emergency stop
3. For each action, estimate its risk and reward, then compute:
   - Probability of choosing the action
   - Expected value based on the situation
4. Select the most reasonable action according to the EV and probability.
5. Update the vehicle state, statistics, and logs on the UI.
6. Repeat the process to simulate the autonomous driving decision loop.

## Tech Stack

- HTML
- CSS
- JavaScript

## What I Learned

- How to design and implement state-based decision logic in a simulation environment
- How to use probability distributions and expected values for action selection
- How to visualize internal decision processes in a browser UI
- How to record and interpret logs and statistics for analysis

## Future Work

- Add more diverse road environments and events
- Improve the reward / risk functions for each action
- Compare rule-based decision making with reinforcement learning or optimization-based methods
- Add scenario-based performance metrics and analysis tools

## How to Run

1. Clone this repository.
2. Open `autonomous-driving-simulator.html` in a modern web browser.
3. Click **Start** to begin the simulation, and use the controls to adjust the speed or reset the environment.

---

## Japanese Summary / 日本語概要

このプロジェクトは、自動運転車の意思決定プロセスをシミュレーションするための Web ベースのツールです。  
車両の現在状態（速度・車線）や前方障害物の有無に応じて、直進、減速、車線変更、急停止などの行動候補ごとに確率分布と期待値を計算し、最も合理的な行動を選択します。

### 特徴

- 行動候補ごとの確率分布と期待値（EV）の計算
- 行動選択プロセスの可視化（現在状態・選択された行動・ログなど）
- 走行距離、障害물 회피回数、車線変更回数、危険イベント数などの統計表示
- シミュレーションの開始・初期化・速度調整機能

### 使用技術

- HTML
- CSS
- JavaScript

このシミュレータを通じて、「自動運転車がどのように状況を判断し、どのような基準で行動を選択するのか」を、直感的に理解できるように設計しました。

## Author

Ajou University Software Student / Portfolio Project
