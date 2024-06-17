
<!-- # ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)  -->

# 🚀 Awesome-Evolutionary-Reinforcement-Learning
Evolutionary Reinforcement Learning (ERL), which integrates Evolutionary Algorithms (EAs) and Reinforcement Learning (RL) for optimization, has demonstrated remarkable performance advancements. By fusing the strengths of both approaches, ERL has emerged as a promising research direction. 


<!--## [![](https://img.shields.io/badge/-Update%20List-orange)]() --> 

# 📋 Update List

**This repository is under construction ...**

**16 April 2024**: I will be updating the paper and the website this month. The new paper will include more related work. Stay tuned!

**17 February 2024**: I am in the process of filling in the related methods and codes according to the survey.

**23 January 2024**: Our survey paper has been updated on arXiv. Arxiv: **[Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey on Hybrid Algorithms](http://arxiv.org/abs/2401.11963)**  **This survey is now categorized to better align with the conventions of researchers in different fields, providing a quicker and more accessible introduction for researchers.** 

**20 January 2024**: I am updating the survey on this topic and will fully update the site when the survey is updated.

**If you discover any related works that I have missed, please submit an issue. I will update it in the survey and on the website. Thank you very much!**

<!--## [![](https://img.shields.io/badge/-Comment-red.svg)]() -->

# 🔑 Comments

* **If you want to get started, I recommend referring to the *Accepted Papers with the Released Code*, as it provides an easy way to explore research papers and their associated code implementations. 
Furthermore, building your algorithm on top of state-of-the-art algorithms will greatly enhance your productivity and efficiency.**

* If you are interested in sequential decision-making problems, it is recommended to focus primarily on **EA-Assisted Optimization of RL** and **Synergistic Optimization of EA and RL**. If you are interested in other optimization problems, it is suggested to pay attention to **RL-Assisted Optimization of EA**. I primarily focus on the former.



**If you do find our survey or the repository helpful (or if you would be so kind as to offer us some encouragement), please consider kindly giving a star, and citing our paper.**

```
@article{li2024bridging,
  title={Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey},
  author={Pengyi Li and Jianye Hao and Hongyao Tang and Xian Fu and Yan Zheng and Ke Tang},
  journal={arXiv preprint arXiv:2401.11963},
  year={2024}
}
```



# 🎥 Resources

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
  - [Morphological Evolution](#multi-agent-optimization)
  - [Interpretable AI](#multi-agent-optimization)
  - [Learning Classifier Systems](#others-2)


![image](https://github.com/yeshenpy/Awesome-Evolutionary-Reinforcement-Learning/assets/43668853/562fb989-bada-4499-8779-29e5f56be657)

![image](https://github.com/yeshenpy/Awesome-Evolutionary-Reinforcement-Learning/assets/43668853/c3bec864-9b20-42fa-8315-a11acceb9c7c)


Detailed information can be found in our survey paper.


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


**GECCO 2018** Online Meta-learning by Parallel Algorithm Competition

Link: [https://arxiv.org/abs/1702.07490](https://arxiv.org/abs/1702.07490) Code: Not Found

**Preprint 2017** Population Based Training of Neural Networks

Link: [https://arxiv.org/abs/1711.09846](https://arxiv.org/abs/1711.09846) Code: [https://github.com/voiler/PopulationBasedTraining](https://github.com/voiler/PopulationBasedTraining)

**ICLR 2021** Sample-efficient Automated Deep Reinforcement Learning

Link: [https://arxiv.org/abs/2009.01555](https://arxiv.org/abs/2009.01555) Code: [https://github.com/automl/SEARL](https://github.com/automl/SEARL)

**IEEE IRC 2022** GA+DDPG+HER: Genetic Algorithm-based Function Optimizer in Deep Reinforcement Learning for Robotic Manipulation Tasks

Link: [https://arxiv.org/abs/2203.00141](https://arxiv.org/abs/2203.00141) Code: [https://github.com/aralab-unr/ga-drl-aubo-ara-lab](https://github.com/aralab-unr/ga-drl-aubo-ara-lab)

**Preprint 2021** Towards Automatic Actor-critic Solutions to Continuous Control

Link: [https://arxiv.org/abs/2106.08918](https://arxiv.org/abs/2106.08918) Code: [https://github.com/jakegrigsby/deep_control](https://github.com/jakegrigsby/deep_control)

**Preprint 2020** Online Hyper-parameter Tuning in Offpolicy Learning via Evolutionary Strategies

Link: [https://arxiv.org/abs/2006.07554](https://arxiv.org/abs/2006.07554) Code: Not Found

## Others

**ICLR 2021** Evolving Reinforcement Learning Algorithms

Link: [https://arxiv.org/abs/2101.03958](https://arxiv.org/abs/2101.03958) Code: [https://github.com/google/brain_autorl/tree/main/evolving_rl](https://github.com/google/brain_autorl/tree/main/evolving_rl)

**NeurIPS 2022** Discovered Policy Optimisation

Link: [https://arxiv.org/abs/2210.05639](https://arxiv.org/abs/2210.05639) Code: [https://github.com/luchris429/discovered-policy-optimisation](https://github.com/luchris429/discovered-policy-optimisation)

**ICLR 2024** Discovering Temporally-Aware Reinforcement Learning Algorithms

Link: [https://arxiv.org/abs/2402.05828](https://arxiv.org/abs/2402.05828) Code: [https://github.com/EmptyJackson/groove](https://github.com/EmptyJackson/groove)

**ICLR 2024** Behaviour Distillation

Link: [https://openreview.net/forum?id=qup9xD8mW4](https://openreview.net/forum?id=qup9xD8mW4) Code: [https://github.com/FLAIROx/behaviour-distillation](https://github.com/FLAIROx/behaviour-distillation)

**ICML 2023** Adversarial Cheap Talk

Link: [https://arxiv.org/abs/2211.11030](https://arxiv.org/abs/2211.11030) Code: [https://github.com/luchris429/adversarial-cheap-talk](https://github.com/luchris429/adversarial-cheap-talk)

**IROS 2021** PNS: Population-guided Novelty Search for Reinforcement Learning in Hard Exploration Environments

Link: [https://arxiv.org/abs/1811.10264](https://arxiv.org/abs/1811.10264) Code: Not Found

**Nature 2021** Go explore: A New Approach for Hard-exploration Problems

Link: [https://arxiv.org/abs/1901.10995](https://arxiv.org/abs/1901.10995) Code: [https://github.com/uber-research/go-explore](https://github.com/uber-research/go-explore)

**NeurIPS 2018** Genetic-gated Networks for Deep Reinforcement Learning

Link: [https://arxiv.org/abs/1903.01886](https://arxiv.org/abs/1903.01886) Code: Not Found

**GECCO 2021** Evo-rl: Evolutionary-driven Reinforcement Learning

Link: [https://arxiv.org/abs/2007.04725](https://arxiv.org/abs/2007.04725) Code: Not Found

**AAAI 2023** Robust Multi-agent Coordination via Evolutionary Generation of Auxiliary Adversarial Attackers

Link: [https://arxiv.org/abs/2305.05909](https://arxiv.org/abs/2305.05909) Code: [https://github.com/zzq-bot/ROMANCE](https://github.com/zzq-bot/ROMANCE)

**Preprint 2023** Communication-robust Multiagent Learning by Adaptable Auxiliary Multi-agent Adversary Generation

Link: [https://arxiv.org/abs/2305.05116](https://arxiv.org/abs/2305.05116) Code: Not Found

**ICLR 2020** Evolutionary Population Curriculum for Scaling Multi-agent Reinforcement Learning

Link: [https://arxiv.org/abs/2003.10423](https://arxiv.org/abs/2003.10423) Code: [https://github.com/qian18long/epciclr2020](https://github.com/qian18long/epciclr2020)

**IROS 2020** MAPPER: Multi-agent Path Planning with Evolutionary Reinforcement Learning in Mixed Dynamic Environments

Link: [https://arxiv.org/abs/2007.15724](https://arxiv.org/abs/2007.15724) Code: Not Found

# :star: RL-Assisted Optimization of EA
## Population Initialization

**NeurIPS 2021** Symbolic Regression Via Neural-guided Genetic Programming Population Seeding

Link: [https://arxiv.org/pdf/2111.00053.pdf](https://arxiv.org/pdf/2111.00053.pdf) Code: [https://github.com/dso-org/deep-symbolic-optimization](https://github.com/dso-org/deep-symbolic-optimization)

**Knowl Based Syst 2021** Rule-based Reinforcement Learning Methodology To Inform Evolutionary Algorithms For Constrained Optimization Of Engineering Applications

Link: [https://www.sciencedirect.com/science/article/abs/pii/S095070512100099X](https://www.sciencedirect.com/science/article/abs/pii/S095070512100099X) Code: [https://github.com/mradaideh/neorl](https://github.com/mradaideh/neorl)

**NeurIPS 2023** Deepaco: Neuralenhanced Ant Systems For Combinatorial Optimization,

Link: [https://arxiv.org/abs/2309.14032](https://arxiv.org/abs/2309.14032) Code: [https://github.com/henry-yeh/DeepACO](https://github.com/henry-yeh/DeepACO)

## Population Evaluation

**ICLR 2023** ERL-Re2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation 

Arxiv: [https://arxiv.org/abs/2210.17375](https://arxiv.org/abs/2210.17375) Code: [https://github.com/yeshenpy/ERL-Re2](https://github.com/yeshenpy/ERL-Re2)

**ELSEVIER Information Sciences** A Surrogate-Assisted Controller for Expensive Evolutionary Reinforcement Learning

Arxiv: [https://arxiv.org/abs/2201.00129](https://arxiv.org/abs/2201.00129) Code: [https://github.com/Yuxing-Wang-THU/Surrogate-assisted-ERL](https://github.com/Yuxing-Wang-THU/Surrogate-assisted-ERL)

**ICLR 2021 submission** PGPS: Coupling Policy Gradient with Population-based Search

OpenReview: [https://openreview.net/forum?id=PeT5p3ocagr](https://openreview.net/forum?id=PeT5p3ocagr) Code: [https://github.com/NamKim88/PGPS/blob/master/Main.py](https://github.com/NamKim88/PGPS/blob/master/Main.py)

## Variation Operator

**ICLR 2018** Policy Optimization By Genetic Distillation

Link: [https://arxiv.org/abs/1711.01012](https://arxiv.org/abs/1711.01012) Code: Not Found

**AAMMAS 2021** Guiding Evolutionary Strategies With Off-policy Actor-critic

Link: [https://robintyh1.github.io/papers/Tang2021CEMACER.pdf](https://robintyh1.github.io/papers/Tang2021CEMACER.pdf) Code: Not Found

**SSCI 2021** Population Based Reinforcement Learning

Link: [https://ieeexplore.ieee.org/document/9660084](https://ieeexplore.ieee.org/document/9660084) Code: [https://github.com/jjccero/pbrl](https://github.com/jjccero/pbrl)

**IEEE Acess 2020** Efficient Novelty Search Through Deep Reinforcement Learning

Link: [https://ieeexplore.ieee.org/document/9139203](https://ieeexplore.ieee.org/document/9139203) Code: Not Found

**Comput. Intell. Neurosci 2021** Diversity Evolutionary Policy Deep Reinforcement Learning

Link: [https://www.hindawi.com/journals/cin/2021/5300189/](https://www.hindawi.com/journals/cin/2021/5300189/) Code: Not Found

**Arxiv Preprint 2020** QD-RL: Efficient Mixing Of Quality And Diversity In Reinforcement Learning,

Link: [https://www.researchgate.net/publication/342198149_QD-RL_Efficient_Mixing_of_Quality_and_Diversity_in_Reinforcement_Learning](https://www.researchgate.net/publication/342198149_QD-RL_Efficient_Mixing_of_Quality_and_Diversity_in_Reinforcement_Learning) Code: Not Found

**GECCO 2021** Policy Gradient Assisted Map-elites

Link: [https://www.semanticscholar.org/paper/Policy-gradient-assisted-MAP-Elites-Nilsson-Cully/67038237383a8f4802a9595636a6fb73f748dc5b](https://www.semanticscholar.org/paper/Policy-gradient-assisted-MAP-Elites-Nilsson-Cully/67038237383a8f4802a9595636a6fb73f748dc5b) Code: [https://github.com/ollebompa/PGA-MAP-Elites](https://github.com/ollebompa/PGA-MAP-Elites) 

**GECCO 2022** Approximating Gradients For Differentiable Quality Diversity In Reinforcement Learning

Link: [https://arxiv.org/abs/2202.03666](https://arxiv.org/abs/2202.03666) Code: [https://github.com/icaros-usc/dqd-rl](https://github.com/icaros-usc/dqd-rl)

**ICLR 2024** Sample-efficient Quality-diversity By Cooperative Coevolution

Link: [https://openreview.net/forum?id=JDud6zbpFv](https://openreview.net/forum?id=JDud6zbpFv) Code: Not Found

**ICLR 2023** Neuroevolution is a Competitive Alternative to Reinforcement Learning for Skill Discovery

Link: [https://openreview.net/forum?id=6BHlZgyPOZY](https://openreview.net/forum?id=6BHlZgyPOZY) Code: [https://github.com/instadeepai/qd-skill-discovery-benchmark](https://github.com/instadeepai/qd-skill-discovery-benchmark)

**GECCO 2022** Approximating Gradients for Differentiable Quality Diversity in Reinforcement Learning

Link: [https://arxiv.org/pdf/2202.03666.pdf](https://arxiv.org/pdf/2202.03666.pdf) Code: [https://github.com/icaros-usc/dqd-rl](https://github.com/icaros-usc/dqd-rl)

**Preprint 2022** QD-RL: Efficient Mixing of Quality and Diversity in Reinforcement Learning

Link：[https://arxiv.org/abs/2006.08505v2](https://arxiv.org/abs/2006.08505v2) Code: Not Found

**ICLR 2019** CEM-RL: Combining evolutionary and gradient-based methods for policy search

Arxiv: [https://arxiv.org/abs/1810.01222](https://arxiv.org/abs/1810.01222) Code: [https://github.com/apourchot/CEM-RL](https://github.com/apourchot/CEM-RL)

## Dynamic Operator Selection

Waiting for updates

## Hyperparameter Configuration

**ESOA 2006** Reinforcement learning for online control of evolutionary algorithms

Link: [https://link.springer.com/chapter/10.1007/978-3-540-69868-5_10](https://link.springer.com/chapter/10.1007/978-3-540-69868-5_10) Code: Not Found

**PPSN 2020** Learning step-size adaptation in CMA-ES

Link: [https://ml.informatik.uni-freiburg.de/wp-content/uploads/papers/20-PPSN-LTO-CMA.pdf](https://ml.informatik.uni-freiburg.de/wp-content/uploads/papers/20-PPSN-LTO-CMA.pdf) Code: [https://github.com/automl/LTO-CMA](https://github.com/automl/LTO-CMA)

**ECAI 2020** Dynamic algorithm configuration: Foundation of a new meta-algorithmic framework

Link: [https://ecai2020.eu/papers/1237_paper.pdf](https://ecai2020.eu/papers/1237_paper.pdf) Code: [https://github.com/automl/DAC](https://github.com/automl/DAC)

**TETCI 2022** Variational reinforcement learning for hyper-parameter tuning of adaptive evolutionary algorithm

Link: [https://www.researchgate.net/publication/365582495_Variational_Reinforcement_Learning_for_Hyper-Parameter_Tuning_of_Adaptive_Evolutionary_Algorithm](https://www.researchgate.net/publication/365582495_Variational_Reinforcement_Learning_for_Hyper-Parameter_Tuning_of_Adaptive_Evolutionary_Algorithm) Code: Not Found

**IEEE Comput. Intell. Mag., 2023** Controlling sequential hybrid evolutionary algorithm by q-learning

Link: [https://ieeexplore.ieee.org/document/10035716/](https://ieeexplore.ieee.org/document/10035716/) Code: Not Found

**NeurIPS 2022** Multiagent dynamic algorithm configuration

Arxiv: [https://arxiv.org/abs/2210.06835](https://arxiv.org/abs/2210.06835) Code: [https://github.com/lamda-bbo/madac](https://github.com/lamda-bbo/madac)

**Appl. Soft Comput., 2021** Q-learning-based parameter control in differential evolution for structural optimization

Link: [https://www.sciencedirect.com/science/article/abs/pii/S1568494621003872](https://www.sciencedirect.com/science/article/abs/pii/S1568494621003872) Code: Not Found

**Energy Reports, 2021** Reinforcement learning-based differential evolution for parameters extraction of photovoltaic models

Link: [https://www.sciencedirect.com/science/article/pii/S2352484721000974](https://www.sciencedirect.com/science/article/pii/S2352484721000974) Code: Not Found

## Others

**L4DC 2020** Model-predictive control via cross-entropy and gradient-based optimization

Link: [https://proceedings.mlr.press/v120/bharadhwaj20a/bharadhwaj20a.pdf](https://proceedings.mlr.press/v120/bharadhwaj20a/bharadhwaj20a.pdf) Code: [https://github.com/homangab/gradcem](https://github.com/homangab/gradcem)

**CORL 2021** Learning off-policy with online planning

Arxiv: [https://arxiv.org/abs/2008.10066](https://arxiv.org/abs/2008.10066) Code: [https://github.com/hari-sikchi/LOOP](https://github.com/hari-sikchi/LOOP)

**ICML 2022** Temporal difference learning for model predictive control

Arxiv: [https://arxiv.org/abs/2203.04955](https://arxiv.org/abs/2203.04955) Code: [https://github.com/nicklashansen/tdmpc](https://github.com/nicklashansen/tdmpc)

# :star: Synergistic Optimization of EA and RL

## Single-Agent Optimization


**ICLR 2023** ERL-Re2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation 

Arxiv: [https://arxiv.org/abs/2210.17375](https://arxiv.org/abs/2210.17375) Code: [https://github.com/yeshenpy/ERL-Re2](https://github.com/yeshenpy/ERL-Re2)

**ICLR 2021 submission** PGPS: Coupling Policy Gradient with Population-based Search

OpenReview: [https://openreview.net/forum?id=PeT5p3ocagr](https://openreview.net/forum?id=PeT5p3ocagr) Code: [https://github.com/NamKim88/PGPS/blob/master/Main.py](https://github.com/NamKim88/PGPS/blob/master/Main.py)

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

**GECCO 2023** Novelty Seeking Multiagent Evolutionary Reinforcement Learning

Link: [https://dl.acm.org/doi/abs/10.1145/3583131.3590428](https://dl.acm.org/doi/abs/10.1145/3583131.3590428) Code: Not Found

**IJCNN 2023** Evolution Strategies Enhanced Complex Multiagent Coordination

Link: [https://ieeexplore.ieee.org/document/10191313](https://ieeexplore.ieee.org/document/10191313) Code: Not Found

**ICONIP 2022** Cooperation and Competition: Flocking with Evolutionary Multi-Agent Reinforcement Learning

Arxiv: [https://link.springer.com/chapter/10.1007/978-3-031-30105-6_23](https://link.springer.com/chapter/10.1007/978-3-031-30105-6_23) Code: Not Found

**GECCO 2021** MAEDyS: multiagent evolution via dynamic skill selection 

Link [https://dl.acm.org/doi/abs/10.1145/3449639.3459387](https://dl.acm.org/doi/abs/10.1145/3449639.3459387) Code: Not Found

**ICML 2020** Evolutionary Reinforcement Learning for Sample-Efficient Multiagent Coordination

Arxiv: [https://arxiv.org/abs/1906.07315](https://arxiv.org/abs/1906.07315) Code: [Anonymous Code](https://anonymous.4open.science/repository/1590ffb0-aa6b-4838-9d59-ae20cdd8df11/README.md) or [https://github.com/ShawK91/MERL](https://github.com/ShawK91/MERL)


## Morphological Evolution

Waiting for updates

## Interpretable AI

Waiting for updates

## Learning Classifier Systems

Waiting for updates


