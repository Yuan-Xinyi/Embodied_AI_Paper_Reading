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
- [Model-Based Diffusion Sampling for Predictive Control in Offline Decision Making](https://arxiv.org/abs/2512.08280)
  > Improve reliability: a planner + a dynamics model
- [Equivariant Diffusion Policy](https://arxiv.org/abs/2407.01812)

### Reinforcement Learning

### IL+RL
- [ReinforceGen: Hybrid Skill Policies with Automated Data Generation and Reinforcement Learning](https://arxiv.org/abs/2512.16861)  
  > IL (teleoperation and synthetic data gen) + RL (online adaptation)
- [RL-100: Performant Robotic Manipulation with Real-World Reinforcement Learning](https://arxiv.org/abs/2510.14830)

## Reasoning
- [Watching, Reasoning, and Searching: A Video Deep Research Benchmark on Open Web for Agentic Video Reasoning](https://arxiv.org/abs/2601.06943)
- [Lost in the Noise: How Reasoning Models Fail with Contextual Distractors](https://arxiv.org/abs/2601.07226)
  > models disproportionately focus on distractor tokens

### Inference
- [SpatialTree: How Spatial Abilities Branch Out in MLLMs](https://arxiv.org/pdf/2512.20617)  
  > Spatial abilities: low-level perception (L1), mental mapping (L2), simulation (L3), and agentic competence (L4)

### Reward Design
- [RoboReward: General-Purpose Vision-Language Reward Models for Robotics](https://arxiv.org/pdf/2601.00675)  
  > Relabels successful episodes with failed instructions and near-miss instructions for the same video (clipping).

## Manipulation

### Tool Box

**Basics**
- [Foam: Spherical Approximations of URDFs](https://github.com/CoMMALab/foam): Convert `.stl` and `.urdf` into spheres.
- [On the Continuity of Rotation Representations in Neural Networks](https://arxiv.org/pdf/1812.07035): Continuous rotation representations in 5D and 6D

**Action Smoothing**
- [Real-Time Action Chunking with Large Models](https://www.pi.website/research/real_time_chunking): Inference-time RTC
- [Training-Time Action Conditioning for Efficient Real-Time Chunking](https://arxiv.org/pdf/2512.05964): Training-time RTC

**Representations**
- [DINOv2: Learning Robust Visual Features without Supervision](https://arxiv.org/abs/2304.07193)
- [SAM 3: Segment Anything with Concepts](https://github.com/facebookresearch/sam3)
- [Depth Anything 3: Recovering the Visual Space from Any Views](https://github.com/ByteDance-Seed/Depth-Anything-3)
- [PointNet: Deep Learning on Point Sets for 3D Classification and Segmentation](https://arxiv.org/abs/1612.00593): PCD encoder

**Data Augmentation**
- [RoboEngine: Plug-and-Play Robot Data Augmentation with Semantic Robot Segmentation and Background Generation](https://arxiv.org/abs/2503.18738): Visual data augmentations
- [RoboVIP: Multi-View Video Generation with Visual Identity Prompting Augments Robot Manipulation](https://robovip.github.io/RoboVIP/): Multi-view video generation

### TAMP

## Foundation Models
- [One Language-Free Foundation Model Is Enough for Universal Vision Anomaly Detection](https://arxiv.org/abs/2601.05552) 
- [What Is The Best 3D Scene Representation for Robotics? From Geometric to Foundation Models](https://arxiv.org/pdf/2512.03422)

### World Model
- [Flow Equivariant World Models: Memory for Partially Observed Dynamic Environments](https://arxiv.org/abs/2601.01075)  
  > Self-motion and external object motion are unified as flows to attain spatial latent memory & internal dynamics.
- [Yume1.5: A Text-Controlled Interactive World Generation Model](https://arxiv.org/pdf/2512.22096)

### VLA & VLM
- [ReconVLA: Reconstructive Vision-Language-Action Model as Effective Robot Perceiver](https://arxiv.org/pdf/2508.10333) **(AAAI2026 Outstanding Paper Award)**
- [Emergence of Human to Robot Transfer in Vision-Language-Action Models](https://www.pi.website/download/human_to_robot.pdf)  
  > The diversity of robot data for pre-training VLAs is proportional to the capability of leveraging human videos during post-training.
- [π 0.6: a VLA That Learns From Experience](https://arxiv.org/abs/2511.14759)  
  > Improve VLA through real-world deployments via reinforcement learning (RL)
