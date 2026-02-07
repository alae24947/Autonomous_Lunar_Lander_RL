# Lunar Lander RL Algorithm Comparison

Comparing **Q-Learning**, **DQN**, and **PPO** on OpenAI Gym's LunarLander-v3 environment.

![Comparison Demo](results/coparaison_demo.mp4)

## Results

| Algorithm  | Avg Score | Success Rate | Training Time |
|------------|-----------|--------------|---------------|
| Q-Learning | 185       | 72%          | 2.1 hrs       |
| DQN        | 229       | 85%          | 2.8 hrs       |
| **PPO**    | **245**   | **91%**      | **1.5 hrs**   |

**Winner: PPO** - Best performance with fastest training

[Full Comparison Video](https://youtu.be/7o4nDNbENxs)

[website](https://astorius761.github.io/Astorius)

[detailed report about the models]
(file:///C:/Users/LENOVO/Downloads/Autonomous_Lunar_Lander_RL/documents/RIENF_LEARN_ROCKET_PFE_L3.pdf)

---

## Algorithm Demos

### Q-Learning
![Q-Learning](results/QLearning_results.mp4)
- Vision-based tabular method
- 84×84 grid discretization

### DQN
![DQN](results/Dqn_results.mp4)
- CNN + experience replay
- Frame stacking (4 frames)

### PPO
![PPO](results/PPO_results.mp4)
- Actor-Critic architecture
- Policy gradient method

---

## Tech Stack
Python • PyTorch • OpenAI Gym • OpenCV

## Run It
```bash
pip install -r requirements.txt
python run_ppo.py --render
```

## final results 
PPO achieved the best results due to stable policy updates and sample efficiency. Q Learning struggled with visual state space complexity, while DQN showed improvement but required more hyperparameter tuning.
