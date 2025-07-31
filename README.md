## Question:
You can implement ANY GAME OF YOUR CHOICE, either in Python or another programming language of your choice as well. Within this game, your goal is to develop a learning agent utilising Double DQN and another agent utilising Duelling DQN, both of them gaining proficiency in the game through experimentation, making moves, and obtaining rewards or penalties based on whether those moves result in a victory, defeat, or tie. 

You are permitted to utilise standard libraries like T ensorFlow, Keras, pandas, numpy, and similar tools. To be clear and precise your code should have the following components: Establishing the ecosystem/environment, Outlining the gameplay, Constructing the Double DQN AND Duelling DQN reinforcement learning framework, Conducting model training, Evaluating the model and providing a comparison between the two.










# 🎮 Double DQN & Dueling DQN Reinforcement Learning Agents (CartPole-v1)

This repository implements and compares **Double DQN** and **Dueling DQN** architectures on the classic **CartPole-v1** environment using **TensorFlow 2.x** and **OpenAI Gym**. The goal is to balance a pole on a moving cart by learning optimal actions through trial and error using reinforcement learning.

![Double DQN Training](DoubleDQN_selected_episodes_training.mp4)
![Dueling DQN Training](DuelingDQN_selected_episodes_training.mp4)

---

## 🧰 Features

- ✅ TensorFlow-based implementation of Double DQN and Dueling DQN
- 🎓 Full training pipeline with experience replay and target network
- 🔄 Epsilon-greedy strategy for exploration
- 📉 Live reward tracking with matplotlib
- 🎥 Frame capture for generating training videos
- 🧪 Easy switching between agent types (`DoubleDQN` vs `DuelingDQN`)

---

## 🧠 Concepts Covered

- Q-Learning
- Deep Q-Network (DQN)
- Double Q-Learning
- Dueling architecture for value and advantage separation
- Experience Replay Buffer
- Target Network updates

---

## 🚀 How to Run

### 📦 Requirements

```bash
pip install gym tensorflow matplotlib numpy pillow
```
## 🏁 Train Agent
The training is built into a single Jupyter Notebook. Just run all cells.
```bash
jupyter notebook Double_DQN_AND_Duelling_DQN_reinforcement_learning_learning_agent_Framework.ipynb
```
Choose which agent to train by modifying:
```bash
agent = DoubleDQN(num_actions)   # or DuelingDQN(num_actions)
```
## 🎥 Video Recording
The agent collects frames using env.render(mode='rgb_array') and converts them to GIF or MP4 for analysis.
## 📊 Training Parameters
| Parameter           | Value     |
| ------------------- | --------- |
| Episodes            | 150       |
| Batch Size          | 32        |
| Gamma (Discount)    | 0.99      |
| Replay Buffer Size  | 10,000    |
| Minimum Replay Size | 1,000     |
| Epsilon Decay       | 0.995     |
| Target Update Freq  | 100 steps |
| Learning Rate       | 0.001     |

## 📈 Sample Results
- Double DQN shows smoother and more stable learning curves

- Dueling DQN learns faster in early episodes due to its architectural separation of value and advantage
## 🔮 Future Improvements
- Add Prioritized Experience Replay (PER)

- Extend to more complex environments (e.g., Atari games)

- Incorporate Noisy Networks or Rainbow DQN variants

- Save/load models for continued training
## 📁 Repository Structure
```bash
.
├── Double_DQN_AND_Duelling_DQN_reinforcement_learning_learning_agent_Framework.ipynb
├── DoubleDQN_selected_episodes_training.mp4
├── DuelingDQN_selected_episodes_training.mp4
└── README.md
```
## 🤝 Acknowledgments
- OpenAI Gym for the environment

- TensorFlow for model development

- DeepMind for the DQN architecture concepts
```bash

</details>

---

### 📦 `requirements.txt`

```txt
gym
tensorflow
matplotlib
numpy
pillow
```
🚫 .gitignore
```bash
__pycache__/
.ipynb_checkpoints/
*.pyc
*.pyo
*.pyd
.env
*.DS_Store
```
## Author
- Manjul Mayank

