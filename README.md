# Awesome Evolutionary Reinforcement Learning

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Survey](https://img.shields.io/badge/Survey-arXiv%3A2401.11963-b31b1b.svg)](https://arxiv.org/abs/2401.11963)
[![IEEE TEVC](https://img.shields.io/badge/IEEE%20TEVC-2025-00629B.svg)](https://doi.org/10.1109/TEVC.2024.3443913)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](#contributing)

A curated collection of papers, implementations, benchmarks, and tooling for **Evolutionary Reinforcement Learning (ERL)**: hybrid methods that combine Evolutionary Algorithms (EAs) and Reinforcement Learning (RL).

This repository follows the taxonomy in the latest version of:

> **Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey on Hybrid Algorithms**
> Pengyi Li, Jianye Hao, Hongyao Tang, Xian Fu, Yan Zheng, and Ke Tang.
> IEEE Transactions on Evolutionary Computation, 29(5):1707-1728, 2025.
> [IEEE](https://doi.org/10.1109/TEVC.2024.3443913) | [arXiv v5](https://arxiv.org/abs/2401.11963) | [PDF](https://arxiv.org/pdf/2401.11963)

## Latest update

- **28 Aug 2026**: synchronized the repository with arXiv v5; added Reward Design, Dynamic Operator Selection, missing QD methods, recent 2024-2026 works, code repositories, frameworks, and updated taxonomy figures.
- **26 Jul 2024**: the survey was accepted by IEEE Transactions on Evolutionary Computation.

If a paper, codebase, or category is missing, please [open an issue](https://github.com/yeshenpy/Awesome-Evolutionary-Reinforcement-Learning/issues) with its BibTeX entry, official paper URL, official code URL, and proposed category.

## Contents

- [How to use this list](#how-to-use-this-list)
- [Taxonomy](#taxonomy)
- [Code-first reading list](#code-first-reading-list)
- [EA-assisted Optimization of RL](#ea-assisted-optimization-of-rl)
  - [EA-assisted Parameter Search](#ea-assisted-parameter-search)
  - [EA-assisted Action Selection](#ea-assisted-action-selection)
  - [Hyperparameter Optimization](#hyperparameter-optimization)
  - [Other EA-assisted RL methods](#other-ea-assisted-rl-methods)
- [RL-assisted Optimization of EA](#rl-assisted-optimization-of-ea)
  - [Population Initialization](#population-initialization)
  - [Population Evaluation](#population-evaluation)
  - [Variation Operator](#variation-operator)
  - [Dynamic Operator Selection](#dynamic-operator-selection)
  - [Hyperparameter Configuration](#hyperparameter-configuration)
  - [Other RL-assisted EA methods](#other-rl-assisted-ea-methods)
- [Synergistic Optimization of EA and RL](#synergistic-optimization-of-ea-and-rl)
  - [Single-Agent Optimization](#single-agent-optimization)
  - [Multi-Agent Optimization](#multi-agent-optimization)
  - [Reward Design](#reward-design)
  - [Morphological Evolution](#morphological-evolution)
  - [Interpretable AI](#interpretable-ai)
  - [Learning Classifier Systems](#learning-classifier-systems)
- [Frameworks, benchmarks, and tooling](#frameworks-benchmarks-and-tooling)
- [Recent and emerging directions](#recent-and-emerging-directions)
- [Related surveys](#related-surveys)
- [Contributing](#contributing)
- [Citation](#citation)

## How to use this list

- For sequential decision-making, begin with **EA-assisted Optimization of RL** and **Synergistic Optimization of EA and RL**.
- For combinatorial, continuous, multi-objective, or multimodal optimization, begin with **RL-assisted Optimization of EA**.
- For reproducible baselines, start from the [code-first reading list](#code-first-reading-list) and [frameworks](#frameworks-benchmarks-and-tooling).
- `Code: Not found` means that no author-maintained public repository was verified. Paper pages are never labeled as code.
- Some works are intentionally cross-listed because the same mechanism contributes to more than one branch.

## Taxonomy

The survey organizes ERL into three major directions and sixteen research branches.

![ERL taxonomy](assets/erl-taxonomy.png)

The image reproduces survey v5 Figure 1. The v5 body and Table V additionally include **LERO** under Reward Design and explicitly discuss **XCSRG** alongside XCSG; the detailed tables below follow the body and tables when they are more complete than the figure.

The four integration patterns clarify whether EA assists RL, RL assists EA, or both optimizers collaborate in solution or decomposed problem spaces.

![Four integration approaches](assets/integration-approaches.png)

## Code-first reading list

The following papers have public implementations verified against the paper, project page, or authors' repositories and are useful starting points. Community reimplementations are kept out of this short list and labeled explicitly in the full taxonomy.

| Direction | Method | Paper | Code |
|---|---|---|---|
| EA-assisted RL | SAC-CEPO | [Soft Actor-Critic with Cross-Entropy Policy Optimization](https://arxiv.org/abs/2112.11115) | [wcgcyx/SAC-CEPO](https://github.com/wcgcyx/SAC-CEPO) |
| EA-assisted RL | GRAC | [GRAC: Self-Guided and Self-Regularized Actor-Critic](https://arxiv.org/abs/2009.08973) | [stanford-iprl-lab/GRAC](https://github.com/stanford-iprl-lab/GRAC) |
| EA-assisted RL | OMAR | [Plan Better Amid Conservatism: Offline Multi-Agent Reinforcement Learning with Actor Rectification](https://arxiv.org/abs/2111.11188) | [ling-pan/OMAR](https://github.com/ling-pan/OMAR) |
| EA-assisted RL | SEARL | [Sample-Efficient Automated Deep Reinforcement Learning](https://arxiv.org/abs/2009.01555) | [automl/SEARL](https://github.com/automl/SEARL) |
| EA-assisted RL | Evolving RL Algorithms | [Evolving Reinforcement Learning Algorithms](https://arxiv.org/abs/2101.03958) | [google/brain_autorl](https://github.com/google/brain_autorl/tree/main/evolving_rl) |
| EA-assisted RL | Go-Explore | [A New Approach for Hard-Exploration Problems](https://arxiv.org/abs/1901.10995) | [uber-research/go-explore](https://github.com/uber-research/go-explore) |
| EA-assisted RL | ROMANCE | [Robust Multi-Agent Coordination via Evolutionary Generation of Auxiliary Adversarial Attackers](https://arxiv.org/abs/2305.05909) | [zzq-bot/ROMANCE](https://github.com/zzq-bot/ROMANCE) |
| EA-assisted RL | EvIL | [Evolution Strategies for Generalisable Imitation Learning](https://arxiv.org/abs/2406.11905) | [SilviaSapora/evil](https://github.com/SilviaSapora/evil) |
| RL-assisted EA | DeepACO | [Neural-Enhanced Ant Systems for Combinatorial Optimization](https://arxiv.org/abs/2309.14032) | [henry-yeh/DeepACO](https://github.com/henry-yeh/DeepACO) |
| RL-assisted EA | CEM-RL | [Combining Evolutionary and Gradient-Based Methods for Policy Search](https://arxiv.org/abs/1810.01222) | [apourchot/CEM-RL](https://github.com/apourchot/CEM-RL) |
| RL-assisted EA | PBRL | [Population Based Reinforcement Learning](https://ieeexplore.ieee.org/document/9660084) | [jjccero/pbrl](https://github.com/jjccero/pbrl) |
| RL-assisted EA | PGA-ME | [Policy Gradient Assisted MAP-Elites](https://doi.org/10.1145/3449639.3459304) | [ollebompa/PGA-MAP-Elites](https://github.com/ollebompa/PGA-MAP-Elites) |
| RL-assisted EA | CMA-MEGA | [Approximating Gradients for Differentiable Quality Diversity in Reinforcement Learning](https://arxiv.org/abs/2202.03666) | [icaros-usc/dqd-rl](https://github.com/icaros-usc/dqd-rl) |
| RL-assisted EA | CCQD | [Sample-Efficient Quality-Diversity by Cooperative Coevolution](https://openreview.net/forum?id=JDud6zbpFv) | [lamda-bbo/CCQD](https://github.com/lamda-bbo/CCQD) |
| RL-assisted EA | RefQD | [Quality-Diversity with Limited Resources](https://arxiv.org/abs/2406.03731) | [lamda-bbo/RefQD](https://github.com/lamda-bbo/RefQD) |
| RL-assisted EA | Wuji | [Automatic Online Combat Game Testing Using Evolutionary Deep Reinforcement Learning](https://doi.org/10.1109/ASE.2019.00077) | [NeteaseFuxiRL/wuji](https://github.com/NeteaseFuxiRL/wuji) |
| Synergistic | ERL | [Evolution-Guided Policy Gradient in Reinforcement Learning](https://arxiv.org/abs/1805.07917) | [ShawK91/Evolutionary-Reinforcement-Learning](https://github.com/ShawK91/Evolutionary-Reinforcement-Learning) |
| Synergistic | CERL | [Collaborative Evolutionary Reinforcement Learning](https://arxiv.org/abs/1905.00976) | [intelai/cerl](https://github.com/intelai/cerl) |
| Synergistic | PDERL | [Proximal Distilled Evolutionary Reinforcement Learning](https://arxiv.org/abs/1906.09807) | [crisbodnar/pderl](https://github.com/crisbodnar/pderl) |
| Synergistic | ERL-Re2 | [ERL-Re^2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation](https://arxiv.org/abs/2210.17375) | [yeshenpy/ERL-Re2](https://github.com/yeshenpy/ERL-Re2) |
| Synergistic | VEB-RL | [Value-Evolutionary-Based Reinforcement Learning](https://openreview.net/forum?id=XobPpcN4yZ) | [yeshenpy/VEB-RL](https://github.com/yeshenpy/VEB-RL) |
| Synergistic | EvoRainbow | [EvoRainbow: Combining Improvements in Evolutionary Reinforcement Learning for Policy Search](https://openreview.net/forum?id=75Hes6Zse4) | [yeshenpy/EvoRainbow](https://github.com/yeshenpy/EvoRainbow) |
| Synergistic | RACE | [RACE: Improve Multi-Agent Reinforcement Learning with Representation Asymmetry and Collaborative Evolution](https://proceedings.mlr.press/v202/li23r.html) | [yeshenpy/RACE](https://github.com/yeshenpy/RACE) |
| Synergistic | CORE | [CORE: Collaborative Optimization with Reinforcement Learning and Evolutionary Algorithm for Floorplanning](https://papers.neurips.cc/paper_files/paper/2025/hash/cc0f00fd7c873fe2b196529e19b1a6bf-Abstract-Conference.html) | [yeshenpy/CORE](https://github.com/yeshenpy/CORE) |
| Reward design | Eureka | [Human-Level Reward Design via Coding Large Language Models](https://openreview.net/forum?id=IEduRUO55F) | [eureka-research/Eureka](https://github.com/eureka-research/Eureka) |
| Reward design | DrEureka | [Language Model Guided Sim-to-Real Transfer](https://arxiv.org/abs/2406.01967) | [eureka-research/dreureka](https://github.com/eureka-research/dreureka) |
| Reward design | LaRes | [LaRes: Evolutionary Reinforcement Learning with LLM-Based Adaptive Reward Search](https://openreview.net/forum?id=jRjvcqtdtA) | [yeshenpy/LaRes](https://github.com/yeshenpy/LaRes) |
| Morphology | EvoGym | [Evolution Gym: A Large-Scale Benchmark for Evolving Soft Robots](https://arxiv.org/abs/2201.09863) | [EvolutionGym/evogym](https://github.com/EvolutionGym/evogym) |
| Morphology | HERD | [Leveraging Hyperbolic Embeddings for Coarse-to-Fine Robot Design](https://arxiv.org/abs/2311.00462) | [drdh/HERD](https://github.com/drdh/HERD) |
| Morphology | AIEA | [Rapidly Evolving Soft Robots via Action Inheritance](https://doi.org/10.1109/TEVC.2023.3327459) | [HandingWangXDGroup/AIEA](https://github.com/HandingWangXDGroup/AIEA) |
| Morphology | DERL | [Embodied Intelligence via Learning and Evolution](https://arxiv.org/abs/2102.02202) | [agrimgupta92/derl](https://github.com/agrimgupta92/derl) |
| Morphology | TAME | [Task-Agnostic Morphology Evolution](https://arxiv.org/abs/2102.13100) | [jhejna/morphology-opt](https://github.com/jhejna/morphology-opt) |

# EA-assisted Optimization of RL

EA is used as a supporting optimizer for RL. The RL process remains responsible for solving the task.

## EA-assisted Parameter Search

| Method | Paper | Venue | Code |
|---|---|---|---|
| EQ | [Reinforcement Learning Beyond the Bellman Equation](https://direct.mit.edu/isal/proceedings/isal2020/32/441/98464) | ALIFE 2020 | [ajleite/RLBeyondBellman](https://github.com/ajleite/RLBeyondBellman) |
| Supe-RL | [Genetic Soft Updates for Policy Evolution in Deep Reinforcement Learning](https://openreview.net/forum?id=TGFO0DbD_pk) | ICLR 2021 | Not found |
| VFS | [Improving Deep Policy Gradients with Value Function Search](https://openreview.net/forum?id=6qZC7pfenQm) | ICLR 2023 | Not found |

## EA-assisted Action Selection

| Method | Paper | Venue | Code |
|---|---|---|---|
| Qt-Opt | [Scalable Deep Reinforcement Learning for Vision-Based Robotic Manipulation](https://proceedings.mlr.press/v87/kalashnikov18a.html) | CoRL 2018 | [community reimplementation](https://github.com/quantumiracle/QT_Opt) |
| CGP | [Q-Learning for Continuous Actions with Cross-Entropy Guided Policies](https://arxiv.org/abs/1903.10605) | ICML RL4RealLife 2019 | Not found |
| EAS-RL | [Evolutionary Action Selection for Gradient-Based Policy Learning](https://doi.org/10.1007/978-3-031-30111-7_49) | ICONIP 2022 | Not found |
| SAC-CEPO | [Soft Actor-Critic with Cross-Entropy Policy Optimization](https://arxiv.org/abs/2112.11115) | Preprint 2021 | [wcgcyx/SAC-CEPO](https://github.com/wcgcyx/SAC-CEPO) |
| GRAC | [Self-Guided and Self-Regularized Actor-Critic](https://arxiv.org/abs/2009.08973) | CoRL 2021 | [stanford-iprl-lab/GRAC](https://github.com/stanford-iprl-lab/GRAC) |
| OMAR | [Plan Better Amid Conservatism: Offline Multi-Agent Reinforcement Learning with Actor Rectification](https://arxiv.org/abs/2111.11188) | ICML 2022 | [ling-pan/OMAR](https://github.com/ling-pan/OMAR) |
| COMIX | [Deep Multi-Agent RL for Decentralized Continuous Cooperative Control](https://arxiv.org/abs/2003.06709v1) | Preprint 2020 | [oxwhirl/comix](https://github.com/oxwhirl/comix) |

## Hyperparameter Optimization

| Method | Paper | Venue | Code |
|---|---|---|---|
| OMPAC | [Online Meta-Learning by Parallel Algorithm Competition](https://arxiv.org/abs/1702.07490) | GECCO 2018 | Not found |
| PBT | [Population Based Training of Neural Networks](https://arxiv.org/abs/1711.09846) | Preprint 2017 | Not found |
| SEARL | [Sample-Efficient Automated Deep Reinforcement Learning](https://arxiv.org/abs/2009.01555) | ICLR 2021 | [automl/SEARL](https://github.com/automl/SEARL) |
| GA-DRL | [Genetic Algorithm-Based Function Optimizer in DRL for Robotic Manipulation](https://arxiv.org/abs/2203.00141) | IEEE IRC 2022 | [aralab-unr/ga-drl-aubo-ara-lab](https://github.com/aralab-unr/ga-drl-aubo-ara-lab) |
| AAC | [Towards Automatic Actor-Critic Solutions to Continuous Control](https://arxiv.org/abs/2106.08918) | Preprint 2021 | [jakegrigsby/deep_control](https://github.com/jakegrigsby/deep_control) |
| OHT-ES | [Online Hyper-Parameter Tuning in Off-Policy Learning via Evolutionary Strategies](https://arxiv.org/abs/2006.07554) | Preprint 2020 | Not found |

## Other EA-assisted RL methods

| Method | Paper | Venue | Code |
|---|---|---|---|
| Evo-Reward | [Genetic Programming for Reward Function Search](https://doi.org/10.1109/TAMD.2010.2051436) | IEEE TAMD 2010 | Not found |
| DQNClipped / DQNReg | [Evolving Reinforcement Learning Algorithms](https://arxiv.org/abs/2101.03958) | ICLR 2021 | [google/brain_autorl](https://github.com/google/brain_autorl/tree/main/evolving_rl) |
| GP-MAXQ | [Evolutionary Development of Hierarchical Learning Structures](https://faculty.cc.gatech.edu/~hic/hic-papers/04141056.pdf) | IEEE TEVC 2007 | Not found |
| PNS-RL | [PNS: Population-Guided Novelty Search for Reinforcement Learning in Hard Exploration Environments](https://arxiv.org/abs/1811.10264) | IROS 2021 | Not found |
| Go-Explore | [A New Approach for Hard-Exploration Problems](https://arxiv.org/abs/1901.10995) | Nature 2021 | [uber-research/go-explore](https://github.com/uber-research/go-explore) |
| G2N | [Genetic-Gated Networks for Deep Reinforcement Learning](https://arxiv.org/abs/1903.01886) | NeurIPS 2018 | Not found |
| EVO-RL | [Evolutionary-Driven Reinforcement Learning](https://arxiv.org/abs/2007.04725) | GECCO 2021 | Not found |
| ROMANCE | [Robust Multi-Agent Coordination via Evolutionary Generation of Auxiliary Adversarial Attackers](https://arxiv.org/abs/2305.05909) | AAAI 2023 | [zzq-bot/ROMANCE](https://github.com/zzq-bot/ROMANCE) |
| MA3C | [Communication-Robust Multi-Agent Learning by Adaptable Auxiliary Adversary Generation](https://arxiv.org/abs/2305.05116) | Preprint 2023 | Not found |
| EPC | [Evolutionary Population Curriculum for Scaling Multi-Agent RL](https://arxiv.org/abs/2003.10423) | ICLR 2020 | [qian18long/epciclr2020](https://github.com/qian18long/epciclr2020) |
| MAPPER | [MAPPER: Multi-Agent Path Planning with Evolutionary Reinforcement Learning in Mixed Dynamic Environments](https://arxiv.org/abs/2007.15724) | IROS 2020 | Not found |
| EvIL | [Evolution Strategies for Generalisable Imitation Learning](https://arxiv.org/abs/2406.11905) | ICML 2024 | [SilviaSapora/evil](https://github.com/SilviaSapora/evil) |

# RL-assisted Optimization of EA

RL is used as a supporting optimizer for one or more stages of an EA.

## Population Initialization

| Method | Paper | Venue | Code |
|---|---|---|---|
| NGGP | [Symbolic Regression via Neural-Guided Genetic Programming Population Seeding](https://arxiv.org/abs/2111.00053) | NeurIPS 2021 | [dso-org/deep-symbolic-optimization](https://github.com/dso-org/deep-symbolic-optimization) |
| RL-guided GA | [Rule-Based Reinforcement Learning to Inform Evolutionary Algorithms](https://doi.org/10.1016/j.knosys.2021.106836) | Knowledge-Based Systems 2021 | [mradaideh/neorl](https://github.com/mradaideh/neorl) |
| DeepACO | [Neural-Enhanced Ant Systems for Combinatorial Optimization](https://arxiv.org/abs/2309.14032) | NeurIPS 2023 | [henry-yeh/DeepACO](https://github.com/henry-yeh/DeepACO) |

## Population Evaluation

These methods are intentionally cross-listed with synergistic policy optimization because RL both evaluates and exchanges information with the population.

- **SC** - [A Surrogate-Assisted Controller for Expensive Evolutionary Reinforcement Learning](https://arxiv.org/abs/2201.00129) - [code](https://github.com/Yuxing-Wang-THU/Surrogate-assisted-ERL)
- **PGPS** - [Coupling Policy Gradient with Population-Based Search](https://openreview.net/forum?id=PeT5p3ocagr) - Code: Not found
- **ERL-Re2** - [ERL-Re^2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation](https://arxiv.org/abs/2210.17375) - [code](https://github.com/yeshenpy/ERL-Re2)

## Variation Operator

| Method | Paper | Code |
|---|---|---|
| GPO | [Policy Optimization by Genetic Distillation](https://arxiv.org/abs/1711.01012) | Not found |
| CEM-RL | [Combining Evolutionary and Gradient-Based Methods for Policy Search](https://arxiv.org/abs/1810.01222) | [apourchot/CEM-RL](https://github.com/apourchot/CEM-RL) |
| CEM-ACER | [Guiding Evolutionary Strategies with Off-Policy Actor-Critic](https://dl.acm.org/doi/10.5555/3463952.3464104) | Not found |
| PBRL | [Population Based Reinforcement Learning](https://ieeexplore.ieee.org/document/9660084) | [jjccero/pbrl](https://github.com/jjccero/pbrl) |
| NS-RL | [Efficient Novelty Search through Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9139203) | [shilx001/NoveltySearch_Improvement](https://github.com/shilx001/NoveltySearch_Improvement) |
| DEPRL | [Diversity Evolutionary Policy Deep Reinforcement Learning](https://doi.org/10.1155/2021/5300189) | Not found |
| QD-RL | [QD-RL: Efficient Mixing of Quality and Diversity in Reinforcement Learning](https://arxiv.org/abs/2006.08505v1) | Not found |
| PGA-ME | [Policy Gradient Assisted MAP-Elites](https://doi.org/10.1145/3449639.3459304) | [ollebompa/PGA-MAP-Elites](https://github.com/ollebompa/PGA-MAP-Elites) |
| GAC QD-RL | [Understanding Synergies between Quality-Diversity and Deep RL](https://arxiv.org/abs/2303.06164) | Not found |
| CMA-MEGA | [Approximating Gradients for Differentiable Quality Diversity in RL](https://arxiv.org/abs/2202.03666) | [icaros-usc/dqd-rl](https://github.com/icaros-usc/dqd-rl) |
| CCQD | [Sample-Efficient Quality-Diversity by Cooperative Coevolution](https://openreview.net/forum?id=JDud6zbpFv) | [lamda-bbo/CCQD](https://github.com/lamda-bbo/CCQD) |
| RefQD | [Quality-Diversity with Limited Resources](https://arxiv.org/abs/2406.03731) | [lamda-bbo/RefQD](https://github.com/lamda-bbo/RefQD) |
| Wuji | [Automatic Online Combat Game Testing Using Evolutionary Deep RL](https://doi.org/10.1109/ASE.2019.00077) | [NeteaseFuxiRL/wuji](https://github.com/NeteaseFuxiRL/wuji) |

## Dynamic Operator Selection

This branch was empty in the previous README. Survey v5 identifies sixteen methods.

| Method | Paper | Venue | Code |
|---|---|---|---|
| RL-GA(a) | [Controlling Genetic Algorithms with Reinforcement Learning](https://dl.acm.org/doi/10.5555/2955491.2955607) | GECCO 2002 | Not found |
| RLEP | [Adaptive Evolutionary Programming Based on Reinforcement Learning](https://doi.org/10.1016/j.ins.2007.09.026) | Information Sciences 2008 | Not found |
| EA+RL | [Increasing Efficiency of Evolutionary Algorithms by Choosing between Auxiliary Fitness Functions with Reinforcement Learning](https://doi.org/10.1109/ICMLA.2012.32) | ICMLA 2012 | Not found |
| EA+RL(O) | [Selecting Evolutionary Operators Using Reinforcement Learning: Initial Explorations](https://doi.org/10.1145/2598394.2605681) | GECCO 2014 | Not found |
| RL-GA(b) | [RL-GA: A Reinforcement Learning-Based Genetic Algorithm for Electromagnetic Detection Satellite Scheduling](https://doi.org/10.1016/j.swevo.2023.101236) | Swarm and Evolutionary Computation 2023 | Not found |
| GSF | [Automated Design of Metaheuristics Using Reinforcement Learning within a Novel General Search Framework](https://doi.org/10.1109/TEVC.2022.3197298) | IEEE TEVC 2023 | Not found |
| MARLwCMA | [Evolutionary Framework with Reinforcement Learning-Based Mutation Adaptation](https://doi.org/10.1109/ACCESS.2020.3033593) | IEEE Access 2020 | Not found |
| MPSORL | [Multi-Strategy Self-Learning Particle Swarm Optimization Based on Reinforcement Learning](https://doi.org/10.3934/mbe.2023373) | Mathematical Biosciences and Engineering 2023 | Not found |
| DEDQN | [Differential Evolution with Mixed Mutation Strategy Based on Deep Reinforcement Learning](https://doi.org/10.1016/j.asoc.2021.107678) | Applied Soft Computing 2021 | Not found |
| DE-DDQN | [Deep Reinforcement Learning Based Parameter Control in Differential Evolution](https://doi.org/10.1145/3321707.3321813) | GECCO 2019 | Not found |
| RL-CORCO | [Constrained Evolutionary Optimization Based on Reinforcement Learning Using the Objective Function and Constraints](https://doi.org/10.1016/j.knosys.2021.107731) | Knowledge-Based Systems 2022 | Not found |
| RL-HDE | [Reinforcement Learning-Based Hybrid Differential Evolution for Global Optimization of Interplanetary Trajectory Design](https://doi.org/10.1016/j.swevo.2023.101351) | Swarm and Evolutionary Computation 2023 | Not found |
| DE-RLFR | [Differential Evolution Based on Reinforcement Learning with Fitness Ranking for Multimodal Multiobjective Problems](https://doi.org/10.1016/j.swevo.2019.06.010) | Swarm and Evolutionary Computation 2019 | Not found |
| LRMODE | [A Fitness Landscape Ruggedness Multiobjective Differential Evolution Algorithm with a Reinforcement Learning Strategy](https://doi.org/10.1016/j.asoc.2020.106693) | Applied Soft Computing 2020 | Not found |
| MOEA/D-DQN | [Deep Reinforcement Learning Based Adaptive Operator Selection for Evolutionary Multi-Objective Optimization](https://doi.org/10.1109/TETCI.2022.3146882) | IEEE TETCI 2023 | Not found |
| AMODE-DRL | [Scheduling of Continuous Annealing with a Multi-Objective Differential Evolution Algorithm Based on Deep Reinforcement Learning](https://doi.org/10.1109/TASE.2023.3244331) | IEEE T-ASE 2024 | Not found |

## Hyperparameter Configuration

Survey v5 contains: `AGA`, `LTO`, `RL-DAC`, `REM`, `Q-LSHADE & DQ-HSES`, `MADAC`, `qlDE`, and `RLDE`.

| Method | Paper | Code |
|---|---|---|
| AGA | [Reinforcement Learning for Online Control of Evolutionary Algorithms](https://link.springer.com/chapter/10.1007/978-3-540-69868-5_10) | Not found |
| LTO | [Learning Step-Size Adaptation in CMA-ES](https://ml.informatik.uni-freiburg.de/wp-content/uploads/papers/20-PPSN-LTO-CMA.pdf) | [automl/LTO-CMA](https://github.com/automl/LTO-CMA) |
| RL-DAC | [Dynamic Algorithm Configuration: Foundation of a New Meta-Algorithmic Framework](https://doi.org/10.3233/FAIA200122) | [automl/DAC](https://github.com/automl/DAC) |
| REM | [Variational Reinforcement Learning for Hyper-Parameter Tuning of Adaptive Evolutionary Algorithm](https://doi.org/10.1109/TETCI.2022.3221483) | Not found |
| MADAC | [Multiagent Dynamic Algorithm Configuration](https://arxiv.org/abs/2210.06835) | [lamda-bbo/madac](https://github.com/lamda-bbo/madac) |
| Q-LSHADE & DQ-HSES | [Controlling Sequential Hybrid EA by Q-Learning](https://ieeexplore.ieee.org/document/10035716) | [official code](https://github.com/xiaomeiabc/Controlling-Sequential-Hybrid-Evolutionary-Algorithm-by-Q-Learning) |
| qlDE | [Q-Learning-Based Parameter Control in Differential Evolution for Structural Optimization](https://doi.org/10.1016/j.asoc.2021.107464) | Not found |
| RLDE | [Reinforcement Learning-Based Differential Evolution for Parameters Extraction of Photovoltaic Models](https://doi.org/10.1016/j.egyr.2021.01.096) | Not found |

## Other RL-assisted EA methods

| Method | Paper | Code |
|---|---|---|
| Grad-CEM | [Model-Predictive Control via Cross-Entropy and Gradient-Based Optimization](https://proceedings.mlr.press/v120/bharadhwaj20a.html) | [homangab/gradcem](https://github.com/homangab/gradcem) |
| LOOP | [Learning Off-Policy with Online Planning](https://arxiv.org/abs/2008.10066) | [hari-sikchi/LOOP](https://github.com/hari-sikchi/LOOP) |
| TD-MPC | [Temporal Difference Learning for Model Predictive Control](https://arxiv.org/abs/2203.04955) | [nicklashansen/tdmpc](https://github.com/nicklashansen/tdmpc) |
| RGP | [Reinforced Genetic Programming](https://doi.org/10.1023/A:1011953410319) | Not found |
| GNP-RL | [A Graph-Based Evolutionary Algorithm: Genetic Network Programming (GNP) and Its Extension Using Reinforcement Learning](https://doi.org/10.1162/evco.2007.15.3.369) | Not found |
| LPO | [Discovered Policy Optimisation](https://arxiv.org/abs/2210.05639) | [luchris429/discovered-policy-optimisation](https://github.com/luchris429/discovered-policy-optimisation) |
| TA-LPG / TA-LPO | [Discovering Temporally-Aware RL Algorithms](https://arxiv.org/abs/2402.05828) | [EmptyJackson/groove](https://github.com/EmptyJackson/groove) |

# Synergistic Optimization of EA and RL

EA and RL both contribute directly to solving the task, either in a shared solution space or through decomposed subproblems.

## Single-Agent Optimization

| Method | Paper | Venue | Code |
|---|---|---|---|
| ERL | [Evolution-Guided Policy Gradient in Reinforcement Learning](https://arxiv.org/abs/1805.07917) | NeurIPS 2018 | [ShawK91/Evolutionary-Reinforcement-Learning](https://github.com/ShawK91/Evolutionary-Reinforcement-Learning) |
| CERL | [Collaborative Evolutionary Reinforcement Learning](https://arxiv.org/abs/1905.00976) | ICML 2019 | [intelai/cerl](https://github.com/intelai/cerl) |
| PDERL | [Proximal Distilled Evolutionary Reinforcement Learning](https://arxiv.org/abs/1906.09807) | AAAI 2020 | [crisbodnar/pderl](https://github.com/crisbodnar/pderl) |
| SC | [A Surrogate-Assisted Controller for Expensive Evolutionary Reinforcement Learning](https://arxiv.org/abs/2201.00129) | Information Sciences 2022 | [Yuxing-Wang-THU/Surrogate-assisted-ERL](https://github.com/Yuxing-Wang-THU/Surrogate-assisted-ERL) |
| GEATL | [Evolutionary Reinforcement Learning for Sparse Rewards](https://doi.org/10.1145/3449726.3463142) | GECCO 2021 | Not found |
| CSPS | [Cooperative Heterogeneous Deep Reinforcement Learning](https://arxiv.org/abs/2011.00791) | NeurIPS 2020 | Not found |
| T-ERL | [Rethinking Population-Assisted Off-Policy Reinforcement Learning](https://doi.org/10.1145/3583131.3590512) | GECCO 2023 | Not found |
| ESAC | [Off-Policy Evolutionary Reinforcement Learning with Maximum Mutations](https://www.ifaamas.org/Proceedings/aamas2022/pdfs/p1237.pdf) | AAMAS 2022 | [karush17/esac](https://github.com/karush17/esac) |
| PGPS | [Coupling Policy Gradient with Population-Based Search](https://openreview.net/forum?id=PeT5p3ocagr) | ICLR 2021 submission | Not found |
| ERL-Re2 | [ERL-Re^2: Efficient Evolutionary Reinforcement Learning with Shared State Representation and Individual Policy Representation](https://arxiv.org/abs/2210.17375) | ICLR 2023 | [yeshenpy/ERL-Re2](https://github.com/yeshenpy/ERL-Re2) |
| VEB-RL | [Value-Evolutionary-Based Reinforcement Learning](https://openreview.net/forum?id=XobPpcN4yZ) | ICML 2024 | [yeshenpy/VEB-RL](https://github.com/yeshenpy/VEB-RL) |
| EvoRainbow | [EvoRainbow: Combining Improvements in Evolutionary Reinforcement Learning for Policy Search](https://openreview.net/forum?id=75Hes6Zse4) | ICML 2024 | [yeshenpy/EvoRainbow](https://github.com/yeshenpy/EvoRainbow) |
| EvoRainbow-Exp | [EvoRainbow: Combining Improvements in Evolutionary Reinforcement Learning for Policy Search](https://openreview.net/forum?id=75Hes6Zse4) | ICML 2024 | [yeshenpy/EvoRainbow](https://github.com/yeshenpy/EvoRainbow) |
| CORE | [CORE: Collaborative Optimization with Reinforcement Learning and Evolutionary Algorithm for Floorplanning](https://papers.neurips.cc/paper_files/paper/2025/hash/cc0f00fd7c873fe2b196529e19b1a6bf-Abstract-Conference.html) | NeurIPS 2025 | [yeshenpy/CORE](https://github.com/yeshenpy/CORE) |

## Multi-Agent Optimization

| Method | Paper | Venue | Code |
|---|---|---|---|
| MERL | [Evolutionary Reinforcement Learning for Sample-Efficient Multiagent Coordination](https://arxiv.org/abs/1906.07315) | ICML 2020 | [ShawK91/MERL](https://github.com/ShawK91/MERL) |
| NS-MERL | [Novelty Seeking Multi-Agent ERL](https://dl.acm.org/doi/10.1145/3583131.3590428) | GECCO 2023 | Not found |
| CEMARL | [Evolution Strategies Enhanced Complex Multiagent Coordination](https://ieeexplore.ieee.org/document/10191313) | IJCNN 2023 | Not found |
| EMARL | [Cooperation and Competition: Flocking with Evolutionary Multi-Agent Reinforcement Learning](https://link.springer.com/chapter/10.1007/978-3-031-30105-6_23) | ICONIP 2022 | Not found |
| RACE | [RACE: Improve Multi-Agent Reinforcement Learning with Representation Asymmetry and Collaborative Evolution](https://proceedings.mlr.press/v202/li23r.html) | ICML 2023 | [yeshenpy/RACE](https://github.com/yeshenpy/RACE) |

## Reward Design

This branch is new relative to the previous README. LLM-based evolutionary search has made reward design a major ERL direction.

| Method | Paper | Venue | Code |
|---|---|---|---|
| Evo-Reward | [Genetic Programming for Reward Function Search](https://doi.org/10.1109/TAMD.2010.2051436) | IEEE TAMD 2010 | Not found |
| Eureka | [Human-Level Reward Design via Coding Large Language Models](https://openreview.net/forum?id=IEduRUO55F) | ICLR 2024 | [eureka-research/Eureka](https://github.com/eureka-research/Eureka) |
| DrEureka | [Language Model Guided Sim-to-Real Transfer](https://arxiv.org/abs/2406.01967) | RSS 2024 | [eureka-research/dreureka](https://github.com/eureka-research/dreureka) |
| ROSKA | [Efficient Language-Instructed Skill Acquisition via Reward-Policy Co-Evolution](https://arxiv.org/abs/2412.13492) | AAAI 2025 | Not found |
| R* | [R*: Efficient Reward Design via Reward Structure Evolution and Parameter Alignment Optimization with Large Language Models](https://openreview.net/forum?id=qZMLrURRr9) | ICML 2025 | Not found |
| LaRes | [LaRes: Evolutionary Reinforcement Learning with LLM-Based Adaptive Reward Search](https://openreview.net/forum?id=jRjvcqtdtA) | NeurIPS 2025 | [yeshenpy/LaRes](https://github.com/yeshenpy/LaRes) |
| LERO | [LERO: LLM-Driven Evolutionary Framework with Hybrid Rewards and Enhanced Observation for Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2503.21807) | ICIC 2025 | Not found |
| ReMAC | [ReMAC: Large Language Model-Driven Reward Design for Multi-Agent Manipulation Collaboration](https://openreview.net/forum?id=CWYWhLho0a) | NeurIPS Workshop 2025 | [Project](https://remac-manicraft.github.io/) |

## Morphological Evolution

| Method | Paper | Venue | Code |
|---|---|---|---|
| EvoGym | [Evolution Gym: A Large-Scale Benchmark for Evolving Soft Robots](https://arxiv.org/abs/2201.09863) | NeurIPS 2021 | [EvolutionGym/evogym](https://github.com/EvolutionGym/evogym) |
| HERD | [Leveraging Hyperbolic Embeddings for Coarse-to-Fine Robot Design](https://arxiv.org/abs/2311.00462) | ICLR 2024 | [drdh/HERD](https://github.com/drdh/HERD) |
| AIEA | [Rapidly Evolving Soft Robots via Action Inheritance](https://doi.org/10.1109/TEVC.2023.3327459) | IEEE TEVC 2024 | [HandingWangXDGroup/AIEA](https://github.com/HandingWangXDGroup/AIEA) |
| DERL | [Embodied Intelligence via Learning and Evolution](https://arxiv.org/abs/2102.02202) | Nature Communications 2021 | [agrimgupta92/derl](https://github.com/agrimgupta92/derl) |
| TAME | [Task-Agnostic Morphology Evolution](https://arxiv.org/abs/2102.13100) | ICLR 2021 | [jhejna/morphology-opt](https://github.com/jhejna/morphology-opt) |
| Encoding study | [How the Morphology Encoding Influences the Learning Ability in Body-Brain Co-Optimization](https://doi.org/10.1145/3583131.3590429) | GECCO 2023 | Not found |

## Interpretable AI

| Method | Paper | Venue | Code |
|---|---|---|---|
| POC-NLDT | [Toward Interpretable-AI Policies Using Evolutionary Nonlinear Decision Trees for Discrete Action Systems](https://ieeexplore.ieee.org/document/9805655) | IEEE TCYB 2024 | [yddhebar/NLDT](https://github.com/yddhebar/NLDT) |
| GE-QL / CG-DT | [Interpretable AI for Policy-Making in Pandemics](https://arxiv.org/abs/2204.04256) | GECCO 2022 | Not found |
| CC-POC | [A Co-Evolutionary Approach to Interpretable RL in Environments with Continuous Action Spaces](https://doi.org/10.1109/SSCI50451.2021.9660048) | SSCI 2021 | Not found |
| QD-GT | [Quality Diversity Evolutionary Learning of Decision Trees](https://arxiv.org/abs/2208.12758) | ACM SAC 2023 | Not found |
| SIRL | [Social Interpretable Reinforcement Learning](https://doi.org/10.1007/978-3-031-90065-5_1) | EvoApplications 2025 | Not found |
| SVI | [Symbolic Regression Methods for Reinforcement Learning](https://arxiv.org/abs/1903.09688) | IEEE Access 2021 | Not found |

## Learning Classifier Systems

| Method | Paper | Venue | Code |
|---|---|---|---|
| XCS | [Classifier Fitness Based on Accuracy](https://doi.org/10.1162/evco.1995.3.2.149) | Evolutionary Computation 1995 | [community implementation](https://github.com/hosford42/xcs) |
| XCSG / XCSRG | [Gradient Descent Methods in Learning Classifier Systems: Improving XCS Performance in Multistep Problems](https://doi.org/10.1109/TEVC.2005.850265) | IEEE TEVC 2005 | Not found |
| XCSF | [Classifiers That Approximate Functions](https://link.springer.com/article/10.1023/A:1016535925043) | Natural Computing 2002 | Not found |
| XCSF with tile coding | [XCSF with Tile Coding in Discontinuous Action-Value Landscapes](https://link.springer.com/article/10.1007/s12065-015-0129-7) | Evolutionary Intelligence 2015 | Not found |
| DGP-XCSF | [Dynamical Genetic Programming in XCSF](https://doi.org/10.1162/EVCO_a_00080) | Evolutionary Computation 2013 | Not found |

# Frameworks, benchmarks, and tooling

| Resource | Scope | Paper | Code |
|---|---|---|---|
| EvoRL | GPU-accelerated ERL, EC, AutoRL, and RL workflows in JAX | [EvoRL: A GPU-Accelerated Framework for ERL](https://doi.org/10.1145/3750053), ACM TELO 2025 | [EMI-Group/evorl](https://github.com/EMI-Group/evorl) |
| EvoX | Distributed GPU-accelerated evolutionary computation | [Documentation](https://evox.readthedocs.io/) | [EMI-Group/evox](https://github.com/EMI-Group/evox) |
| QDax | Quality-Diversity and neuroevolution in JAX | [QDax](https://arxiv.org/abs/2308.03665) | [adaptive-intelligent-robotics/QDax](https://github.com/adaptive-intelligent-robotics/QDax) |
| QD skill discovery | Comparing neuroevolution and RL for skill discovery | [Paper](https://openreview.net/forum?id=6BHlZgyPOZY) | [instadeepai/qd-skill-discovery-benchmark](https://github.com/instadeepai/qd-skill-discovery-benchmark) |
| EvoGym | Co-design benchmark for soft robots | [Paper](https://arxiv.org/abs/2201.09863) | [EvolutionGym/evogym](https://github.com/EvolutionGym/evogym) |

# Recent and emerging directions

Accepted papers are separated from preprints and active submissions.

## Published or accepted

- **ERLAP** - [Evolutionary Reinforcement Learning with Parameterized Action Primitives for Diverse Manipulation Tasks](https://ojs.aaai.org/index.php/AAAI/article/view/33606), AAAI 2025.
- **CORE** - [CORE: Collaborative Optimization with Reinforcement Learning and Evolutionary Algorithm for Floorplanning](https://papers.neurips.cc/paper_files/paper/2025/hash/cc0f00fd7c873fe2b196529e19b1a6bf-Abstract-Conference.html), NeurIPS 2025, [code](https://github.com/yeshenpy/CORE).
- **LaRes** - [LaRes: Evolutionary Reinforcement Learning with LLM-Based Adaptive Reward Search](https://openreview.net/forum?id=jRjvcqtdtA), NeurIPS 2025, [code](https://github.com/yeshenpy/LaRes).
- **Nevo-CRL** - [Neuro-Evolutionary Continual Reinforcement Learning](https://openreview.net/forum?id=Hv0jK8xYcT), ICML 2026 Spotlight, [code](https://github.com/yeshenpy/Nevo-CRL).
- **HELIX** - [Evolutionary Reinforcement Learning for Open-Ended Scientific Problem Solving](https://openreview.net/forum?id=2CHz6NYBmd), ICLR 2026.
- **JEDi** - [Quality with Just Enough Diversity in Evolutionary Policy Search](https://doi.org/10.1145/3638529.3654047), GECCO 2024, pages 105-113.

## Preprints and watchlist

- **Differentiable Evolutionary Reinforcement Learning** - [arXiv:2512.13399](https://arxiv.org/abs/2512.13399), [code](https://github.com/sitaocheng/DERL). Status: preprint.
- **Lifelong Control through Neuro-Evolution** - [OpenReview](https://openreview.net/forum?id=7CHE4RZYNm). Status: submitted work.

# Related surveys

- [Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey on Hybrid Algorithms](https://arxiv.org/abs/2401.11963)
- [Evolutionary Reinforcement Learning: A Survey](https://arxiv.org/abs/2303.04150)
- [Reinforcement Learning-Assisted Evolutionary Algorithm: A Survey and Research Opportunities](https://arxiv.org/abs/2308.13420)
- [Combining Evolution and Deep Reinforcement Learning for Policy Search: A Survey](https://arxiv.org/abs/2203.14009)

# Contributing

Please open an issue or pull request with:

1. the paper title and BibTeX;
2. an official paper URL (publisher, proceedings, arXiv, or OpenReview);
3. an author-maintained code URL, if available;
4. one taxonomy branch from this README;
5. one or two sentences explaining the EA-RL interaction.

To keep the list reliable, unofficial mirrors, generic search pages, and paper pages mislabeled as code will not be added.

# Citation

```bibtex
@article{li2025bridging,
  author  = {Pengyi Li and Jianye Hao and Hongyao Tang and Xian Fu and Yan Zheng and Ke Tang},
  title   = {Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey on Hybrid Algorithms},
  journal = {IEEE Transactions on Evolutionary Computation},
  year    = {2025},
  volume  = {29},
  number  = {5},
  pages   = {1707--1728},
  doi     = {10.1109/TEVC.2024.3443913}
}
```
