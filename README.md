<<<<<<< HEAD
# Training Super Mario game playing agent using Action-Value apprioximation and Policy Apprioximation and Performance Comparision.

<p align='center'>
    <img src="/Analysis/Plots/PPO.gif" alt="drawing" width="800"/>
</p>


=======
# Performance Comparison of Reinforcement Learning Algorithms in Super Mario Bros: DQN, DDQN, and PPO
>>>>>>> 2fdafd71391e9ced254b25d67e9c93aec4da33d2
This repository contains jupyter notebooks for training and analysing the performance of a game-playing agents trained to complete one level of Super Mario Bros. As the state-action sapce is enoromous, the agents are trained using two algorithms using action value approximation - Deep-Q-Network, Double Deep Q-Networks - and one using policy approximation - Proximal Policy Approximation.

The notebooks use Pytorch Framework for training and analyzing the Reinforcement learning algorithms.

## Results 

### Training 

The following plots highlight the discounted and undiscounted rewards obtained by the agent while training

#### Undiscounted returns vs Episodes
<p align='center'>
    <img src="/Analysis/Plots/undisc_returns.png" alt="drawing" width="600"/>
</p>

#### Discounted returns vs Episodes
<p align='center'>
    <img src="/Analysis/Plots/disc_returns.png" alt="drawing" width="600"/>
</p>


### Testing

The models obtained after training were used to play the same level for 100 episodes. The table summarizes the results.

| Metric/RL algorithm                     |    DQN  |  DDQN  |   PPO   |  
| :--------------------------------------:|:-------:|:------:|:-------:|
| **Average Discounted returns**          | 708.34  | 704.51 | 853.24  |
| **Average number of steps per episode** | 537.58  | 549.49 | 342.07  |
| **Success rate**                        | 430     | 424    | 720     |

#### Discounted returns vs Episodes
<p align='center'>
    <img src="/Analysis/Plots/retvsep_test.png" alt="drawing" width="600"/>
</p>

#### Number of steps/episode vs Episodes
<p align='center'>
    <img src="/Analysis/Plots/stepvsep_test.png" alt="drawing" width="600"/>
</p>

#Simulation

The DDQN and PPO models were simulated with the same parameters used while training. The simulation results are shown below.

<p align='center'>
    <img src="/Analysis/Plots/DDQN.gif" alt="drawing" width="800"/>
</p>

<p align='center'>
    <img src="/Analysis/Plots/PPO.gif" alt="drawing" width="800"/>
</p>
