# Case Study - Legged robots

- SEA serial elastic actuator, torque controllable, impact robust joint units

## Control

- proprioception (joint position, IMU, contact sensors)
-> state estimation
- planning (motion, foothold, reference torque)
-> whole-body control
- joint control (torque,position)

- exteroception (camera, lidar)
-> Localization and Mapping
- navigation -> planning

## Floating base model

q = irib,qib,qj

u = ivb,bwib,dqj
(not q dot, angular velocities)

usually **quaternions**

$M(q)du + h(q,u) = S^T\tau + J_S^T(q)\lambda$

lambda  1..m

J_S=vec J_Ek

_IJ_E_k = vec I, -C_B...

### whole-body control

- planning
- EoM
  - split first 6, rest
  - ...

prioritized tasks

- 1 eom
- 1 force torque limits
- 2 no motion at contact points
- 3 CoM motion tracking
- 3 torso angular motion
- 3 foot motion tracking
- 3 end effector motion | force tracking
- 3 ...

### Actuation signals

 $\tau^d = M_j(q)du^\star + h_j(q,u) - J_s,j(q)\lambda^\star$

$\tau^{ref} = \tau^d + k_Pq + k_Ddq$

### Classic approach

### MPC

### Reinforcement Learning

- learn from massive data generated with a fast and accurate simulator

#### Reality gap

- delay, noise

- **Solution** use nn: from commands to torques

#### Learning to locomote over rough terrain

- impossible to model in siumulation
- hard to sense from perception

##### Method: privileged training

Policy training

1. teacher policy training
1. ??

##### Friction Estimation

- worked in model based control, not very good
- much better for RL

##### Reflex

#### Learning-based locomotion including perception

## Navigation

### Environment perception

- SLAM

#### Traversability estimation

Train with

- feature extractor
- cost predictor

### avoid human guidance

- target pos 
- path planner 
- mm
- mm
- mm

### measurement - reconstruction



