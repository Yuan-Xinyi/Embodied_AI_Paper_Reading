# Embodied_AI_Paper_Reading

***Disclaimer***: *This page contains subjective comments regarding the listed papers. For technical details and improved accuracy, please refer to the original papers via the provided links.*

## Surveys
- [A Survey of Reinforcement Learning for Large Reasoning Models](https://arxiv.org/abs/2509.08827)
- [A review of learning-based dynamics models for robotic manipulation](https://pubmed.ncbi.nlm.nih.gov/40961212/)
- [Diffusion Models for Reinforcement Learning: A Survey](https://arxiv.org/abs/2311.01223)
- [Diffusion Model for Planning: A Systematic Literature Review](https://arxiv.org/abs/2408.10266)

## Learning-based Method

### Dynamics
- [Contact-Aware Neural Dynamics](https://arxiv.org/pdf/2601.12796)

### Imitation Learning
- [How to Peel with a Knife: Aligning Fine-Grained Manipulation with Human Preference](https://arxiv.org/pdf/2603.03280)
- [Abstracting Robot Manipulation Skills via Mixture-of-Experts Diffusion Policies](https://arxiv.org/abs/2601.21251)
- [Do You Need Proprioceptive States in Visuomotor Policies?](https://arxiv.org/abs/2509.18644): State-free Policies.
- [Action-to-Action Flow Matching](https://arxiv.org/abs/2602.07322)
- [Diffusion In Diffusion: Reclaiming Global Coherence in Semi-Autoregressive Diffusion](https://huggingface.co/papers/2601.13599)
- [Model-Based Diffusion Sampling for Predictive Control in Offline Decision Making](https://arxiv.org/abs/2512.08280): DP as planner and dynamics model.
- [Equivariant Diffusion Policy](https://arxiv.org/abs/2407.01812)

### Reinforcement Learning

### IL+RL
- [ReinforceGen: Hybrid Skill Policies with Automated Data Generation and Reinforcement Learning](https://arxiv.org/abs/2512.16861): IL+RL 
- [RL-100: Performant Robotic Manipulation with Real-World Reinforcement Learning](https://arxiv.org/abs/2510.14830)

## Reasoning
- [Watching, Reasoning, and Searching: A Video Deep Research Benchmark on Open Web for Agentic Video Reasoning](https://arxiv.org/abs/2601.06943)
- [Lost in the Noise: How Reasoning Models Fail with Contextual Distractors](https://arxiv.org/abs/2601.07226): Models are distracted.

### Inference
- [SpatialTree: How Spatial Abilities Branch Out in MLLMs](https://arxiv.org/pdf/2512.20617): Spatial abilities level 1-4.

### Reward Models
- [ROBOMETER: Scaling General-Purpose Robotic Reward Models via Trajectory Comparisons](https://arxiv.org/pdf/2603.02115)
- [TOPReward: Token Probabilities as Hidden Zero-Shot Rewards for Robotics](https://topreward.github.io/webpage/)
- [Real-Time Aligned Reward Model beyond Semantics](https://huggingface.co/papers/2601.22664): Dense reward for RLHF.
- [DenseGRPO: From Sparse to Dense Reward for Flow Matching Model Alignment](https://huggingface.co/papers/2601.20218): Dense reward guidance.
- [RoboReward: General-Purpose Vision-Language Reward Models for Robotics](https://arxiv.org/pdf/2601.00675): Construct failure demonstrations.

## Manipulation

### Tool Box

**Basics**
- [Demystifying Action Space Design for Robotic Manipulation Policies](https://arxiv.org/pdf/2602.23408)
  > **Quote:** Our large-scale results suggest that properly designing the policy to predict delta actions consistently improves performance, while joint-space and task-space representations offer complementary strengths, favoring control stability and generalization, respectively.
- [Foam: Spherical Approximations of URDFs](https://github.com/CoMMALab/foam): Convert `.stl` and `.urdf` into spheres.
- [On the Continuity of Rotation Representations in Neural Networks](https://arxiv.org/pdf/1812.07035): Continuous rotation representations in 5D and 6D.

**Action Smoothing**
- [Real-Time Action Chunking with Large Models](https://www.pi.website/research/real_time_chunking): Inference-time RTC.
- [Training-Time Action Conditioning for Efficient Real-Time Chunking](https://arxiv.org/pdf/2512.05964): Training-time RTC.

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
