# Rotorcraft

- Helicopter
- Autogyro
- Gyrodyne

## Helicopter

- Single rotor
  - most efficient
  - limited payload
  - need to balance, counter-torque
- Multi rotor

## UAS

- Quadrotor / Multicopter
  - very good torque compensation
  - high maneuverability and agility
- Standard helicopter
  - most efficient design
  - complex control
- ducted fan
  - torques produced by control surfaces
- Coaxial
- Omnidirectional Multicoper
  - over-actuated
  - flies in all directions at any attitude of the main body

## Modeling of Quadcopter

- system analysis
- control laws design and simulation

### model assumptions
<!-- TODO: -->

### overview

- motor dynamics
- aerodynamics
- body dynamics

### Modelling

- EoM
- Newton-Euler
  - F =
  - T =
  - (in body coordinates)

### Acting forces and torques

- thrust
- counter-torque
- gravity in earth-frame

 often (x,y,z) expressed as (north, east, down)

### Structural properties

- arm length
- rotor height (to CoG)
- mass
- inertia matrix

### Forces

- thrust, sum of thrusts (in body frame)
- weight, g rotated to body frame

### Torques

<!-- TODO: [t,t,q] -->

### Representing the attitude

zyx-euler angel for rotation

- yaw z (-pi->pi)
<!-- WARN: check angle limits! -->
- pitch y (-pi/2->pi/2)
- roll x (-pi->pi)

Problems with singularity


