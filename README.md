# Embodied_AI_Paper_Reading

***Disclaimer***: *This page contains subjective comments regarding the listed papers. For technical details and improved accuracy, please refer to the original papers via the provided links.*

## Surveys
- (2025.09 Arxiv) [A Survey of Reinforcement Learning for Large Reasoning Models](https://arxiv.org/abs/2509.08827)
- (2025.09 Science Robotics) [A review of learning-based dynamics models for robotic manipulation](https://pubmed.ncbi.nlm.nih.gov/40961212/)
- (2024.08 Arxiv) [Diffusion Model for Planning: A Systematic Literature Review](https://arxiv.org/abs/2408.10266)
- (2023.11 Arxiv) [Diffusion Models for Reinforcement Learning: A Survey](https://arxiv.org/abs/2311.01223)


## New Trends

### Future-Guided Learning-Based Method
- (2026.03 Arxiv) [FutureVLA: Joint Visuomotor Prediction for Vision-Language-Action Model](https://arxiv.org/pdf/2603.10712)
  > ... processes continuous multi-frame clips and structurally decouples the latent representation into a visual stream and a motor stream ...
- (2026.03 Arxiv) [Inference-Time Enhancement of Generative Robot Policies via Predictive World Modeling](https://ieeexplore.ieee.org/abstract/document/11433756)
  > ... train an action-conditioned world model on expert demonstrations and ... to forecast the consequences of action proposals produced by the diffusion policy

### Self-Improvement Policy and Data Curation
- (2026.03 Arxiv) [Beyond Imitation: Reinforcement Learning Fine-Tuning for Adaptive Diffusion Navigation Policies](https://arxiv.org/pdf/2603.12868)
  > ... adopts Group Relative Policy Optimization (GRPO), which estimates relative advantages across sampled trajectories ...
- (2026.03 Arxiv) [RL-100: Performant Robotic Manipulation with Real-World Reinforcement Learning](https://arxiv.org/abs/2510.14830)
  > ... unifies imitation and reinforcement learning under a single clipped PPO surrogate objective applied within the denoising process ...
- (2025.12 Arxiv) [ReinforceGen: Hybrid Skill Policies with Automated Data Generation and Reinforcement Learning](https://arxiv.org/abs/2512.16861)
  > (A) ... pose predictor is fine-tuned towards a privileged teacher; ...(B) The skill policy is fine-tuned through residual reinforcement learning. (C) ... false-positive predictions from the termination predictor.
- (2024.03 Arxiv) [SELFI: Autonomous Self-Improvement with Reinforcement Learning for Social Navigation](https://arxiv.org/pdf/2603.12248)
  > ... applies online model-free reinforcement learning on top of offline model-based learning ...

## Learning-Based Method

### Dynamics
- (2026.01 Arxiv) [Contact-Aware Neural Dynamics](https://arxiv.org/pdf/2601.12796)
  > ...yields a contact-aware neural dynamics model that performs consistently across both simulation and the real world.

### Imitation Learning
- (2026.03 Arxiv) [OCRA: Object-Centric Learning with 3D and Tactile Priors for Human-to-Robot Action Transfer](https://arxiv.org/pdf/2603.14401)
  > ... object-centric learning from multi-view human demonstration videos and tactile sensing ...
- (2026.03 Arxiv) [One-Policy-Fits-All: Geometry-Aware Action Latents for Cross-Embodiment Manipulation](https://arxiv.org/pdf/2603.14522)
  > ... geometric structures of diverse end-effectors to construct a unified latent action representation, and employs a unified latent retargeting decoder to recover embodiment-specific actions.
- (2026.03 Arxiv) [How to Peel with a Knife: Aligning Fine-Grained Manipulation with Human Preference](https://arxiv.org/pdf/2603.03280)
  > ... initial policy via force-aware data collection and imitation learning, ... refine the policy through preference-based finetuning using a learned reward model ...
- (2026.02 Arxiv) [Action-to-Action Flow Matching](https://arxiv.org/abs/2602.07322)
  > ... a novel policy paradigm that shifts from random sampling to initialization informed by the previous action.
- (2026.01 Arxiv) [Diffusion In Diffusion: Reclaiming Global Coherence in Semi-Autoregressive Diffusion](https://huggingface.co/papers/2601.13599)
  > ... a 'draft-then-refine' framework designed to overcome the irreversibility and myopia problems inherent in block diffusion models.
- (2026.01 Arxiv) [Abstracting Robot Manipulation Skills via Mixture-of-Experts Diffusion Policies](https://arxiv.org/abs/2601.21251)
  > ... a diffusion-based mixture-of-experts policy that learns a compact orthogonal skill basis ...
- (2025.12 Arxiv) [Model-Based Diffusion Sampling for Predictive Control in Offline Decision Making](https://arxiv.org/abs/2512.08280):
  > ... a compositional diffusion framework that combines a diffusion planner with a dynamics diffusion model to generate task-aligned and dynamically plausible trajectories.
- (2025.09 Arxiv) [Do You Need Proprioceptive States in Visuomotor Policies?](https://arxiv.org/abs/2509.18644):
  > ... removing the proprioceptive state input and predicting actions only conditioned on visual observations ...
- (2024 CoRL) [Equivariant Diffusion Policy](https://arxiv.org/abs/2407.01812)
  > ... leverages domain symmetries to obtain better sample efficiency and generalization in the denoising function. 


### Reward Models
- (2026.03 Arxiv) [ROBOMETER: Scaling General-Purpose Robotic Reward Models via Trajectory Comparisons](https://arxiv.org/pdf/2603.02115)
  > ... a scalable reward modeling framework that combines intra-trajectory progress supervision with inter-trajectory preference supervision.
- (2026.02 Arxiv) [TOPReward: Token Probabilities as Hidden Zero-Shot Rewards for Robotics](https://topreward.github.io/webpage/)
  > TOPReward extracts task progress directly from the VLM's internal token logits. 
- (2026.01 Arxiv) [Real-Time Aligned Reward Model beyond Semantics](https://huggingface.co/papers/2601.22664):
  > Instead, it leverages the evolving hidden states of the policy (namely policy feedback) to align with the real-time distribution shift of the policy during the RL process.
- (2026.01 Arxiv) [DenseGRPO: From Sparse to Dense Reward for Flow Matching Model Alignment](https://huggingface.co/papers/2601.20218):
  > ... propose to predict the step-wise reward gain as dense reward of each denoising step, which applies a reward model on the intermediate clean images via an ODE-based approach.
- (2026.01 Arxiv) [RoboReward: General-Purpose Vision-Language Reward Models for Robotics](https://arxiv.org/pdf/2601.00675):
  > ... a robotics reward dataset and benchmark built on large-scale real-robot corpora from Open X-Embodiment (OXE) and RoboArena, ... propose counterfactual relabeling that turns successful episodes into calibrated negative and near-miss examples for the same video.

## Manipulation

### Tool Box

**Basics**
- (2026.02 Arxiv) [Demystifying Action Space Design for Robotic Manipulation Policies](https://arxiv.org/pdf/2602.23408)
  > ...properly designing the policy to predict delta actions consistently improves performance, while joint-space and task-space representations offer complementary strengths, favoring control stability and generalization, respectively.
- (2025.03 Arxiv) [Foam: Spherical Approximations of URDFs](https://github.com/CoMMALab/foam):
  > ... a tool to generate spherical approximations of robot geometry from an input Universal Robot Description Format (URDF) file.
- (2019 CVPR) [On the Continuity of Rotation Representations in Neural Networks](https://arxiv.org/pdf/1812.07035):
  > We show that the 3D rotations have continuous representations in 5D and 6D, which are more suitable for learning.

**Action Smoothing**
- (2025.12 Arxiv) [Training-Time Action Conditioning for Efficient Real-Time Chunking](https://arxiv.org/pdf/2512.05964): Training-time RTC.
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

**Data Augmentation**
- [RoboEngine: Plug-and-Play Robot Data Augmentation with Semantic Robot Segmentation and Background Generation](https://arxiv.org/abs/2503.18738): Visual data augmentations.
- [RoboVIP: Multi-View Video Generation with Visual Identity Prompting Augments Robot Manipulation](https://robovip.github.io/RoboVIP/): Multi-view video generation.

### TAMP

## Foundation Models
- [DeFM: Learning Foundation Representations from Depth for Robotics](https://arxiv.org/pdf/2601.18923): Depth foundation representations.
- [Point Bridge: 3D Representations for Cross Domain Policy Learning](https://arxiv.org/pdf/2601.16212)
- [One Language-Free Foundation Model Is Enough for Universal Vision Anomaly Detection](https://arxiv.org/abs/2601.05552) 
- [What Is The Best 3D Scene Representation for Robotics? From Geometric to Foundation Models](https://arxiv.org/pdf/2512.03422)

### World Model
- [ContactGaussian-WM: Learning Physics-Grounded World Model from Videos](https://arxiv.org/pdf/2602.11021)
- [Causal World Modeling for Robot Control](https://arxiv.org/abs/2601.21998): Representation entanglement.
- [World Action Models are Zero-shot Policies](https://dreamzero0.github.io/)
- [Flow Equivariant World Models: Memory for Partially Observed Dynamic Environments](https://arxiv.org/abs/2601.01075): Dynamic spatial memory.
- [Yume1.5: A Text-Controlled Interactive World Generation Model](https://arxiv.org/pdf/2512.22096)

### VLA & VLM
- [MEM: Multi-Scale Embodied Memory for Vision Language Action Models](https://arxiv.org/pdf/2603.03596)
- [SkillVLA: Tackling Combinatorial Diversity in Dual-Arm Manipulation via Skill Reuse](https://arxiv.org/pdf/2603.03836)
- [A Pragmatist Robot: Learning to Plan Tasks by Experiencing the Real World](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=11419794)
- [ANY3D-VLA: Enhancing VLA Robustness via Diverse Point Clouds](https://arxiv.org/pdf/2602.00807)
- [ST4VLA: Spatially Guided Training for Vision-Language-Action Models](https://arxiv.org/abs/2602.10109)
- [Steerable Vision-Language-Action Policies for Embodied Reasoning and Hierarchical Control](https://arxiv.org/pdf/2602.13193)
- [ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver](https://arxiv.org/pdf/2508.10333) **(AAAI2026 Outstanding Paper Award)**
- [Emergence of Human to Robot Transfer in Vision-Language-Action Models](https://www.pi.website/download/human_to_robot.pdf): Robotics data matters.  
- [π 0.6: a VLA That Learns From Experience](https://arxiv.org/abs/2511.14759): Improve real-world deployment.  
