# Embodied_AI_Paper_Reading

***Disclaimer***: *This page contains subjective comments regarding the listed papers. For technical details and improved accuracy, please refer to the original papers via the provided links.*
## Surveys
[A Survey of Reinforcement Learning for Large Reasoning Models](https://arxiv.org/abs/2509.08827)<br>
[A review of learning-based dynamics models for robotic manipulation](https://www.science.org/doi/10.1126/scirobotics.adt1497)<br>
[Diffusion Models for Reinforcement Learning: A Survey](https://arxiv.org/abs/2311.01223)<br>

## Learning-based Method
### Imitation Learning
[Model-Based Diffusion Sampling for Predictive Control in Offline Decision Making](https://arxiv.org/abs/2512.08280)<br>
> Improve reliability: a planner + a dynamics model<br>

[Equivariant Diffusion Policy](https://arxiv.org/abs/2407.01812)<br>

### Reinforcement Learning
### IL+RL
[ReinforceGen: Hybrid Skill Policies with Automated Data Generation and Reinforcement Learning](https://arxiv.org/abs/2512.16861)
> Long horizon and complicated task decomposition
> IL (teleoperation and synthetic data gen) + RL (online adaptation)

[RL-100: Performant Robotic Manipulation with Real-World Reinforcement Learning](https://arxiv.org/abs/2510.14830)

## Reasoning
### Inference
[SpatialTree: How Spatial Abilities Branch Out in MLLMs](https://arxiv.org/pdf/2512.20617)
> Spatial abilities: low-level perception (L1), mental mapping (L2), simulation (L3), and agentic competence (L4)

### Reward Design
[RoboReward: General-Purpose Vision-Language Reward Models for Robotics](https://arxiv.org/pdf/2601.00675)<br>
> Automated vision-language reward models considering negative and partial progress examples.<br>
> Relabels successful episodes with failed instructions and near-miss instructions for the same video (clipping).<br>

## Manipulation
### Tool Box
**Basics**<br>
[Foam: Spherical Approximations of URDFs](https://github.com/CoMMALab/foam): Convert .stl and .urdf into spheres. <br>
[On the Continuity of Rotation Representations in Neural Networks](https://arxiv.org/pdf/1812.07035): Continuous rotation representations in 5D and 6D<br>

**Action Smoothing**<br>
[Real-Time Action Chunking with Large Models](https://www.pi.website/research/real_time_chunking): Inference-time RTC<br>
[Training-Time Action Conditioning for Efficient Real-Time Chunking](https://arxiv.org/pdf/2512.05964): Training-time RTC<br>

**Representations**<br>
[DINOv2: Learning Robust Visual Features  without Supervision](https://arxiv.org/abs/2304.07193)<br>
[SAM 3: Segment Anything with Concepts](https://github.com/facebookresearch/sam3)<br>
[Depth Anything 3: Recovering the Visual Space from Any Views](https://github.com/ByteDance-Seed/Depth-Anything-3)<br>


### Motion Planning

### TAMP

## Foundation Models
[What Is The Best 3D Scene Representation for Robotics? From Geometric to Foundation Models](https://arxiv.org/pdf/2512.03422)

### World Model
[Flow Equivariant World Models: Memory for Partially Observed Dynamic Environments](https://arxiv.org/abs/2601.01075)
> Self-motion and external object motion are unified as flows to attain spatial latent memory & internal dynamics.

[Yume1.5: A Text-Controlled Interactive World Generation Model](https://arxiv.org/pdf/2512.22096)

### VLA & VLM
[Emergence of Human to Robot Transfer in Vision-Language-Action Models](https://www.pi.website/download/human_to_robot.pdf)
> The diversity of robot data for pre-training VLAs is proportional to the capability of leveraging human videos during post-training.

[π 0.6: a VLA That Learns From Experience](https://arxiv.org/abs/2511.14759)
> Improve VLA through real-world deployments via reinforcement learning (RL)
