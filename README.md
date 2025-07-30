# 🐍 Automated Snake Game – Deep Q-Learning

This project implements an **AI agent that learns to play the classic Snake game** using **Deep Q-Learning (DQN)**.  
The agent is trained using **reinforcement learning**, where it learns optimal moves to maximize the score by eating food and avoiding collisions.

---

## 🚀 Features

- ✅ Classic Snake game implemented with **Pygame**  
- ✅ AI agent trained via **Deep Q-Network (DQN)**  
- ✅ Uses **Replay Memory** for stable learning  
- ✅ Implements **epsilon-greedy strategy** for exploration vs exploitation  
- ✅ Real-time visualization of training scores with Matplotlib  
- ✅ Neural network with **PyTorch** for Q-value prediction  

---

## 🛠️ Tech Stack

- **Python**
- **PyTorch** – Neural network for Q-learning  
- **Pygame** – Game environment  
- **Matplotlib** – Real-time training plot  

---

## 📂 Project Structure

```

Automated Snake Game/
│── agent.py       # AI agent with training loop
│── game.py        # Snake game environment
│── helper.py      # Live plotting of training scores
│── model.py       # Neural network (DQN) and Q-learning trainer
│── model/         # Saved trained models
│── README.md

````

---

## 🧠 How It Works

1. **State Representation** – The agent observes the game state (dangers, direction, and food location).  
2. **Action Space** – Three possible actions: `[straight, right, left]`.  
3. **Reward System** –  
   - `+10` for eating food  
   - `-10` for collision or dying  
   - `0` for regular moves  
4. **Neural Network** – A simple feed-forward network that predicts Q-values for each action.  
5. **Deep Q-Learning** –  
   - Experience replay with a replay memory  
   - Bellman equation to update Q-values  
   - Discount factor `gamma` for future rewards  
6. **Training Loop** – The agent plays games, learns from experience, and improves over time.  

---

## 📊 Training Visualization

During training, a live plot shows:

- **Game Score** – The score achieved in each game  
- **Mean Score** – Average score across games  

---

## ▶️ Running the Project

### 1️⃣ Clone the repository:
```bash
git clone https://github.com/MohammedPathariya/Automated-Sname-Game.git
cd Automated-Sname-Game
````

### 2️⃣ Install dependencies:

```bash
pip install torch pygame matplotlib numpy
```

### 3️⃣ Run the training:

```bash
python agent.py
```

### 4️⃣ Watch the AI play:

* The game window will show the snake’s movement
* The agent learns gradually and improves with more games

---

## 📈 Example Training Output:

```
Game 10   Score: 2   Record: 3
Game 50   Score: 10  Record: 12
Game 100  Score: 20  Record: 25
...
```

---

## 🔮 Future Enhancements

* Add a **GUI toggle** for human vs AI gameplay
* Implement **Double DQN** or **Dueling DQN** for improved learning
* Deploy a pre-trained model to play directly without retraining
* Hyperparameter tuning for better performance

---

## 📜 License

MIT License © 2025

---

## 🙌 Acknowledgments

* Inspired by reinforcement learning tutorials and Snake game implementations
* Built with PyTorch and Pygame

---
