# **A Survey of Task Planning with Large Language Models**
---
<div align="center">

![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Visits Badge](https://badges.pufler.dev/visits/ZhaiWenShuo/Survey-of-Task-Planning)](https://badges.pufler.dev/visits/ZhaiWenShuo/Survey-of-Task-Planning)
![Stars](https://img.shields.io/github/stars/ZhaiWenShuo/Survey-of-Task-Planning)
![Forks](https://img.shields.io/github/forks/ZhaiWenShuo/Survey-of-Task-Planning)
</div>

🏃 **Coming soon**: More related works.

## 🌟 News
✨ [2024/11/24] Creation of this repository to maintain the list of resources on Task Planning based on LLMs. More resoures are coming soon!

## 📜 Contents

  - [🤖 Embodied Artificial Intelligence](#-embodied-artificial-intelligence)
  - [🎮 Game Playing](#-game-playing)
  - [🗺 Economy and Society](#-economy-and-society)
  - [🔗 Citation](#-citation)
  - [🤝 Contact](#-contact)
  
## 🤖 Embodied Artificial Intelligence
- VirtualHome: A Multi-Agent Household Simulator [[paper](https://arxiv.org/abs/1806.07011)] [[blog](http://virtual-home.org/)] [[code](https://github.com/xavierpuigf/virtualhome)]
  - VirtualHome is a multi-agent platform to simulate activities in a household. Agents are represented as humanoid avatars, which can interact with the environment through high-level instructions. You can use VirtualHome to render videos of human activities, or train agents to perform complex tasks. VirtualHome also includes a Knowledge Base, providing instructions to perform a large set of activities.
  - [2023 ICLR'24] Tree-Planner: Efficient Close-loop Task Planning with Large Language Models [[paper](https://arxiv.org/abs/2310.08582)]
  - [2023 NeurIPS] Large Language Models as Commonsense Knowledge for Large-Scale Task Planning [[paper]([[paper](https://arxiv.org/abs/2310.08582)])]
<br>
<div align="center">
<img src="https://github.com/xavierpuigf/virtualhome/blob/master/assets/vh_intro.gif" width="600px">
</div>
<br>

- ALFWorld: Aligning Text and Embodied Environments for Interactive Learning [[paper](https://arxiv.org/abs/2010.03768)] [[blog](https://alfworld.github.io/)] [[code](https://github.com/alfworld/alfworld)]
  - ALFWorld contains interactive TextWorld environments (Côté et. al) that parallel embodied worlds in the ALFRED dataset (Shridhar et. al). The aligned environments allow agents to reason and learn high-level policies in an abstract space before solving embodied tasks through low-level actuation.
<br>
<div align="center">
<img src="https://github.com/alfworld/alfworld/blob/master/media/alfworld_teaser.png" width="600px">
</div>
<br>

- TDW: A Platform for Interactive Multi-Modal Physical Simulation [[paper](https://arxiv.org/abs/2007.04954)] [[blog](https://arxiv.org/abs/2007.04954)] [[code](https://arxiv.org/abs/2007.04954)]
  - ThreeDWorld (TDW) is a platform for interactive multi-modal physical simulation. With TDW, users can simulate high-fidelity sensory data and physical interactions between mobile agents and objects in a wide variety of rich 3D environments.
<br>
<div align="center">
<img src="https://github.com/threedworld-mit/tdw/blob/master/splash.jpg" width="600px">
</div>
<br>

- Isaac Sim: an advanced simulation platform for robotics and AI research [[[blog](https://developer.nvidia.com/isaac/sim)] [[code](https://github.com/isaac-sim)]
  - The NVIDIA Isaac Sim™ robotics developer simulation platform and reference application is designed to help developers design, simulate, test, and train AI-based robots and autonomous machines in a physically based virtual environment.
<br>
<div align="center">
<img src="https://developer.download.nvidia.com/images/isaac-lab-1980x1080.jpg" width="600px">
</div>
<br>

## 🎮 Game Playing
- StarCraft II
  - PySC2 [[code](https://github.com/BurnySc2/python-sc2)] - A StarCraft II API Client for Python 3
  - LLM-PySC2 [[code](https://github.com/NKAI-Decision-Team/LLM-PySC2)] - A LLM StarCraft II Learning Environment
  - Large Language Models Play StarCraft II: Benchmarks and A Chain of Summarization Approach [[paper](https://arxiv.org/abs/2312.11865)] [[code](https://github.com/histmeisah/Large-Language-Models-play-StarCraftII)]
  - SwarmBrain: Embodied agent for real-time strategy game StarCraft II via large language models [[paper](https://arxiv.org/abs/2401.17749)] [[code](https://github.com/ramsayxiaoshao/SwarmBrain)]

<p align="center">
  <img src="https://github.com/NKAI-Decision-Team/LLM-PySC2/blob/master/docs/figures/llm_smac_demo1.gif" width="225">
  <img src="https://github.com/NKAI-Decision-Team/LLM-PySC2/blob/master/docs/figures/llm_smac_demo3.gif" width="225">
  <img src="https://github.com/NKAI-Decision-Team/LLM-PySC2/blob/master/docs/figures/llm_smac_demo2.gif" width="225"><br/>
</p>

- Minecraft
  - Minecraft, as the world's best-selling game, boasts over 238 million copies sold and more than 140 million peak monthly active users. Within the game, hundreds of millions of players have experienced a digital second life by surviving, exploring and creating, closely resembling the human world in many aspects. Minecraft acts as a microcosm of the real world. Developing an automated agent that can master all technical challenges in Minecraft is akin to creating an artificial intelligence capable of autonomously learning and mastering the entire real-world technology.
  - Voyager: An Open-Ended Embodied Agent with Large Language Models [[paper](https://arxiv.org/abs/2305.16291)] [[blog](https://voyager.minedojo.org/)] [[code](https://github.com/MineDojo/Voyager)]
    - We introduce Voyager, the first LLM-powered embodied lifelong learning agent in Minecraft that continuously explores the world, acquires diverse skills, and makes novel discoveries without human intervention. Voyager consists of three key components: 1) an automatic curriculum that maximizes exploration, 2) an ever-growing skill library of executable code for storing and retrieving complex behaviors, and 3) a new iterative prompting mechanism that incorporates environment feedback, execution errors, and self-verification for program improvement. Voyager interacts with GPT-4 via blackbox queries, which bypasses the need for model parameter fine-tuning. The skills developed by Voyager are temporally extended, interpretable, and compositional, which compounds the agent’s abilities rapidly and alleviates catastrophic forgetting. Empirically, Voyager shows strong in-context lifelong learning capability and exhibits exceptional proficiency in playing Minecraft. It obtains 3.3× more unique items, travels 2.3× longer distances, and unlocks key tech tree milestones up to 15.3× faster than prior SOTA. Voyager is able to utilize the learned skill library in a new Minecraft world to solve novel tasks from scratch, while other techniques struggle to generalize.
<br>
<div align="center">
<img src="https://github.com/MineDojo/Voyager/blob/main/images/pull.png" width="600px">
</div>
<br>  
  - Ghost in the Minecraft: Generally Capable Agents for Open-World Environments via Large Language Models with Text-based Knowledge and Memory [[paper](https://arxiv.org/abs/2305.17144)] [[code](https://github.com/OpenGVLab/GITM)]
    - Ghost in the Minecraft (GITM) is a novel framework integrates Large Language Models (LLMs) with text-based knowledge and memory, aiming to create Generally Capable Agents in Minecraft.
<br>
<div align="center">
<img src="https://github.com/OpenGVLab/GITM/blob/main/figs/fig3.png" width="600px">
</div>
<br>  
    

  
- Cradle: Empowering Foundation Agents Towards General Computer Control [[paper](https://arxiv.org/html/2403.03186v1)] [[blog](https://baai-agents.github.io/Cradle/)] [[code](https://github.com/BAAI-Agents/Cradle)]
  - The Cradle framework empowers nascent foundation models to perform complex computer tasks via the same unified interface humans use, i.e., screenshots as input and keyboard & mouse operations as output.
  - 2024-06-27: A major update! Cradle is extened to four games: [RDR2](https://www.rockstargames.com/reddeadredemption2), [Stardew Valley](https://www.stardewvalley.net/), [Cities: Skylines](https://www.paradoxinteractive.com/games/cities-skylines/about), and [Dealer's Life 2](https://abyteentertainment.com/dealers-life-2/) and various software, including but not limited to Chrome, Outlook, Capcut, Meitu and Feishu. We also release our latest [paper](https://arxiv.org/pdf/2403.03186).
<br>
<div align="center">
<img src="https://github.com/BAAI-Agents/Cradle/blob/main/docs/images/gcc.jpg" width="600px">
</div>
<br>

## 🗺 Economy and Society
- Generative Agents: interactive simulacra of human behavior [[paper](https://arxiv.org/abs/2304.03442)] [[code](https://github.com/joonspk-research/generative_agents)]
  - This work describes an architecture that extends a large language model to store a complete record of the agent's experiences using natural language, synthesize those memories over time into higher-level reflections, and retrieve them dynamically to plan behavior.

<br>
<div align="center">
<img src="https://github.com/joonspk-research/generative_agents/blob/main/cover.png" width="600px">
</div>
<br>

- 
## 🔗 Citation
If you find this repository useful, please cite our paper:

```

```

## 🤝 Contact
- Wenshuo Zhai [@WenshuoZhai](https://github.com/ZhaiWenShuo): zhaiwenshuo@nudt.edu.cn
