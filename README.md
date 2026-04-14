***Disclaimer***: *This page may contain subjective comments. For technical details and improved accuracy, please refer to the original papers via the provided links. For papers from arXiv, the date indicated refers to the month of the first upload*

## External Resources
- Akihiko Watanabe [X上のAIトレンド（？）（個人の感想です）](https://github.com/AkihikoWatanabe/paper_notes/wiki/X%E4%B8%8A%E3%81%AEAI%E3%83%88%E3%83%AC%E3%83%B3%E3%83%89%EF%BC%88%EF%BC%9F%EF%BC%89%EF%BC%88%E5%80%8B%E4%BA%BA%E3%81%AE%E6%84%9F%E6%83%B3%E3%81%A7%E3%81%99%EF%BC%89) [わたしのべんきょうノート](https://akihikowatanabe.github.io/paper_notes/)
- [Awesome-Robotics-Manipulation](https://github.com/BaiShuanghao/Awesome-Robotics-Manipulation)
- [Awesome Robotics Libraries](https://github.com/jslee02/awesome-robotics-libraries)
- [awesome-world-models-for-robots](https://github.com/operator22th/awesome-world-models-for-robots)
- [Awesome Physical AI](https://github.com/keon/awesome-physical-ai)
- [Awesome RL-VLA for Robotic Manipulation](https://github.com/Denghaoyuan123/Awesome-RL-VLA)

## Surveys
- (2025.09 arXiv) [A Survey of Reinforcement Learning for Large Reasoning Models](https://arxiv.org/abs/2509.08827)
- (2025.09 Science Robotics) [A review of learning-based dynamics models for robotic manipulation](https://pubmed.ncbi.nlm.nih.gov/40961212/)
- (2024.08 arXiv) [Diffusion Model for Planning: A Systematic Literature Review](https://arxiv.org/abs/2408.10266)
- (2023.11 arXiv) [Diffusion Models for Reinforcement Learning: A Survey](https://arxiv.org/abs/2311.01223)

## New Trends

### Future-Guided Learning-Based Method & WAM
- (2026.03 arXiv) [FutureVLA: Joint Visuomotor Prediction for Vision-Language-Action Model](https://arxiv.org/pdf/2603.10712)
  > ... processes continuous multi-frame clips and structurally decouples the latent representation into a visual stream and a motor stream ...
- (2026.03 arXiv) [Inference-Time Enhancement of Generative Robot Policies via Predictive World Modeling](https://ieeexplore.ieee.org/abstract/document/11433756)
  > ... train an action-conditioned world model on expert demonstrations and ... to forecast the consequences of action proposals produced by the diffusion policy

### Self-Improvement Policy
- (2026.03 PI) [RL Token: Bootstrapping Online RL with  Vision-Language-Action Models](https://www.pi.website/research/rlt)
  > We achieve this by training the VLA to expose an RL token, a compressed representation that makes task-relevant pretrained knowledge accessible to a lightweight online RL policy.
- (2026.03 arXiv) [SPIRAL: A Closed-Loop Framework for Self-Improving Action World Models via Reflective Planning Agents](https://arxiv.org/abs/2603.08403)
  > ... a closed-loop think-act-reflect process, ... A PlanAgent decomposes abstract actions into object-centric sub-actions, while a CriticAgent evaluates intermediate results and guides iterative refinement with long-horizon memory. 
- (2026.03 arXiv) [Update-Free On-Policy Steering via Verifiers](https://arxiv.org/pdf/2603.10282)
  > ... enables the robot to predict the success likelihood of its actions and adapt its strategy at execution time.
- (2026.03 arXiv) [Beyond Imitation: Reinforcement Learning Fine-Tuning for Adaptive Diffusion Navigation Policies](https://arxiv.org/pdf/2603.12868)
  > ... adopts Group Relative Policy Optimization (GRPO), which estimates relative advantages across sampled trajectories ...
- (2026.03 arXiv) [RL-100: Performant Robotic Manipulation with Real-World Reinforcement Learning](https://arxiv.org/abs/2510.14830)
  > ... unifies imitation and reinforcement learning under a single clipped PPO surrogate objective applied within the denoising process ...
- (2025.12 arXiv) [ReinforceGen: Hybrid Skill Policies with Automated Data Generation and Reinforcement Learning](https://arxiv.org/abs/2512.16861)
  > (A) ... pose predictor is fine-tuned towards a privileged teacher; ...(B) The skill policy is fine-tuned through residual reinforcement learning. (C) ... false-positive predictions from the termination predictor.
- (2025 NeurIPS) [Self-Improving Embodied Foundation Models](https://openreview.net/forum?id=KXMIIVUB9U)
  > The first stage, Supervised Fine-Tuning (SFT), fine-tunes pretrained foundation models using both: a) behavioral cloning, and b) steps-to-go prediction objectives. In the second stage, Self-Improvement, steps-to-go prediction enables the extraction of a well-shaped reward function and a robust success detector,...
- (2025 ICLR) [RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation](https://iclr.cc/virtual/2025/poster/31507)
  > ..., named RoboCat, is a visual goal-conditioned decision transformer capable of consuming action-labelled visual experience.
- (2024.03 arXiv) [Scaling Instructable Agents Across Many Simulated Worlds](https://arxiv.org/abs/2404.10179)
  > Our agents interact with environments in real-time using a generic, human-like interface: the inputs are image observations and language instructions and the outputs are keyboard-and-mouse actions.
- (2024.03 arXiv) [SELFI: Autonomous Self-Improvement with Reinforcement Learning for Social Navigation](https://arxiv.org/pdf/2603.12248)
  > SELFI stabilizes the online learning process by incorporating the same model-based learning objective from offline pre-training into the Q-values learned with online model-free reinforcement learning.
- (2020 NeurIPS) [AWAC: Accelerating Online Reinforcement Learning with Offline Datasets](https://openreview.net/forum?id=OJiM1R3jAtZ)
  > ... providing a simple and effective framework that is able to leverage large amounts of offline data and then quickly perform online fine-tuning of RL policies.

## Learning-Based Method

### Dynamics
- (2026.01 arXiv) [Contact-Aware Neural Dynamics](https://arxiv.org/pdf/2601.12796)
  > ...yields a contact-aware neural dynamics model that performs consistently across both simulation and the real world.

### Imitation Learning
- (2026.03 arXiv) [ICLR: In-Context Imitation Learning with Visual Reasoning](https://arxiv.org/abs/2603.07530)
  > ... augments demonstration prompts with structured visual reasoning traces representing anticipated future robot trajectories in image space.
- (2026.03 arXiv) [OCRA: Object-Centric Learning with 3D and Tactile Priors for Human-to-Robot Action Transfer](https://arxiv.org/pdf/2603.14401)
  > ... object-centric learning from multi-view human demonstration videos and tactile sensing ...
- (2026.03 arXiv) [One-Policy-Fits-All: Geometry-Aware Action Latents for Cross-Embodiment Manipulation](https://arxiv.org/pdf/2603.14522)
  > ... geometric structures of diverse end-effectors to construct a unified latent action representation, and employs a unified latent retargeting decoder to recover embodiment-specific actions.
- (2026.03 arXiv) [How to Peel with a Knife: Aligning Fine-Grained Manipulation with Human Preference](https://arxiv.org/pdf/2603.03280)
  > ... initial policy via force-aware data collection and imitation learning, ... refine the policy through preference-based finetuning using a learned reward model ...
- (2026.02 arXiv) [Action-to-Action Flow Matching](https://arxiv.org/abs/2602.07322)
  > ... a novel policy paradigm that shifts from random sampling to initialization informed by the previous action.
- (2026.01 arXiv) [Diffusion In Diffusion: Reclaiming Global Coherence in Semi-Autoregressive Diffusion](https://huggingface.co/papers/2601.13599)
  > ... a 'draft-then-refine' framework designed to overcome the irreversibility and myopia problems inherent in block diffusion models.
- (2026.01 arXiv) [Abstracting Robot Manipulation Skills via Mixture-of-Experts Diffusion Policies](https://arxiv.org/abs/2601.21251)
  > ... a diffusion-based mixture-of-experts policy that learns a compact orthogonal skill basis ...
- (2025 CoRL) [Steering Your Diffusion Policy with Latent Space Reinforcement Learning](https://arxiv.org/abs/2506.15799)
  > ... adapting the BC policy by running RL over its latent-noise space.
- (2025.12 arXiv) [Model-Based Diffusion Sampling for Predictive Control in Offline Decision Making](https://arxiv.org/abs/2512.08280):
  > ... a compositional diffusion framework that combines a diffusion planner with a dynamics diffusion model to generate task-aligned and dynamically plausible trajectories.
- (2025.09 arXiv) [Do You Need Proprioceptive States in Visuomotor Policies?](https://arxiv.org/abs/2509.18644):
  > ... removing the proprioceptive state input and predicting actions only conditioned on visual observations ...
- (2024 CoRL) [Equivariant Diffusion Policy](https://arxiv.org/abs/2407.01812)
  > ... leverages domain symmetries to obtain better sample efficiency and generalization in the denoising function. 


### Reward Models
- (2026.03 arXiv) [Reward-Conditioned Reinforcement Learning](https://arxiv.org/abs/2603.05066)
  >  RCRL conditions the agent on reward parameterizations and learns multiple reward objectives from a shared replay data entirely off-policy, enabling a single policy to represent reward-specific behaviors. 
- (2026.03 arXiv) [ROBOMETER: Scaling General-Purpose Robotic Reward Models via Trajectory Comparisons](https://arxiv.org/pdf/2603.02115)
  > ... a scalable reward modeling framework that combines intra-trajectory progress supervision with inter-trajectory preference supervision.
- (2026.02 arXiv) [TOPReward: Token Probabilities as Hidden Zero-Shot Rewards for Robotics](https://topreward.github.io/webpage/)
  > TOPReward extracts task progress directly from the VLM's internal token logits. 
- (2026.01 arXiv) [Real-Time Aligned Reward Model beyond Semantics](https://huggingface.co/papers/2601.22664):
  > Instead, it leverages the evolving hidden states of the policy (namely policy feedback) to align with the real-time distribution shift of the policy during the RL process.
- (2026.01 arXiv) [DenseGRPO: From Sparse to Dense Reward for Flow Matching Model Alignment](https://huggingface.co/papers/2601.20218):
  > ... propose to predict the step-wise reward gain as dense reward of each denoising step, which applies a reward model on the intermediate clean images via an ODE-based approach.
- (2026.01 arXiv) [RoboReward: General-Purpose Vision-Language Reward Models for Robotics](https://arxiv.org/pdf/2601.00675):
  > ... a robotics reward dataset and benchmark built on large-scale real-robot corpora from Open X-Embodiment (OXE) and RoboArena, ... propose counterfactual relabeling that turns successful episodes into calibrated negative and near-miss examples for the same video.

## Manipulation

### Tool Box

**Basics**
- (2026.02 arXiv) [Demystifying Action Space Design for Robotic Manipulation Policies](https://arxiv.org/pdf/2602.23408)
  > ...properly designing the policy to predict delta actions consistently improves performance, while joint-space and task-space representations offer complementary strengths, favoring control stability and generalization, respectively.
- (2025.03 arXiv) [Foam: Spherical Approximations of URDFs](https://github.com/CoMMALab/foam):
  > ... a tool to generate spherical approximations of robot geometry from an input Universal Robot Description Format (URDF) file.
- (2019 CVPR) [On the Continuity of Rotation Representations in Neural Networks](https://arxiv.org/pdf/1812.07035):
  > We show that the 3D rotations have continuous representations in 5D and 6D, which are more suitable for learning.

**Action Smoothing**
- (2026.03 arXiv) [FASTER: Rethinking Real-Time Flow VLAs](https://arxiv.org/pdf/2603.19199)
  > FASTER adaptively prioritizes near-term actions during flow sampling,...
- (2026 ICLR) [Real-time robot execution with masked action chunking.](https://openreview.net/forum?id=r0RGJ1j9on)
  > ... critical yet overlooked factor: intra-chunk inconsistency, where the robot’s executed action chunk partially misaligns with its current perception ...
- (2025.12 arXiv) [VLASH: Real-Time VLAs via Future-State-Aware Asynchronous Inference](https://arxiv.org/abs/2512.01031)
  > VLASH estimates the future execution-time state by rolling the robot state forward with the previously generated action chunk, thereby bridging the gap between prediction and execution.
- (2025.12 arXiv) [Training-Time Action Conditioning for Efficient Real-Time Chunking](https://arxiv.org/pdf/2512.05964): Training-time RTC.
  > ... simulating inference delay at training time and conditioning on action prefixes directly, eliminating any inference-time overhead.
- (2025.11 TRO) [DiffOG: Differentiable Policy Trajectory Optimization With Generalizability](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=11267071)
  > ...take an unoptimized action trajectory as input and output an optimized trajectory that can accomplish the demonstrated task, ensuring constraint satisfaction and improving smoothness.
- (2025 NeurIPS) [Real-Time Execution of Action Chunking Flow Policies](https://arxiv.org/abs/2506.07339)
  > It generates the next action chunk while executing the current one, "freezing" actions guaranteed to execute and "inpainting" the rest.
- (2025.09 PI) [Real-Time Action Chunking with Large Models](https://www.pi.website/research/real_time_chunking): Inference-time RTC.
  > Our key insight is to pose real-time chunking as an inpainting problem. ... our goal is then to fill in the remainder of the new chunk, much like inpainting a section of an image that has been removed. 

**Representations**
- [OAT: Ordered Action Tokenization](https://ordered-action-tokenization.github.io/)
- [DINOv2: Learning Robust Visual Features without Supervision](https://arxiv.org/abs/2304.07193)
- [SAM 3: Segment Anything with Concepts](https://github.com/facebookresearch/sam3)
- [Depth Anything 3: Recovering the Visual Space from Any Views](https://github.com/ByteDance-Seed/Depth-Anything-3)
- [PointNet: Deep Learning on Point Sets for 3D Classification and Segmentation](https://arxiv.org/abs/1612.00593): PCD encoder.

**Data Augmentation and Data Curation**
- (2026.03 arXiv) [MolmoB T: Large-Scale Simulation Enables Zero-Shot Manipulation](https://arxiv.org/pdf/2603.16861)
  > ... we show that zero-shot transfer to the real world is not only possible, but effective for both static and mobile manipulation.
- (2026.03 arXiv) [SOFTMIMICGEN: A Data Generation System for Scalable Robot Learning in Deformable Object Manipulation](https://arxiv.org/pdf/2603.25725)
  > an automated data generation pipeline for deformable object manipulation tasks.
- (2026.04 arXiv) [Bridging the Simulation-to-Experiment Gap with Generative Models using Adversarial Distribution Alignment](https://arxiv.org/pdf/2604.01169)
  > ... bridges this simulation-to-experiment gap by pre-training a generative model on fully observed (but imperfect) simulation data, then aligning it with partial (but real) observations of experimental data. 
- (2026 CVPR) [MotionMaster: Generalizable Text-Driven Motion Generation and Editing](https://yzhu.io/publication/hoi2026cvpr/paper.pdf)
  > MotionMaster generates compositional action sequences from textual instructions, successfully producing action combinations never seen during training
- (2026.04 arXiv) [CRAFT: Video Diffusion for Bimanual Robot Data Generation](https://arxiv.org/pdf/2604.03552)
  > ... supports a unified augmentation pipeline spanning object pose changes, camera viewpoints, lighting and background variations, crossembodiment transfer, and multi-view synthesis.
- (2025 IROS) [RoboEngine: Plug-and-Play Robot Data Augmentation with Semantic Robot Segmentation and Background Generation](https://arxiv.org/abs/2503.18738)
  > ... generalize robot manipulation tasks across six entirely new scenes, based solely on demonstrations collected from a single scene ...
- (2026 CVPR) [RoboVIP: Multi-View Video Generation with Visual Identity Prompting Augments Robot Manipulation](https://robovip.github.io/RoboVIP/)
  > ... introduce visual identity prompting, which supplies exemplar images as conditioning inputs to guide the generation of the desired scene setup.

## Foundation Models
- (2026.01 arXiv) [DeFM: Learning Foundation Representations from Depth for Robotics](https://arxiv.org/pdf/2601.18923): Depth foundation representations.
- (2026.01 arXiv) [Point Bridge: 3D Representations for Cross Domain Policy Learning](https://arxiv.org/pdf/2601.16212)
- (2026.01 arXiv) [One Language-Free Foundation Model Is Enough for Universal Vision Anomaly Detection](https://arxiv.org/abs/2601.05552) 
- (2025.12 arXiv) [What Is The Best 3D Scene Representation for Robotics? From Geometric to Foundation Models](https://arxiv.org/pdf/2512.03422)
- (2024 CoRL) [Steering Your Generalists: Improving Robotic Foundation Models via Value Guidance](https://openreview.net/forum?id=6FGlpzC9Po)
  > ... enhances the performance of such generalist robot policies at deployment time by re-ranking their actions according to a value function learned via offline RL.

### World Model
- (2026.03 arXiv) [Physion-Eval: Evaluating Physical Realism in Generated Video via Human Reasoning](https://arxiv.org/pdf/2603.19607)
  > Each generated video is derived from a corresponding realworld reference video depicting a clear physical process, and annotated with temporally localized glitches, structured failure categories, and natural-language explanations of the violated physical behavior.
- (2026.04 arXiv) [World Action Verifier: Self-Improving World Models via Forward-Inverse Asymmetry](https://arxiv.org/pdf/2604.01985)
  > The key idea is to decompose action-conditioned state prediction into two factors—state plausibility and action reachability—and verify each separately.
- [ContactGaussian-WM: Learning Physics-Grounded World Model from Videos](https://arxiv.org/pdf/2602.11021)
- [Causal World Modeling for Robot Control](https://arxiv.org/abs/2601.21998): Representation entanglement.
- [World Action Models are Zero-shot Policies](https://dreamzero0.github.io/)
- [Flow Equivariant World Models: Memory for Partially Observed Dynamic Environments](https://arxiv.org/abs/2601.01075): Dynamic spatial memory.
- [Yume1.5: A Text-Controlled Interactive World Generation Model](https://arxiv.org/pdf/2512.22096)

### VLA & VLM
- (2026.04 arXiv) [CompassAD: Intent-Driven 3D Affordance Grounding in Functionally Competing Objects](https://arxiv.org/pdf/2604.02060)_
  > In real-world scenes, multiple objects may share identical affordances, yet only one is appropriate under the given task context. 
- [Can Vision-Language Models Solve the Shell Game?](https://arxiv.org/abs/2603.08436)
- [MEM: Multi-Scale Embodied Memory for Vision Language Action Models](https://arxiv.org/pdf/2603.03596)
- [SkillVLA: Tackling Combinatorial Diversity in Dual-Arm Manipulation via Skill Reuse](https://arxiv.org/pdf/2603.03836)
- [A Pragmatist Robot: Learning to Plan Tasks by Experiencing the Real World](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=11419794)
- [ANY3D-VLA: Enhancing VLA Robustness via Diverse Point Clouds](https://arxiv.org/pdf/2602.00807)
- [ST4VLA: Spatially Guided Training for Vision-Language-Action Models](https://arxiv.org/abs/2602.10109)
- [Steerable Vision-Language-Action Policies for Embodied Reasoning and Hierarchical Control](https://arxiv.org/pdf/2602.13193)
- [ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver](https://arxiv.org/pdf/2508.10333) **(AAAI 2026 Outstanding Paper Award)**
- [Emergence of Human to Robot Transfer in Vision-Language-Action Models](https://www.pi.website/download/human_to_robot.pdf): Robotics data matters.  
- [π 0.6: a VLA That Learns From Experience](https://arxiv.org/abs/2511.14759): Improve real-world deployment.  
