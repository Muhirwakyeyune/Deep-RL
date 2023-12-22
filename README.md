# Intelligent Traffic Light Control Using Deep Reinforcement Learning

## Authors
- Khady Gaye
- Mame Diarra Diouf
- Honorine Gnonfin
- Mame Diarra Diop
- Salomon Muhirwa

## Date
September 29, 2023

## 1. Introduction

Transportation is an essential aspect of our daily lives. Traffic congestion, especially at intersections, poses significant challenges. Traditional traffic light systems operate deterministically, with predefined durations for each color. This approach may not be optimal, considering varying traffic flows. This project explores Intelligent Traffic Light Control using Deep Reinforcement Learning (DRL) with a focus on Deep Q-Network (DQN) and Double Deep Q-Network (DDQN).

## 2. Related Works

Various approaches exist for traffic light control, including classic optimization, evolutionary algorithms, and fuzzy logic. Deep Reinforcement Learning (DRL) has gained attention for optimizing traffic light control. DRL utilizes neural networks and reinforcement learning algorithms to adaptively learn and optimize traffic signal timings based on real-time conditions.

## 3. Methodology

### 3.1 Environment

The project focuses on a single intersection with two unidirectional traffic flows. The environment's state includes the number of vehicles on each road and the light configuration (red or green). Actions involve changing the light state, and the agent receives rewards based on the number of waiting vehicles.

### 3.2 Deep Q-Network

DQN is explored to optimize traffic light control policies in real-time. The algorithm uses a neural network to estimate the action-value function, and experience replay is employed to update network parameters.

### 3.3 Double Deep Q-Network

DDQN aims to reduce overestimation by decomposing the max operation in the target into action selection and evaluation. The weights of the second network are replaced with the weights of the target network for evaluation.

## 4. Results and Discussion

DQN implementation involves a two-hidden-layer neural network with ReLu activation. The reward evolution over 10,000 episodes is presented, and the model is evaluated on 1,000 episodes. DDQN results are also discussed. Challenges and potential improvements are outlined.

## 5. Conclusion

The project explores the potential of DQN and DDQN algorithms for optimizing traffic light control policies in a simplified intersection environment. Challenges and areas for further exploration are identified.

## 6. References

[1] Micha Hofri and Keith W Ross. On the optimal control of two queues with server setup times and its analysis. SIAM Journal on computing, 16(2):399–420, 1987.

[2] Peter Koonce and Lee Rodegerdts. Traffic signal timing manual. Technical report, United States. Federal Highway Administration, 2008.

[3] Xiaoyuan Liang, Xunsheng Du, Guiling Wang, and Zhu Han. A deep reinforcement learning network for traffic light cycle control. IEEE Transactions on Vehicular Technology, 68(2):1243–1253, 2019.

[4] Wei-Hua Lin and Chenghong Wang. An enhanced 0-1 mixed-integer lp formulation for traffic signal control. IEEE Transactions on Intelligent transportation systems, 5(4):238–245, 2004.

[5] Xiao-Yang Liu, Ming Zhu, Sem Borst, and Anwar Walid. Deep reinforcement learning for traffic light control in intelligent transportation systems. arXiv preprint arXiv:2302.03669, 2023.

[6] Hua Wei, Guanjie Zheng, Huaxiu Yao, and Zhenhui Li. Intellilight: A reinforcement learning approach for intelligent traffic light control. In Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pages 2496–2505, 2018.
