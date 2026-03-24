# 🐦 Flappy Bird DQN (Deep Q-Learning)

A Reinforcement Learning project where an agent learns to play Flappy Bird using **Deep Q-Network (DQN)** with PyTorch and Gymnasium.

---

## 🚀 Project Overview

This project implements a **Deep Q-Learning agent** to solve the Flappy Bird environment from `flappy_bird_gymnasium`.

The agent learns optimal actions (flap or not) by interacting with the environment and maximizing cumulative reward.

---

## 🧠 Key Concepts Used

* Deep Q-Network (DQN)
* Experience Replay
* Target Network
* Epsilon-Greedy Exploration
* Reward Optimization

---

## 🛠️ Tech Stack

* Python 🐍
* PyTorch 🔥
* Gymnasium 🎮
* Pygame 🎨

---

## 📁 Project Structure

```
FLAPPYBIRD_RL/
│── agent.py                # Main training & testing script
│── dqn.py                  # Neural network model
│── experience_replay.py    # Replay buffer implementation
│── parameters.yaml         # Hyperparameters
│── runs/                   # Saved models & logs
│── README.md               # Project documentation
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/FlappyBird-DQN.git
cd FlappyBird-DQN
```

### 2. Install dependencies

```bash
pip install torch gymnasium pygame flappy-bird-gymnasium pyyaml
```

---

## ▶️ How to Run

### 🔹 Train the model

```bash
python agent.py default --train
```

### 🔹 Test (Play using trained model)

```bash
python agent.py default
```

---

## 💾 Model Saving

* Best model is saved as `.pt` file in `runs/`
* Logs are stored in `.log` files

---

## 📊 How it Works

1. Agent observes current state
2. Chooses action using epsilon-greedy policy
3. Stores experience in replay memory
4. Samples mini-batch for training
5. Updates Q-values using Bellman equation
6. Syncs target network periodically

---

## 🧪 Hyperparameters

Configured via `parameters.yaml`:

* Learning Rate (`alpha`)
* Discount Factor (`gamma`)
* Epsilon decay strategy
* Replay memory size
* Batch size

---

## 🎯 Features

* Stable training using target network
* Efficient learning with experience replay
* GPU/CPU/MPS support
* Logging and model checkpointing

---

## ⚠️ Notes

* Ensure `pygame` is properly initialized for rendering
* `.pt` files are excluded via `.gitignore`

---

## 📈 Future Improvements

* Double DQN
* Dueling DQN
* Prioritized Experience Replay
* Reward shaping
* Visualization of training performance

---

## 🤝 Contributing

Feel free to fork this repo and improve the model or add new features.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

**Dinesh Kumar**

---

⭐ If you found this useful, give it a star!
