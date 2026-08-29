# ERL Reading Guides

A bilingual, work-by-work guide to explanatory material for the papers and methods in [Awesome Evolutionary Reinforcement Learning](README.md). This repository is the official companion to [*Bridging Evolutionary Algorithms and Reinforcement Learning: A Comprehensive Survey on Hybrid Algorithms*](https://arxiv.org/abs/2401.11963).

> [!IMPORTANT]
> This guide separates **Core** explanations from **Extended** material. Core entries provide a substantial, work-specific explanation. Extended entries include focused overview sections, project documentation, broader thesis chapters, posters, and talk slides.

**Coverage after independent search and citation review (30 Aug 2026):** 270 canonical works reviewed · **54** works with at least one verified explanation · **27** with Chinese material · **45** with English material · **86** verified work-link mappings across **80** unique URLs.

`—` means that no reliable work-specific explanation passed review. It does not mean the paper or code is unavailable.

[Back to the main collection](README.md)

## Field overview

- [一篇演化强化混合算法综述——一个潜力巨大的研究领域](https://zhuanlan.zhihu.com/p/707204855) · 知乎·李鹏翼（作者自有账号）
- [演化强化学习算法最全 Survey——三大方向、十多个研究分支](https://zhuanlan.zhihu.com/p/679367395) · 知乎·李鹏翼（作者自有账号）

## EA-assisted Optimization of RL

### EA-assisted Parameter Search

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **EQ** | [Paper](https://direct.mit.edu/isal/proceedings/isal2020/32/441/98464) | — | — |
| **Supe-RL** | [Paper](https://openreview.net/forum?id=TGFO0DbD_pk) | *Extended* · [EvoRainbow：演化强化学习策略搜索的集大成者](https://zhuanlan.zhihu.com/p/704285528) · <sub>Overview section</sub> | **Core** · [Enhancing Exploration and Safety in Deep Reinforcement Learning](https://iris.univr.it/handle/11562/1058335) · <sub>Author thesis</sub> · <sub>Chapter 7: Genetic Soft Updates for Policy Evolution</sub> |
| **VFS** | [Paper](https://openreview.net/forum?id=6qZC7pfenQm) | — | — |

### EA-assisted Action Selection

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **Qt-Opt** | [Paper](https://proceedings.mlr.press/v87/kalashnikov18a.html) | **Core** · [机器人如何获得能够有效泛化到各种现实世界物体和环境的技能？](https://spsg.gymf.com.cn/newslist/industrynews/36513) · <sub>Research news</sub> | **Core** · [Scalable Deep Reinforcement Learning for Robotic Manipulation](https://research.google/blog/scalable-deep-reinforcement-learning-for-robotic-manipulation/) · <sub>Author article</sub> |
| **CGP** | [Paper](https://arxiv.org/abs/1903.10605) | — | — |
| **EAS-RL** | [Paper](https://doi.org/10.1007/978-3-031-30111-7_49) | — | — |
| **SAC-CEPO** | [Paper](https://arxiv.org/abs/2112.11115) | — | — |
| **GRAC** | [Paper](https://arxiv.org/abs/2009.08973) | — | *Extended* · [Self-Guided and Self-Regularized Actor-Critic (GRAC)](https://github.com/stanford-iprl-lab/GRAC) · <sub>Project / docs</sub> |
| **OMAR** | [Paper](https://arxiv.org/abs/2111.11188) | — | — |
| **COMIX** | [Paper](https://arxiv.org/abs/2003.06709v1) | — | — |
| **NichGP-DRL** | [Paper](https://doi.org/10.1109/TEVC.2024.3395699) | — | — |
| **ERL-A2S** | [Paper](https://doi.org/10.1016/j.ins.2024.120804) | — | — |
| **QD-ASE** | [Paper](https://doi.org/10.1109/IJCNN64981.2025.11228248) | — | — |
| **ERL-MPP** | [Paper](https://doi.org/10.1609/aaai.v39i7.32748) | — | — |

### Hyperparameter Optimization

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **OMPAC** | [Paper](https://arxiv.org/abs/1702.07490) | — | — |
| **PBT** | [Paper](https://arxiv.org/abs/1711.09846) | **Core** · [《Population Based Training of Neural Networks》论文解读](https://www.cnblogs.com/initial-h/p/10519150.html) · <sub>Technical article</sub><br>**Core** · [前沿 \| DeepMind提出新型超参数最优化方法：性能超越手动调参和贝叶斯优化](https://cloud.tencent.com/developer/article/1120056) · <sub>Research news</sub> | **Core** · [Population Based Training of Neural Networks](https://deepmind.google/blog/population-based-training-of-neural-networks/) · <sub>Author article</sub><br>*Extended* · [A Guide to Population Based Training with Tune](https://docs.ray.io/en/latest/tune/examples/pbt_guide.html) · <sub>Documentation</sub> |
| **SEARL** | [Paper](https://arxiv.org/abs/2009.01555) | — | *Extended* · [Sample-Efficient Automated Deep Reinforcement Learning](https://github.com/automl/SEARL) · <sub>Project / docs</sub> |
| **GA-DRL** | [Paper](https://arxiv.org/abs/2203.00141) | — | — |
| **AAC** | [Paper](https://arxiv.org/abs/2106.08918) | — | — |
| **OHT-ES** | [Paper](https://arxiv.org/abs/2006.07554) | — | — |
| **Adaptive HPO-ERL** | [Paper](https://link.springer.com/article/10.1007/s10846-024-02138-8) | — | — |
| **BiERL** | [Paper](https://doi.org/10.3233/FAIA230551) | — | — |
| **Evolved Meta-Parameters** | [Paper](https://doi.org/10.1109/IROS.2003.1250664) | — | — |

### Algorithm and Update-rule Discovery

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **DQNClipped / DQNReg** | [Paper](https://arxiv.org/abs/2101.03958) | — | **Core** · [Evolving Reinforcement Learning Algorithms](https://research.google/blog/evolving-reinforcement-learning-algorithms/) · <sub>Author article</sub><br>**Core** · [Implementing DQNClipped and DQNReg with Stable Baselines](https://medium.com/aureliantactics/implementing-dqnclipped-and-dqnreg-with-stable-baselines-4e3f02160466) · <sub>Technical article</sub> |
| **LPO** | [Paper](https://arxiv.org/abs/2210.05639) | *Extended* · [切换JAX，强化学习速度提升4000倍，牛津大学开源框架PureJaxRL，训练只需GPU](https://www.36kr.com/p/2214990783558275) · <sub>Overview section</sub> | — |
| **TA-LPG / TA-LPO** | [Paper](https://arxiv.org/abs/2402.05828) | — | — |
| **LLM RL Algorithm Discovery** | [Paper](https://arxiv.org/abs/2603.28416) | — | — |
| **LLM Multiagent Algorithm Discovery** | [Paper](https://arxiv.org/abs/2602.16928) | — | — |
| **EPG** | [Paper](https://papers.nips.cc/paper/2018/hash/7876acb66640bad41f1e1371ef30c180-Abstract.html) | — | — |

### Other EA-assisted RL methods

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **GP-MAXQ** | [Paper](https://faculty.cc.gatech.edu/~hic/hic-papers/04141056.pdf) | — | *Extended* · [Embodied Evolution of Learning Ability — evolutionary development of hierarchical learning structures](https://www.csc.kth.se/utbildning/forskar/avhandlingar/doktor/2007/ElfwingStefan.pdf) · <sub>Author thesis</sub> |
| **PNS-RL** | [Paper](https://arxiv.org/abs/1811.10264) | — | — |
| **Go-Explore** | [Paper](https://arxiv.org/abs/1901.10995) | **Core** · [[论文] Go-Explore](https://zhkmxx9302013.github.io/2019-04-20_%E8%AE%BA%E6%96%87GoExplore.html) · <sub>Technical article</sub><br>**Core** · [First return, then explore.](https://ldy-php.mysxl.cn/blog/first-return-then-explore) · <sub>Technical article</sub> | **Core** · [Montezuma’s Revenge Solved by Go-Explore, a New Algorithm for Hard-Exploration Problems (Sets Records on Pitfall, Too)](https://www.uber.com/mo/en/blog/go-explore/) · <sub>Author article</sub><br>*Extended* · [Exploration Strategies in Deep Reinforcement Learning](https://lilianweng.github.io/posts/2020-06-07-exploration-drl/) · <sub>Overview section</sub> |
| **G2N** | [Paper](https://arxiv.org/abs/1903.01886) | — | — |
| **EVO-RL** | [Paper](https://arxiv.org/abs/2007.04725) | — | — |
| **ROMANCE** | [Paper](https://arxiv.org/abs/2305.05909) | — | — |
| **MA3C** | [Paper](https://doi.org/10.1007/s11704-023-2733-5) | *Extended* · [FCS 文章精要：南京大学俞扬教授团队——基于可适应多智能体辅助对抗生成的鲁棒性多智能体通信算法](https://paper.sciencenet.cn/htmlpaper/2024/9/2024929131546688121562.shtm) · <sub>Research news</sub> | — |
| **EPC** | [Paper](https://arxiv.org/abs/2003.10423) | — | *Extended* · [Evolutionary Population Curriculum for Scaling Multi-Agent Reinforcement Learning (thesis)](https://publications.ri.cmu.edu/storage/publications/2020/05/Qian_Long_thesis.pdf) · <sub>Thesis / lecture</sub> |
| **MAPPER** | [Paper](https://arxiv.org/abs/2007.15724) | *Extended* · [多智能体路径规划技术研究综述](https://journal.bjut.edu.cn/bjgydxxb/article/doi/10.11936/bjutxb2023020021) · <sub>Overview section</sub> | — |
| **EvIL** | [Paper](https://arxiv.org/abs/2406.11905) | — | *Extended* · [EvIL: Evolution Strategies for Generalisable Imitation Learning](https://github.com/SilviaSapora/evil) · <sub>Project / docs</sub> |
| **Behaviour Distillation (HaDES)** | [Paper](https://iclr.cc/virtual/2024/poster/17711) | — | — |
| **Adversarial Cheap Talk (ACT)** | [Paper](https://proceedings.mlr.press/v202/lu23h.html) | — | — |
| **GP Offline Data** | [Paper](https://doi.org/10.1016/j.swevo.2025.102140) | — | — |
| **EDT Curriculum Goals** | [Paper](https://doi.org/10.1007/978-3-031-56855-8_1) | — | — |
| **GA Offline Dataset Reduction** | [Paper](https://doi.org/10.1145/3712256.3726364) | — | — |
| **AEIRL** | [Paper](https://doi.org/10.1016/j.neucom.2026.133327) | — | — |
| **ES-KD-MARL** | [Paper](https://doi.org/10.3390/math13172734) | — | — |
| **E2CL** | [Paper](https://doi.org/10.1007/s44443-025-00215-y) | — | — |

## RL-assisted Optimization of EA

### Population Initialization

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **NGGP** | [Paper](https://arxiv.org/abs/2111.00053) | — | *Extended* · [Deep Symbolic Optimization](https://github.com/dso-org/deep-symbolic-optimization) · <sub>Project / docs</sub> |
| **RL-guided GA** | [Paper](https://doi.org/10.1016/j.knosys.2021.106836) | — | — |
| **DeepACO** | [Paper](https://arxiv.org/abs/2309.14032) | **Core** · [DeepACO Neural-enhanced Ant Systems for Combinatorial Optimization](https://birdie-go.github.io/2024/01/20/DeepACO-Neural-enhanced-Ant-Systems-for-Combinatorial-Optimization/) · <sub>Technical article</sub><br>**Core** · [〖论文笔记〗DeepACO Neural-enhanced Ant Systems for Combinatorial Optimization](https://peterliuzhi.top/posts/%E8%AE%BA%E6%96%87%E7%AC%94%E8%AE%B0/%E8%AE%BA%E6%96%87%E7%AC%94%E8%AE%B0deepaco-neural-enhanced-ant-systems-for-combinatorial-optimization/) · <sub>Technical article</sub> | *Extended* · [DeepACO: Neural-enhanced Ant Systems for Combinatorial Optimization](https://github.com/henry-yeh/DeepACO) · <sub>Project / docs</sub> |

### Population Evaluation

This branch contains six primary RL-assisted evaluation works. SC and PGPS are listed once under [Single-Agent Optimization](#single-agent-optimization), and ERL-Re2 is listed once under [Representation and Search Decomposition](#representation-and-search-decomposition); their guide mappings are not duplicated here.

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **Policy Embedding Surrogate ERL** | [Paper](https://doi.org/10.1007/978-981-99-1549-1_19) | — | — |
| **Neuroevolution Surrogates** | [Paper](https://doi.org/10.1145/3321707.3321829) | — | — |
| **Policy Racing** | [Paper](https://doi.org/10.1145/1553374.1553426) | — | — |
| **Efficient ERL Evaluation** | [Paper](https://doi.org/10.1007/978-3-031-13870-6_4) | — | — |
| **Hybrid SA-EMORL** | [Paper](https://doi.org/10.1007/978-3-031-56855-8_4) | — | — |
| **SA-EMARL** | [Paper](https://doi.org/10.1145/3795095.3805146) | — | — |
| **DRL-SMM** | [Paper](https://doi.org/10.1016/j.swevo.2024.101817) | — | — |


### Variation Operator

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **GPO** | [Paper](https://arxiv.org/abs/1711.01012) | — | *Extended* · [Policy Optimization by Genetic Distillation](https://tgangwani.github.io/data/GPO_poster.pdf) · <sub>Author poster</sub> |
| **CEM-RL** | [Paper](https://arxiv.org/abs/1810.01222) | *Extended* · [EvoRainbow：演化强化学习策略搜索的集大成者](https://zhuanlan.zhihu.com/p/704285528) · <sub>Overview section</sub> | *Extended* · [Evolution Strategies — CEM-RL](https://lilianweng.github.io/posts/2019-09-05-evolution-strategies/) · <sub>Overview section</sub> |
| **CEM-ACER** | [Paper](https://dl.acm.org/doi/10.5555/3463952.3464104) | — | — |
| **PBRL** | [Paper](https://ieeexplore.ieee.org/document/9660084) | — | — |
| **DEPRL** | [Paper](https://doi.org/10.1155/2021/5300189) | — | — |
| **Wuji** | [Paper](https://doi.org/10.1109/ASE.2019.00077) | **Core** · [获顶会最佳论文，天津大学等用强化学习寻找游戏bug](https://cloud.tencent.com/developer/article/1527015) · <sub>Research news</sub> | — |
| **PE-DRL** | [Paper](https://doi.org/10.1145/3583131.3590455) | — | — |
| **EDA-PG** | [Paper](https://doi.org/10.1109/CEC60901.2024.10611765) | — | — |

### Quality-Diversity

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **NS-RL** | [Paper](https://ieeexplore.ieee.org/document/9139203) | *Extended* · [在线深度强化学习探索策略生成方法综述](https://robot.sia.cn/article/doi/10.13973/j.cnki.robot.230252) · <sub>Overview section</sub> | — |
| **QD-PG** | [Paper](https://doi.org/10.1145/3512290.3528845) | *Extended* · [在线深度强化学习探索策略生成方法综述](https://robot.sia.cn/article/doi/10.13973/j.cnki.robot.230252) · <sub>Overview section</sub> | — |
| **PGA-ME** | [Paper](https://doi.org/10.1145/3449639.3459304) | — | *Extended* · [Optimizing with PGAME in JAX](https://qdax.readthedocs.io/en/latest/examples/pgame/) · <sub>Documentation</sub> |
| **GAC QD-RL** | [Paper](https://arxiv.org/abs/2303.06164) | — | — |
| **CMA-MEGA** | [Paper](https://arxiv.org/abs/2202.03666) | — | *Extended* · [Approximating Gradients for Differentiable Quality Diversity in Reinforcement Learning](https://dqd-rl.github.io/) · <sub>Project / docs</sub><br>*Extended* · [Differentiable Quality Diversity in Reinforcement Learning (GECCO slides)](https://slides.btjanaka.net/dqd-rl-gecco/) · <sub>Thesis / lecture</sub> |
| **CCQD** | [Paper](https://openreview.net/forum?id=JDud6zbpFv) | — | — |
| **RefQD** | [Paper](https://arxiv.org/abs/2406.03731) | — | *Extended* · [RefQD: Reference-based Quality Diversity](https://github.com/lamda-bbo/RefQD) · <sub>Project / docs</sub> |
| **QDHUAC** | [Paper](https://arxiv.org/abs/2604.20381) | — | — |
| **EDOCS** | [Paper](https://openreview.net/forum?id=74x5BXs4bWD) | — | — |
| **DvD** | [Paper](https://papers.nips.cc/paper_files/paper/2020/hash/d1dc3a8270a6f9394f88847d7f0050cf-Abstract.html) | — | — |
| **QD-Sim** | [Paper](https://openreview.net/forum?id=bLmSMXbqXr) | — | — |
| **NS-ES** | [Paper](https://papers.nips.cc/paper_files/paper/2018/hash/b1301141feffabac455e1f90a7de2054-Abstract.html) | — | — |
| **CCNCS-ERL** | [Paper](https://doi.org/10.1016/j.swevo.2021.100974) | — | — |
| **DBBD-ERL** | [Paper](https://doi.org/10.1016/j.swevo.2025.102241) | — | — |
| **QDRL-BRPG** | [Paper](https://doi.org/10.1145/3834777) | — | — |

### Dynamic Operator Selection

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **RL-GA(a)** | [Paper](https://dl.acm.org/doi/10.5555/2955491.2955607) | — | — |
| **RLEP** | [Paper](https://doi.org/10.1016/j.ins.2007.09.026) | — | — |
| **EA+RL** | [Paper](https://doi.org/10.1109/ICMLA.2012.32) | — | — |
| **EA+RL(O)** | [Paper](https://doi.org/10.1145/2598394.2605681) | — | — |
| **RL-GA(b)** | [Paper](https://doi.org/10.1016/j.swevo.2023.101236) | — | — |
| **GSF** | [Paper](https://doi.org/10.1109/TEVC.2022.3197298) | — | — |
| **MARLwCMA** | [Paper](https://doi.org/10.1109/ACCESS.2020.3033593) | — | — |
| **MPSORL** | [Paper](https://doi.org/10.3934/mbe.2023373) | — | — |
| **DEDQN** | [Paper](https://doi.org/10.1016/j.asoc.2021.107678) | — | — |
| **DE-DDQN** | [Paper](https://doi.org/10.1145/3321707.3321813) | — | — |
| **RL-CORCO** | [Paper](https://doi.org/10.1016/j.knosys.2021.107731) | — | — |
| **RL-HDE** | [Paper](https://doi.org/10.1016/j.swevo.2023.101351) | — | — |
| **DE-RLFR** | [Paper](https://doi.org/10.1016/j.swevo.2019.06.010) | — | — |
| **LRMODE** | [Paper](https://doi.org/10.1016/j.asoc.2020.106693) | — | — |
| **MOEA/D-DQN** | [Paper](https://doi.org/10.1109/TETCI.2022.3146882) | — | — |
| **AMODE-DRL** | [Paper](https://doi.org/10.1109/TASE.2023.3244331) | — | — |
| **DRL-AEOSF** | [Paper](https://doi.org/10.1016/j.swevo.2026.102453) | — | — |
| **DRL-EMS** | [Paper](https://doi.org/10.1145/3795095.3805102) | — | — |
| **DRL-MM-MOEA** | [Paper](https://doi.org/10.1016/j.eswa.2025.129581) | — | — |
| **RL-HH-OES** | [Paper](https://doi.org/10.1007/s10489-026-07279-x) | — | — |
| **AOS-RL** | [Paper](https://doi.org/10.1016/j.ins.2021.10.025) | — | — |
| **OVEA** | [Paper](https://doi.org/10.1016/j.swevo.2022.101225) | — | — |
| **RLDMDE** | [Paper](https://doi.org/10.1007/s40747-023-01243-9) | — | — |
| **RL-AOS Runtime** | [Paper](https://doi.org/10.1007/s10489-025-06687-9) | — | — |
| **GEA-AOS** | [Paper](https://doi.org/10.1080/17445760.2025.2605297) | — | — |
| **TL-AOS** | [Paper](https://doi.org/10.3390/a15010024) | — | — |
| **CEDE-DRL** | [Paper](https://doi.org/10.1016/j.swevo.2023.101387) | — | — |
| **DRL-AOS-CMO** | [Paper](https://doi.org/10.1109/JAS.2023.123687) | — | — |
| **RL-CMTO** | [Paper](https://doi.org/10.1016/j.ins.2024.120863) | — | — |
| **DRL-AOP** | [Paper](https://doi.org/10.1109/TETCI.2026.3670673) | — | — |

### Dynamic Algorithm Configuration

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **AGA** | [Paper](https://link.springer.com/chapter/10.1007/978-3-540-69868-5_10) | — | — |
| **LTO** | [Paper](https://ml.informatik.uni-freiburg.de/wp-content/uploads/papers/20-PPSN-LTO-CMA.pdf) | — | *Extended* · [LTO-CMA](https://github.com/automl/LTO-CMA) · <sub>Project / docs</sub> |
| **RL-DAC** | [Paper](https://doi.org/10.3233/FAIA200122) | — | *Extended* · [Dynamic Algorithm Configuration — A Short Overview](https://automl.github.io/DACBench/main/source/dac.html) · <sub>Documentation</sub> |
| **REM** | [Paper](https://doi.org/10.1109/TETCI.2022.3221483) | — | — |
| **MADAC** | [Paper](https://arxiv.org/abs/2210.06835) | — | *Extended* · [Multi-Agent DAC](https://automl.github.io/DACBench/main/source/multi_agent_dac.html) · <sub>Documentation</sub> |
| **Q-LSHADE & DQ-HSES** | [Paper](https://ieeexplore.ieee.org/document/10035716) | — | — |
| **qlDE** | [Paper](https://doi.org/10.1016/j.asoc.2021.107464) | — | — |
| **RLDE** | [Paper](https://doi.org/10.1016/j.egyr.2021.01.096) | — | — |
| **GS-DAC** | [Paper](https://proceedings.mlr.press/v267/reijnen25a.html) | — | — |
| **ERLA-HBS** | [Paper](https://doi.org/10.1016/j.eswa.2024.123937) | — | — |
| **ConfigX** | [Paper](https://doi.org/10.1609/aaai.v39i25.34904) | — | — |
| **DRL-EA-CMO** | [Paper](https://doi.org/10.1109/TCYB.2025.3603251) | — | — |
| **RL-MS-ECMO** | [Paper](https://doi.org/10.1145/3764597) | — | — |
| **AC-RL-MMO** | [Paper](https://doi.org/10.1109/TNNLS.2025.3624785) | — | — |
| **RL-MMOF** | [Paper](https://doi.org/10.1016/j.asoc.2025.114318) | — | — |
| **RL-EA Helicopter** | [Paper](https://doi.org/10.1016/j.swevo.2026.102437) | — | — |
| **SuperDE** | [Paper](https://doi.org/10.1109/TEVC.2026.3700208) | — | — |
| **MetaMTO** | [Paper](https://doi.org/10.1109/TEVC.2026.3707341) | — | — |
| **LDE** | [Paper](https://doi.org/10.1109/TEVC.2021.3060811) | — | — |
| **RL-HPSDE** | [Paper](https://doi.org/10.1016/j.swevo.2022.101194) | — | — |
| **RLDE-AFL** | [Paper](https://doi.org/10.1145/3712256.3726309) | — | — |
| **RLDE-PFR** | [Paper](https://doi.org/10.1016/j.engappai.2026.114424) | — | — |
| **RL-PC-MOEA/D** | [Paper](https://doi.org/10.1007/s13748-018-0155-7) | — | — |
| **RL-AMH** | [Paper](https://doi.org/10.1145/3520304.3533983) | — | — |
| **RL-OGPA** | [Paper](https://doi.org/10.1016/j.swevo.2023.101371) | — | — |
| **DRL-DAS** | [Paper](https://doi.org/10.1109/TSMC.2024.3374889) | — | — |
| **DRL-PC-MOEC** | [Paper](https://doi.org/10.1155/2024/6740701) | — | — |
| **KB-HPA-DE** | [Paper](https://doi.org/10.1016/j.neucom.2025.130633) | — | — |
| **RLCDE-LBFGS** | [Paper](https://doi.org/10.1371/journal.pone.0347860) | — | — |

### Dynamic Resource Allocation

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **RLDE-ARA** | [Paper](https://www.sciencedirect.com/science/article/pii/S221065022500046X) | — | — |
| **DRL Multi-Restart CMA-ES** | [Paper](https://doi.org/10.1111/itor.70215) | — | — |

### Other RL-assisted EA methods

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **Grad-CEM** | [Paper](https://proceedings.mlr.press/v120/bharadhwaj20a.html) | — | — |
| **LOOP** | [Paper](https://arxiv.org/abs/2008.10066) | — | **Core** · [LOOP: Learning Off-Policy with Online Planning](https://blog.ml.cmu.edu/2022/01/07/loop/) · <sub>Author article</sub> |
| **TD-MPC** | [Paper](https://arxiv.org/abs/2203.04955) | **Core** · [TD-MPC：世界模型如何用于机器人控制？](https://worldsensetech.com/zh/articles/td-mpc-world-model-control/) · <sub>Technical article</sub> | *Extended* · [Implicit World Model — TD-MPC](https://leeyngdo.github.io/blog/reinforcement-learning/2024-10-07-implicit-world-model/) · <sub>Overview section</sub><br>*Extended* · [TD-MPC Official Implementation](https://github.com/nicklashansen/tdmpc) · <sub>Project / docs</sub> |
| **RGP** | [Paper](https://doi.org/10.1023/A:1011953410319) | — | — |
| **GNP-RL** | [Paper](https://doi.org/10.1162/evco.2007.15.3.369) | — | — |
| **RL-EAO-MWS** | [Paper](https://doi.org/10.1016/j.swevo.2026.102422) | — | — |
| **SSR-RL-EA** | [Paper](https://linklings.s3.amazonaws.com/organizations/WCCI/wcci2026/submissions/stype102/yBVTd-cec_pap196s2.pdf) | — | — |
| **SparseOp-DRL** | [Paper](https://doi.org/10.1016/j.asoc.2026.115167) | — | — |
| **AutoMH** | [Paper](https://doi.org/10.3390/e24070957) | — | — |
| **RL Acceptance Criteria** | [Paper](https://doi.org/10.1007/s44196-025-00924-2) | — | — |
| **RL-RV-EMO** | [Paper](https://doi.org/10.1109/TEVC.2026.3716135) | — | — |

## Synergistic Optimization of EA and RL

### Single-Agent Optimization

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **ERL** | [Paper](https://arxiv.org/abs/1805.07917) | — | *Extended* · [Evolution + Deep RL — Using Evolution to Optimize Policies](https://master-dac.isir.upmc.fr/rl/evo%2Brl_policies.pdf) · <sub>Thesis / lecture</sub><br>*Extended* · [Evolution-Guided Policy Gradient in Reinforcement Learning](https://github.com/ShawK91/Evolutionary-Reinforcement-Learning) · <sub>Project / docs</sub> |
| **CERL** | [Paper](https://arxiv.org/abs/1905.00976) | — | **Core** · [Greedy AI Agents Learn to Cooperate](https://spectrum.ieee.org/reinforcement-learning) · <sub>Research news</sub> |
| **PDERL** | [Paper](https://arxiv.org/abs/1906.09807) | *Extended* · [EvoRainbow：演化强化学习策略搜索的集大成者](https://zhuanlan.zhihu.com/p/704285528) · <sub>Overview section</sub> | — |
| **SC** | [Paper](https://arxiv.org/abs/2201.00129) | *Extended* · [EvoRainbow：演化强化学习策略搜索的集大成者](https://zhuanlan.zhihu.com/p/704285528) · <sub>Overview section</sub> | *Extended* · [Surrogate-Assisted Evolutionary Reinforcement Learning](https://github.com/Yuxing-Wang-THU/Surrogate-assisted-ERL) · <sub>Project / docs</sub> |
| **GEATL** | [Paper](https://doi.org/10.1145/3449726.3463142) | — | — |
| **CSPS** | [Paper](https://arxiv.org/abs/2011.00791) | — | — |
| **T-ERL** | [Paper](https://doi.org/10.1145/3583131.3590512) | — | — |
| **ESAC** | [Paper](https://www.ifaamas.org/Proceedings/aamas2022/pdfs/p1237.pdf) | — | — |
| **PGPS** | [Paper](https://openreview.net/forum?id=PeT5p3ocagr) | — | — |
| **VEB-RL** | [Paper](https://openreview.net/forum?id=XobPpcN4yZ) | **Core** · [Value Evolution：面向 Value-based RL 的值演化](https://zhuanlan.zhihu.com/p/704412445) · <sub>Author article</sub> | *Extended* · [Value-Evolutionary-Based Reinforcement Learning](https://github.com/yeshenpy/VEB-RL) · <sub>Project / docs</sub> |
| **EvoRainbow** | [Paper](https://openreview.net/forum?id=75Hes6Zse4) | **Core** · [EvoRainbow：演化强化学习策略搜索的集大成者](https://zhuanlan.zhihu.com/p/704285528) · <sub>Author article</sub> | *Extended* · [EvoRainbow: Combining Improvements in Evolutionary Reinforcement Learning for Policy Search](https://github.com/yeshenpy/EvoRainbow) · <sub>Project / docs</sub> |
| **ERL-TD** | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/29289) | — | — |
| **CORE** | [Paper](https://papers.neurips.cc/paper_files/paper/2025/hash/cc0f00fd7c873fe2b196529e19b1a6bf-Abstract-Conference.html) | **Core** · [从问题建模到算法设计：如何利用演化算法与强化学习求解一个带约束的多目标组合优化问题？](https://zhuanlan.zhihu.com/p/2002401573419110595) · <sub>Author article</sub> | *Extended* · [CORE: Collaborative Optimization with Reinforcement Learning and Evolutionary Algorithm for Floorplanning](https://github.com/yeshenpy/CORE) · <sub>Project / docs</sub> |
| **RIM** | [Paper](https://www.sciencedirect.com/science/article/pii/S0020025520311828) | — | — |
| **PES** | [Paper](https://link.springer.com/article/10.1007/s12293-024-00419-1) | — | — |
| **RPSA-RL** | [Paper](https://rpsonline.com.sg/proceedings/cis2023/html/P236.html) | — | — |
| **EIERL** | [Paper](https://aclanthology.org/2025.acl-long.171/) | — | — |
| **Evo-RL for DPDP** | [Paper](https://doi.org/10.1016/j.tre.2026.104885) | — | — |
| **NES-ERL** | [Paper](https://doi.org/10.1016/j.jalgor.2009.04.002) | — | — |
| **Preference Racing** | [Paper](https://doi.org/10.1007/s10994-014-5458-8) | — | — |
| **TRES** | [Paper](https://doi.org/10.1609/aaai.v33i01.33014352) | — | — |
| **AMF-ERL** | [Paper](https://doi.org/10.1109/TEVC.2021.3083362) | — | — |
| **SOS** | [Paper](https://doi.org/10.1609/aaai.v36i7.20737) | — | — |
| **MO-PDERL** | [Paper](https://doi.org/10.1145/3583131.3590441) | — | — |
| **Safety-Informed ERL** | [Paper](https://doi.org/10.2514/1.G008112) | — | — |
| **ERLBioSeq** | [Paper](https://doi.org/10.1609/aaai.v38i1.27792) | — | — |
| **EvOD** | [Paper](https://doi.org/10.1609/aaai.v38i1.27795) | — | — |
| **MO-ERL** | [Paper](https://doi.org/10.1016/j.neucom.2025.129991) | — | — |
| **MCE-ERL** | [Paper](https://doi.org/10.1109/ICNSC66229.2025.00019) | — | — |
| **Hetero-ERL** | [Paper](https://doi.org/10.1016/j.swevo.2026.102353) | — | — |
| **EARL-NCO** | [Paper](https://doi.org/10.1109/TEVC.2026.3696052) | — | — |
| **PD-EPO** | [Paper](https://doi.org/10.1109/ACCESS.2026.3702722) | — | — |
| **LLM-EA-HFSP** | [Paper](https://doi.org/10.1109/TEVC.2026.3658149) | — | — |
| **ERL-WPSS** | [Paper](https://doi.org/10.1016/j.ejor.2026.01.023) | — | — |
| **ERL-ER-FedHG** | [Paper](https://doi.org/10.1016/j.asoc.2025.114436) | — | — |

EvoRainbow and EvoRainbow-Exp are aliases for one canonical paper. CORE has a secondary solution-space/policy-space co-optimization tag and is cross-listed in recent work without being counted again.

### Adaptive, Staged, or Stabilized Coupling

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **BEL** | [Paper](https://proceedings.mlr.press/v205/chen23a.html) | — | — |
| **AERL / AESAC** | [Paper](https://link.springer.com/article/10.1007/s11063-024-11548-6) | — | — |
| **TERL** | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/30079) | — | — |
| **NCG-ERL** | [Paper](https://www.sciencedirect.com/science/article/pii/S2210650224002979) | — | — |
| **GDR** | [Paper](https://doi.org/10.1109/CEC60901.2024.10611871) | — | — |
| **AERL-ET** | [Paper](https://www.ifaamas.org/Proceedings/aamas2024/pdfs/p1947.pdf) | — | — |
| **SERL-OS-EF** | [Paper](https://doi.org/10.1109/TNNLS.2025.3596553) | — | — |
| **GECE-RL** | [Paper](https://doi.org/10.1016/j.neucom.2026.133425) | — | — |
| **Progressive Episodes ES** | [Paper](https://doi.org/10.24963/ijcai.2019/172) | — | — |
| **AES-EM** | [Paper](https://doi.org/10.1016/j.knosys.2022.108624) | — | — |
| **MTNE-LSE** | [Paper](https://doi.org/10.1109/TCDS.2022.3221805) | — | — |
| **GESP** | [Paper](https://doi.org/10.1145/3653024) | — | — |
| **Adaptive Mutation ERL** | [Paper](https://doi.org/10.1109/ACCESS.2024.3493198) | — | — |
| **ACERL-DMH** | [Paper](https://doi.org/10.1109/TNNLS.2025.3582299) | — | — |
| **DG-ERL** | [Paper](https://doi.org/10.1016/j.asoc.2026.116185) | — | — |
| **LCERL** | [Paper](https://doi.org/10.1109/TEVC.2025.3627631) | — | — |
| **Dual-Drive-ERL** | [Paper](https://linklings.s3.amazonaws.com/organizations/WCCI/wcci2026/submissions/stype102/Dd8Jf-cec_pap406s2.pdf) | — | — |

### Representation and Search Decomposition

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **ERL-Re2** | [Paper](https://arxiv.org/abs/2210.17375) | **Core** · [ICLR 2023：融合演化算法与强化学习进行策略搜索的新 SOTA](https://zhuanlan.zhihu.com/p/601231924) · <sub>Author article</sub> | *Extended* · [ERL-Re2: Efficient Evolutionary Reinforcement Learning](https://github.com/yeshenpy/ERL-Re2) · <sub>Project / docs</sub> |
| **CoERL** | [Paper](https://journals.sagepub.com/doi/pdf/10.3233/FAIA240878) | — | — |
| **ERL-CDR** | [Paper](https://link.springer.com/chapter/10.1007/978-981-95-8405-5_30) | — | — |
| **SAR-ERL** | [Paper](https://link.springer.com/article/10.1007/s40747-026-02306-3) | — | — |
| **MO-CoERL** | [Paper](https://doi.org/10.1016/j.ins.2026.123517) | — | — |
| **ER-MRL** | [Paper](https://doi.org/10.1007/978-3-031-56855-8_3) | — | — |
| **EFA** | [Paper](https://www.jmlr.org/papers/v7/whiteson06a.html) | — | — |
| **SE-EFA** | [Paper](https://www.cs.utexas.edu/~pstone/Papers/bib2html/b2hd-AAAI06-shimon.html) | — | — |
| **GP Feature Discovery** | [Paper](https://doi.org/10.1007/978-3-540-78671-9_19) | — | — |
| **CoSyNE** | [Paper](https://www.jmlr.org/papers/v9/gomez08a.html) | — | — |
| **World Models** | [Paper](https://papers.nips.cc/paper/2018/hash/2de5d16682c3c35007e4e92982f1a2ba-Abstract.html) | — | — |
| **Weight-Freezing ERL** | [Paper](https://doi.org/10.1016/j.swevo.2026.102347) | — | — |
| **Co-PDERL** | [Paper](https://doi.org/10.3390/math14061078) | — | — |
| **EE-MORL** | [Paper](https://doi.org/10.1109/TEVC.2026.3673422) | — | — |

### Multi-Agent Optimization

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **MERL** | [Paper](https://arxiv.org/abs/1906.07315) | **Core** · [文献分享 \| 《ICML2020:基于样本效率的多智能体协同进化强化学习》](https://pilab.xmu.edu.cn/info/1258/2657.htm) · <sub>Technical article</sub> | **Core** · [Greedy AI Agents Learn to Cooperate](https://spectrum.ieee.org/reinforcement-learning) · <sub>Research news</sub> |
| **NS-MERL** | [Paper](https://dl.acm.org/doi/10.1145/3583131.3590428) | — | — |
| **CEMARL** | [Paper](https://ieeexplore.ieee.org/document/10191313) | — | — |
| **EMARL** | [Paper](https://link.springer.com/chapter/10.1007/978-3-031-30105-6_23) | — | — |
| **RACE** | [Paper](https://proceedings.mlr.press/v202/li23i.html) | **Core** · [ICML 2023 RACE：首个在复杂任务下展示进化算法能够进一步提升 MARL 的通用混合框架](https://zhuanlan.zhihu.com/p/647913479) · <sub>Author article</sub> | *Extended* · [RACE: Improve Multi-Agent Reinforcement Learning with Representation Asymmetry and Collaborative Evolution](https://icml.cc/media/icml-2023/Slides/23791.pdf) · <sub>Conference poster</sub> |
| **MRPM** | [Paper](https://doi.org/10.1007/s40747-024-01385-4) | — | — |
| **EMARL-UAV** | [Paper](https://doi.org/10.1016/j.knosys.2024.112000) | — | — |
| **MAERL-CG** | [Paper](https://doi.org/10.1109/TETCI.2024.3452119) | — | — |
| **EECG** | [Paper](https://www.ifaamas.org/Proceedings/aamas2025/pdfs/p1623.pdf) | — | — |
| **CCL** | [Paper](https://doi.org/10.1007/978-981-96-9894-3_5) | — | — |
| **GDE** | [Paper](https://doi.org/10.1016/j.neunet.2025.108437) | — | — |
| **ES-MCV Dispatch** | [Paper](https://doi.org/10.1109/TNNLS.2025.3649341) | — | — |

### Reward Design

#### Non-LLM Evolutionary Reward Search

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **Evo-Reward** | [Paper](https://doi.org/10.1109/TAMD.2010.2051436) | — | — |
| **Co-Evolved Shaping Rewards** | [Paper](https://doi.org/10.1177/1059712308092835) | — | — |
| **Evolutionary Intrinsic Motivation** | [Paper](https://doi.org/10.1109/TAMD.2010.2051031) | — | — |
| **GP End-Goal Reward** | [Paper](https://linklings.s3.amazonaws.com/organizations/WCCI/wcci2026/submissions/stype102/nZzyN-cec_pap134s2.pdf) | — | — |

#### LLM-based Reward Program Evolution

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **Eureka** | [Paper](https://openreview.net/forum?id=IEduRUO55F) | **Core** · [Eureka: Human-Level Reward Design via Coding Large Language Models 阅读](https://mathpretty.com/16445.html) · <sub>Technical article</sub><br>**Core** · [GPT-4教会机器手转笔、玩魔方！RL社区震惊：LLM设计奖励竟能超越人类？](https://hub.baai.ac.cn/view/31888) · <sub>Research news</sub> | **Core** · [Eureka! NVIDIA Research Breakthrough Puts New Spin on Robot Learning](https://blogs.nvidia.com/blog/eureka-robotics-research/) · <sub>Research news</sub><br>*Extended* · [Eureka: Human-Level Reward Design via Coding Large Language Models](https://eureka-research.github.io/) · <sub>Project / docs</sub> |
| **DrEureka** | [Paper](https://arxiv.org/abs/2406.01967) | — | *Extended* · [DrEureka: Language Model Guided Sim-to-Real Transfer](https://eureka-research.github.io/dr-eureka/) · <sub>Project / docs</sub> |
| **ROSKA** | [Paper](https://arxiv.org/abs/2412.13492) | **Core** · [提出机器人自主学习新范式，深大团队最新顶会论文，刷新6大复杂任务SOTA](https://m.thepaper.cn/newsDetail_forward_30397998) · <sub>Research news</sub> | — |
| <strong>R*</strong> | [Paper](https://openreview.net/forum?id=qZMLrURRr9) | **Core** · [The reward function is truly all you need.](https://zhuanlan.zhihu.com/p/1920477571004503663) · <sub>Author article</sub> | — |
| **LaRes** | [Paper](https://openreview.net/forum?id=jRjvcqtdtA) | **Core** · [The reward function is truly all you need——样本效率篇](https://zhuanlan.zhihu.com/p/1970185335137862348) · <sub>Author article</sub> | *Extended* · [LaRes: Evolutionary Reinforcement Learning with LLM-Based Adaptive Reward Search](https://github.com/yeshenpy/LaRes) · <sub>Project / docs</sub> |
| **LERO** | [Paper](https://arxiv.org/abs/2503.21807) | — | — |
| **ReMAC** | [Paper](https://openreview.net/forum?id=CWYWhLho0a) | — | *Extended* · [ReMAC: Large Language Model-Driven Reward Design for Multi-Agent Manipulation Collaboration](https://remac-manicraft.github.io/) · <sub>Project / docs</sub> |
| **Physics-LLM Reward Evolution** | [Paper](https://doi.org/10.1109/TEVC.2026.3714198) | — | — |

### Morphological Evolution

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **EvoGym** | [Paper](https://arxiv.org/abs/2201.09863) | **Core** · [[Paper Notes] Evolution Gym: A Large-Scale Benchmark for Evolving Soft Robots](https://davidlxu.github.io/posts/2026/08/evolution-gym-paper-notes/) · <sub>Technical article</sub><br>**Core** · [MIT开发新平台 用算法模拟演变机器人“进化”](https://hub.baai.ac.cn/view/13572) · <sub>Research news</sub> | **Core** · [A system for designing and training intelligent soft robots](https://news.mit.edu/2021/system-designing-training-intelligent-soft-robots-1207) · <sub>Research news</sub><br>*Extended* · [Evolution Gym](https://github.com/EvolutionGym/evogym) · <sub>Project / docs</sub> |
| **HERD** | [Paper](https://arxiv.org/abs/2311.00462) | — | *Extended* · [Leveraging Hyperbolic Embeddings for Coarse-to-Fine Robot Design](https://drdh.cc/assets/pubs/2024-HERD/slides.pdf) · <sub>Author slides</sub> |
| **AIEA** | [Paper](https://doi.org/10.1109/TEVC.2023.3327459) | — | — |
| **DERL** | [Paper](https://arxiv.org/abs/2102.02202) | **Core** · [论文解读：通过学习和进化实现具身智能](https://www.modb.pro/db/379078) · <sub>Research news</sub> | **Core** · [How Bodies Get Smarts: Simulating the Evolution of Embodied Intelligence](https://hai.stanford.edu/news/how-bodies-get-smarts-simulating-evolution-embodied-intelligence) · <sub>Research news</sub><br>*Extended* · [DERL Official Implementation](https://github.com/agrimgupta92/derl) · <sub>Project / docs</sub> |
| **TAME** | [Paper](https://arxiv.org/abs/2102.13100) | — | — |
| **Encoding study** | [Paper](https://doi.org/10.1145/3583131.3590429) | — | *Extended* · [How the Morphology Encoding Influences the Learning Ability in Body-Brain Co-Optimization](https://drive.google.com/file/d/1dSHHQI6W20M9KNP_rPOand3RYNuplkOh/view) · <sub>Author slides</sub> |

### Interpretable AI

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **POC-NLDT** | [Paper](https://ieeexplore.ieee.org/document/9805655) | — | *Extended* · [NLDT: Non Linear Decision Tree — Modelling an Interpretable AI Solution](https://github.com/yddhebar/NLDT) · <sub>Project / docs</sub> |
| **GE-QL / CG-DT** | [Paper](https://arxiv.org/abs/2204.04256) | — | — |
| **CC-POC** | [Paper](https://doi.org/10.1109/SSCI50451.2021.9660048) | — | *Extended* · [Interpretable Reinforcement Learning with Continuous Action Spaces](https://iris.unitn.it/retrieve/bafe6bda-8244-42c6-8fff-6a98994cc61b/phd_unitn_leonardolucio_custode.pdf) · <sub>Thesis / lecture</sub> |
| **QD-GT** | [Paper](https://arxiv.org/abs/2208.12758) | — | — |
| **SIRL** | [Paper](https://doi.org/10.1007/978-3-031-90065-5_1) | — | — |
| **SVI** | [Paper](https://arxiv.org/abs/1903.09688) | — | — |
| **Critic-Moderated Evolution** | [Paper](https://bnaic2024.sites.uu.nl/wp-content/uploads/sites/986/2024/10/Human-readable-programs-as-the-actor-of-a-Reinforcement-Learning-agent-using-critic-moderated-evolution.pdf) | — | — |
| **GP Interpretable Policies** | [Paper](https://doi.org/10.1016/j.engappai.2018.09.007) | — | — |
| **EFS Policy Derivation** | [Paper](https://doi.org/10.1007/s40747-020-00175-y) | — | — |
| **MOERL-Interp** | [Paper](https://doi.org/10.1016/j.asoc.2026.115521) | — | — |
| **ERLER** | [Paper](https://doi.org/10.1016/j.asoc.2025.114380) | — | — |

### Learning Classifier Systems

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **XCS** | [Paper](https://doi.org/10.1162/evco.1995.3.2.149) | — | *Extended* · [XCS Tutorial](https://pythonhosted.org/xcs/) · <sub>Documentation</sub> |
| **XCSG / XCSRG** | [Paper](https://doi.org/10.1109/TEVC.2005.850265) | — | — |
| **XCSF** | [Paper](https://link.springer.com/article/10.1023/A:1016535925043) | — | — |
| **XCSF with tile coding** | [Paper](https://link.springer.com/article/10.1007/s12065-015-0129-7) | — | — |
| **DGP-XCSF** | [Paper](https://doi.org/10.1162/EVCO_a_00080) | — | — |

## Non-canonical tooling and benchmarks

This resource is excluded from the canonical-work, code-first, and guide-coverage counts.

| Resource | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **PBRL GPU Benchmark** | [Paper](https://arxiv.org/abs/2404.03336) | — | — |

## Recent and emerging directions

CORE and LaRes are cross-listed as recent work in the main README but appear only in their primary branches above, so their guide mappings and canonical records are counted once.

### Published or accepted

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **ERLAP** | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/33606) | — | — |
| **Nevo-CRL** | [Paper](https://openreview.net/forum?id=Hv0jK8xYcT) | — | *Extended* · [Neuro-Evolutionary Continual Reinforcement Learning](https://github.com/yeshenpy/Nevo-CRL) · <sub>Project / docs</sub> |
| **HELIX** | [Paper](https://openreview.net/forum?id=2CHz6NYBmd) | — | — |
| **JEDi** | [Paper](https://doi.org/10.1145/3638529.3654047) | — | *Extended* · [Synergies in Evolutionary Search for Connectionist Policies](https://depozit.isae.fr/theses/2024/2024_Templier_Paul_D.pdf) · <sub>Thesis / lecture</sub> |

### Canonical preprints and active submissions

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **Differentiable Evolutionary Reinforcement Learning** | [Paper](https://arxiv.org/abs/2512.13399) | — | *Extended* · [Differentiable Evolutionary Reinforcement Learning](https://github.com/sitaocheng/DERL) · <sub>Project / docs</sub> |
| **Lifelong Control through Neuro-Evolution** | [Paper](https://openreview.net/forum?id=7CHE4RZYNm) | — | — |

### Watchlist (not counted as canonical works)

| Work | Paper | 中文讲解 | English guide |
|---|---|---|---|
| **MEGA** | [Paper](https://arxiv.org/abs/2502.13569) | — | — |
| **Surrogate AE-HNN ERL** | [Paper](https://arxiv.org/abs/2505.19423) | — | — |
| **BASIL** | [Paper](https://arxiv.org/abs/2506.00328) | — | — |
| **E-SPL** | [Paper](https://arxiv.org/abs/2602.14697) | — | — |
| **SV-QD-RL** | [Paper](https://arxiv.org/abs/2606.08735) | — | — |
| **NEOL** | [Paper](https://arxiv.org/abs/2606.20817) | — | — |
| **GERS** | [Paper](https://arxiv.org/abs/2606.16236) | — | — |
| **Developmental Reward Schedules** | [Paper](https://arxiv.org/abs/2606.20858) | — | — |
| **HTSE candidate** | [Paper](https://doi.org/10.1145/3520304.3528937) | — | — |
| **Diverse RL Agents with MAP-Elites** | [Paper](https://arxiv.org/abs/2303.12803) | — | — |
| **Evolving Constrained RL Policy** | [Paper](https://arxiv.org/abs/2304.09869) | — | — |
| **RL-GFM** | [Paper](https://openreview.net/forum?id=EEdobb9oWl) | — | — |
| **HERL** | [Paper](https://doi.org/10.1109/TII.2026.3716821) | — | — |
| **PG-QD Cooperative MARL** | [Paper](https://doi.org/10.1145/3795101.3805338) | — | — |

## Curation policy

- Prefer author, research-lab, university, and reputable technical-publisher explanations.
- Keep overview sections, project pages, theses, posters, and slides under **Extended** rather than presenting them as standalone deep-dive articles.
- Exclude paper landing pages, abstract mirrors, scraped summaries, generic background material, and repository pages that contain only installation commands.
- Do not substitute a later paper for an explanation of the target work, even when the later paper contains a useful related-work section.
- Recheck links before relying on them for teaching or long-term archival use.
