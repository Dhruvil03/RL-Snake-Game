# 🐍 RL-Snake-Game

An AI-powered Reinforcement Learning based twist on the classic Snake game! This project uses **Deep Q-Learning (DQN)** and **PyTorch** to train an autonomous agent to learn how to play Snake — all without human intervention.

## 🚀 Features

- 🎮 Autonomous Snake Agent with reinforcement learning  
- 🧠 Deep Neural Network trained using DQN  
- 📈 Real-time score plotting to monitor performance  
- 🔁 Experience replay and epsilon-greedy strategy  

## 📂 Project Structure

- `agent.py` – Training loop & DQN agent logic  
- `game.py` – Pygame-based Snake environment  
- `model.py` – Neural network (Q-Network) & training logic  
- `helper.py` – Score plotting utility  
- `arial.ttf` – Font file for game UI  

## 🧠 How It Works

### 🧾 State Representation
- Obstacle danger (straight, right, left)  
- Movement direction (up, down, left, right)  
- Relative food position  

### 🎮 Action Space
- Move straight  
- Turn right  
- Turn left  

### 🏆 Rewards
- `+10` for eating food  
- `-10` for hitting a wall or itself  
- `0` for surviving a step  

### 🧪 Training Strategy
- Short-term memory: train after every move  
- Long-term memory: replay experiences from previous games  
- Epsilon-greedy exploration: balances exploration and exploitation  

## 📊 Live Training Visualization
Live plotting of scores and average scores to monitor agent performance throughout training.


## 🛠️ Getting Started

### 📦 Prerequisites
```bash
pip install torch torchvision pygame matplotlib ipython
