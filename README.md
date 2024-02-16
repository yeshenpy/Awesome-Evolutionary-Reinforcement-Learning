
# ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)  Awesome-Evolutionary-Reinforcement-Learning
Evolutionary Reinforcement Learning (ERL), which integrates Evolutionary Algorithms (EAs) and Reinforcement Learning (RL) for optimization, has demonstrated remarkable performance advancements. By fusing the strengths of both approaches, ERL has emerged as a promising research direction. 


[![](https://img.shields.io/badge/-Update%20List-orange)]()

**This repository is under construction ...**

**23 January 2024**: Our survey paper has been updated on arXiv. Arxiv: **[Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey](http://arxiv.org/abs/2401.11963)**  **This survey is now categorized to better align with the conventions of researchers in different fields, providing a quicker and more accessible introduction for researchers.** 

**20 January 2024**: I am updating the survey on this topic and will fully update the site when the survey is updated.

***

We provide three main research directions with various branches as follows: **(In total, it includes approximately 90 works.)**

- [ :star: EA-Assisted Optimization of RL](#ea-assisted-optimization-of-rl)
  - [EA-assisted Parameter Search](#ea-assisted-parameter-search)
  - [EA-assisted Action Selection](#ea-assisted-action-selection)
  - [Hyperparameter Optimization](#hyperparameter-optimization)
  - [Others](#others)
- [ :star: RL-Assisted Optimization of EA](#rl-assisted-optimization-of-ea)
  - [Population Initialization](#population-initialization)
  - [Population Evaluation](#population-evaluation)
  - [Variation Operator](#variation-operator)
  - [Dynamic Operator Selection](#dynamic-operator-selection)
  - [Hyperparameter Configuration](#hyperparameter-configuration)
  - [Others](#others-1)
- [ :star: Synergistic Optimization of EA and RL](#synergistic-optimization-of-ea-and-rl)
  - [Single-Agent Optimization](#single-agent-optimization)
  - [Multi-Agent Optimization](#multi-agent-optimization)
  - [Others](#others-2)

![image](https://github.com/yeshenpy/Awesome-Evolutionary-Reinforcement-Learning/assets/43668853/fc550484-e9ef-4e14-9800-88a7355dcfc2)

![image](https://github.com/yeshenpy/Awesome-Evolutionary-Reinforcement-Learning/assets/43668853/96464ff7-db92-4cc8-bc3d-ad2edc76695e)


Detailed information can be found in our survey paper.


---

[![](https://img.shields.io/badge/-Comment-red.svg)]()

* **If you want to get started, I recommend referring to the *Accepted Papers with the Released Code*, as it provides an easy way to explore research papers and their associated code implementations. 
Furthermore, building your algorithm on top of state-of-the-art algorithms will greatly enhance your productivity and efficiency.**



* If you are interested in sequential decision-making problems, it is recommended to focus primarily on **EA-Assisted Optimization of RL** and **Synergistic Optimization of EA and RL**. If you are interested in other optimization problems, it is suggested to pay attention to **RL-Assisted Optimization of EA**. I primarily focus on the former.

---


## Paper With Code [TODO]

# :star: EA-Assisted Optimization of RL
## EA-assisted Parameter Search

**ELIFE 2020** Reinforcement Learning beyond The Bellman Equation: Exploring Critic Objectives using Evolution

[https://direct.mit.edu/isal/proceedings/isal2020/32/441/98464](https://direct.mit.edu/isal/proceedings/isal2020/32/441/98464) Code: [https://github.com/ajleite/RLBeyondBellman](https://github.com/ajleite/RLBeyondBellman)

**ICLR 2021** Genetic Soft Updates for Policy Evolution in Deep Reinforcement Learning

OpenReview: [https://openreview.net/forum?id=TGFO0DbD_pk](https://openreview.net/forum?id=TGFO0DbD_pk) Code: Not Found

**ICLR 2023** Improving Deep Policy Gradients with Value Function Search

OpenReview: [https://openreview.net/forum?id=6qZC7pfenQm](https://openreview.net/forum?id=6qZC7pfenQm) Code: Not Found

## EA-assisted Action Selection

**CORL 2018**  Scalable deep reinforcement learning for vision-based robotic manipulation

Link: [https://proceedings.mlr.press/v87/kalashnikov18a](https://proceedings.mlr.press/v87/kalashnikov18a) Code: [https://github.com/quantumiracle/QT_Opt](https://github.com/quantumiracle/QT_Opt)

**ICML 2019 RL4RealLife Workshop** Q-learning for continuous actions with cross-entropy guided policies

Link: [https://arxiv.org/abs/1903.10605](https://arxiv.org/abs/1903.10605)  Code: Not Found

**Preprint 2022** Evolutionary Action Selection for Gradient-based Policy Learning

Link [https://arxiv.org/abs/2201.04286](https://arxiv.org/abs/2201.04286)  Code: Not Found

**Preprint 2021**  Soft Actor-Critic with Cross-entropy Policy Optimization

Link: [https://arxiv.org/abs/2112.11115](https://arxiv.org/abs/2112.11115) Code: [https://github.com/wcgcyx/SAC-CEPO](https://github.com/wcgcyx/SAC-CEPO)

**CORL 2021** GRAC: Self-guided and Self-regularized Actor-critic

Link: [https://arxiv.org/abs/2009.08973](https://arxiv.org/abs/2009.08973) Code: [https://github.com/stanford-iprl-lab/GRAC](https://github.com/stanford-iprl-lab/GRAC)

**ICML 2022**  Plan better amid conservatism: Offline multi-agent reinforcement learning with actor rectification

Link: [https://arxiv.org/abs/2111.11188](https://arxiv.org/abs/2111.11188)  Code: [https://github.com/ling-pan/OMAR](https://github.com/ling-pan/OMAR)

**Preprint 2020** Deep Multi-agent Reinforcement Learning for Decentralized Continuous Cooperative Control

Link: [https://beipeng.github.io/files/2003.06709.pdf](https://beipeng.github.io/files/2003.06709.pdf)  Code: [https://github.com/oxwhirl/comix](https://github.com/oxwhirl/comix)


## Hyperparameter Optimization


## Others


# :star: RL-Assisted Optimization of EA
## Population Initialization


## Population Evaluation

**ICLR 2023** ERL-Re2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation 

Arxiv: [https://arxiv.org/abs/2210.17375](https://arxiv.org/abs/2210.17375) Code: [https://github.com/yeshenpy/ERL-Re2](https://github.com/yeshenpy/ERL-Re2)

**ELSEVIER Information Sciences** A Surrogate-Assisted Controller for Expensive Evolutionary Reinforcement Learning

Arxiv: [https://arxiv.org/abs/2201.00129](https://arxiv.org/abs/2201.00129) Code: Not Found

**ICLR 2021 submission** PGPS: Coupling Policy Gradient with Population-based Search

OpenReview: [https://openreview.net/forum?id=PeT5p3ocagr](https://openreview.net/forum?id=PeT5p3ocagr) Code: [https://github.com/NamKim88/PGPS/blob/master/Main.py](https://github.com/NamKim88/PGPS/blob/master/Main.py)


## Variation Operator

**ICLR 2023** Neuroevolution is a Competitive Alternative to Reinforcement Learning for Skill Discovery

Link: [https://openreview.net/forum?id=6BHlZgyPOZY](https://openreview.net/forum?id=6BHlZgyPOZY) Code: [https://github.com/instadeepai/qd-skill-discovery-benchmark](https://github.com/instadeepai/qd-skill-discovery-benchmark)

**GECCO 2022** Approximating Gradients for Differentiable Quality Diversity in Reinforcement Learning

Link: [https://arxiv.org/pdf/2202.03666.pdf](https://arxiv.org/pdf/2202.03666.pdf) Code: [https://github.com/icaros-usc/dqd-rl](https://github.com/icaros-usc/dqd-rl)

**Preprint 2022** QD-RL: Efficient Mixing of Quality and Diversity in Reinforcement Learning

Link：[https://arxiv.org/abs/2006.08505v2](https://arxiv.org/abs/2006.08505v2) Code: Not Found

**ICLR 2021 submission** PGPS: Coupling Policy Gradient with Population-based Search

OpenReview: [https://openreview.net/forum?id=PeT5p3ocagr](https://openreview.net/forum?id=PeT5p3ocagr) Code: [https://github.com/NamKim88/PGPS/blob/master/Main.py](https://github.com/NamKim88/PGPS/blob/master/Main.py)

**ICLR 2019** CEM-RL: Combining evolutionary and gradient-based methods for policy search

Arxiv: [https://arxiv.org/abs/1810.01222](https://arxiv.org/abs/1810.01222) Code: [https://github.com/apourchot/CEM-RL](https://github.com/apourchot/CEM-RL)

## Dynamic Operator Selection

## Hyperparameter Configuration

## Others

# :star: Synergistic Optimization of EA and RL
## Single-Agent Optimization


**ICLR 2023** ERL-Re2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation 

Arxiv: [https://arxiv.org/abs/2210.17375](https://arxiv.org/abs/2210.17375) Code: [https://github.com/yeshenpy/ERL-Re2](https://github.com/yeshenpy/ERL-Re2)

**AAMAS 2022** Off-policy evolutionary reinforcement learning with maximum mutations (Maximum Mutation Reinforcement Learning for Scalable Control)

Link: [https://nbviewer.org/github/karush17/karush17.github.io/blob/master/_pages/temp4.pdf](https://nbviewer.org/github/karush17/karush17.github.io/blob/master/_pages/temp4.pdf) Code: [https://github.com/karush17/esac](https://github.com/karush17/esac)

**ELSEVIER Information Sciences** A Surrogate-Assisted Controller for Expensive Evolutionary Reinforcement Learning

Arxiv: [https://arxiv.org/abs/2201.00129](https://arxiv.org/abs/2201.00129) Code: Not Found

**Preprint** Evolutionary action selection for gradient-based policy learning

Arxiv: [https://arxiv.org/abs/2201.04286v1](https://arxiv.org/abs/2201.04286v1) Code: Not Found


**NeurIPS 2020** Competitive and cooperative heterogeneous deep reinforcement learning

Arxiv: [https://arxiv.org/abs/2011.00791](https://arxiv.org/abs/2011.00791) Code: Not Found


**AMMAS** Guiding Evolutionary Strategies with Off-Policy Actor-Critic

Link: [https://dl.acm.org/doi/10.5555/3463952.3464104](https://dl.acm.org/doi/10.5555/3463952.3464104) Code: Not Found

**AAAI 2020** PDERL: Proximal Distilled Evolutionary Reinforcement Learning

Arxiv: [https://arxiv.org/abs/1906.09807](https://arxiv.org/abs/1906.09807) Code: [https://github.com/crisbodnar/pderl](https://github.com/crisbodnar/pderl)

**LOD 2020** Gradient Bias to Solve the Generalization Limit of Genetic Algorithms Through Hybridization with Reinforcement Learning

Link: [https://dl.acm.org/doi/abs/10.1007/978-3-030-64583-0_26](https://dl.acm.org/doi/abs/10.1007/978-3-030-64583-0_26) Code: Not Found

**ICML 2019** Collaborative Evolutionary Reinforcement Learning 

Arxiv: [https://arxiv.org/abs/1905.00976](https://arxiv.org/abs/1905.00976) Code: [https://github.com/intelai/cerl](https://github.com/intelai/cerl)

**Preprint** FiDi-RL: Incorporating Deep Reinforcement Learning with Finite-Difference Policy Search for Efficient Learning of Continuous Control

Link: [https://arxiv.org/pdf/1907.00526v2.pdf](https://arxiv.org/pdf/1907.00526v2.pdf) Code: Not Found

**NeurIPS 2018** Evolution-Guided Policy Gradient in Reinforcement Learning

Arxiv: [https://arxiv.org/abs/1810.01222](https://arxiv.org/abs/1810.01222) Code: [https://github.com/apourchot/CEM-RL](https://github.com/apourchot/CEM-RL)


## Multi-Agent Optimization

**ICML 2023** RACE: Improve Multi-Agent Reinforcement Learning with Representation Asymmetry and Collaborative Evolution

**Link**: [https://icml.cc/virtual/2023/poster/23791](https://icml.cc/virtual/2023/poster/23791)  Code: [https://github.com/yeshenpy/RACE](https://github.com/yeshenpy/RACE)

**ICONIP 2022** Cooperation and Competition: Flocking with Evolutionary Multi-Agent Reinforcement Learning

Arxiv: [https://link.springer.com/chapter/10.1007/978-3-031-30105-6_23](https://link.springer.com/chapter/10.1007/978-3-031-30105-6_23) Code: Not Found

**GECCO 2021** MAEDyS: multiagent evolution via dynamic skill selection 

Link [https://dl.acm.org/doi/abs/10.1145/3449639.3459387](https://dl.acm.org/doi/abs/10.1145/3449639.3459387) Code: Not Found

**ICML 2020** Evolutionary Reinforcement Learning for Sample-Efficient Multiagent Coordination

Arxiv: [https://arxiv.org/abs/1906.07315](https://arxiv.org/abs/1906.07315) Code: [Anonymous Code](https://anonymous.4open.science/repository/1590ffb0-aa6b-4838-9d59-ae20cdd8df11/README.md) or [https://github.com/ShawK91/MERL](https://github.com/ShawK91/MERL)


## Others





