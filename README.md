Sure! Here's an enhanced version of your `README.md` that is more professional, engaging, and designed to attract attention to your GitHub repository. This version includes a clear structure, visual elements, badges, and additional sections to make your project stand out.

---

# 🎮 Super Mario with Deep Q-Learning 🤖

![Super Mario AI](https://i.pinimg.com/originals/63/dd/d7/63ddd7f601b6c9961e83fc5f45bd67f5.gif)

Welcome to **Super Mario with Deep Q-Learning**, a project where artificial intelligence meets classic gaming! This repository showcases how to train an AI agent to master Super Mario using Deep Q-Learning (DQL). By leveraging deep neural networks, our agent learns to navigate the iconic game environment from raw pixel data.

---


## 🚀 Table of Contents

- [🌟 Overview](#-overview)
- [✨ Features](#-features)
- [🛠 Installation](#-installation)
- [🎬 Usage](#-usage)
  - [🏋️‍♂️ Training](#-training)
  - [🧪 Testing](#-testing)
  - [🎥 Demo Video](#-demo-video)
- [📈 Results](#-results)
- [🏗 Architecture](#-architecture)
- [📝 License](#-license)
- [📚 References](#-references)

---

##  Overview

This project demonstrates the application of **Deep Q-Learning** to train an AI agent capable of playing Super Mario. DQL combines the principles of Q-Learning with deep neural networks, enabling the agent to learn optimal strategies for complex games by interpreting raw pixel inputs.

### Key Components

- **Environment Preprocessing**: Enhances the game environment with frame skipping, resizing, grayscale conversion, normalization, and frame stacking for efficient learning.
- **Convolutional Neural Network (CNN) Model**: Processes game frames to extract meaningful features for decision-making.
- **DQN Agent**: Learns to interact with the environment through experience replay and stabilizes learning with a target network.

---

##  Features

- **Real-time Gameplay**: Watch the AI play Super Mario in real-time.
- **Customizable Training Parameters**: Adjust the number of episodes, learning rates, and other hyperparameters.
- **Visualizations**: Track training progress and rewards with interactive Plotly graphs.
- **Modular Codebase**: Easily extend or modify components for further research.

---

##  Installation

Ensure you have Python installed. Then, install the required packages:

```bash
pip install gym-super-mario-bros==7.4.0
pip install gym==0.26.2
pip install nes-py==8.2.1
pip install tensordict
pip install torchrl
pip install gym[accept-rom-license]  # Adjust if needed
```

> **Note**: Some packages may require additional system dependencies. Please refer to their respective documentation for more details.

---

## 🎬 Usage

### 🏋️‍♂️ Training

Train the DQN agent by running the Jupyter notebook:

```python
history = train(agent, env, num_episodes=7000, ckpt_save_interval=500, log=True)
```

### 🧪 Testing

Evaluate the trained agent with:

```python
test('model_mario_6500.pt', num_episodes=1, epsilon=0.02)
```

### 🎥 Demo Video

Watch the AI in action:

![Mario Bros Gameplay](super_mario.gif)

For a full video demonstration, check out [this link](#) *(Add actual link if available)*.

---

## 📈 Results

Monitor the training progress and performance:

- **Average Rewards**: Visualized using Plotly to show the agent's performance over episodes.

![Training Rewards](rewards.png)

---

## 🏗 Architecture

### Environment Preprocessing

- **Frame Skipping**: Reduces computational load by skipping frames.
- **Resizing & Grayscale**: Simplifies input data.
- **Normalization**: Scales pixel values for efficient learning.
- **Frame Stacking**: Provides temporal context to the agent.

### CNN Model

A deep convolutional neural network processes the preprocessed frames to extract features that inform the agent's actions.

### DQN Agent

Implements the core Deep Q-Learning algorithm, utilizing experience replay and a target network to stabilize and enhance learning.

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).


---

## 📚 References

- [Deep Q-Learning Explained](https://blog.damavis.com/aprendizaje-por-refuerzo-profundo-dqn/)
- [NES-PY Documentation](https://github.com/Kautenja/nes-py)

---

