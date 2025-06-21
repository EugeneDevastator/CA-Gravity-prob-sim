# Probability based movement + Gravity sim Cellular automata:
## [Launch](https://htmlpreview.github.io/?https://github.com/EugeneDevastator/CA-Gravity-prob-sim/blob/master/probability-based.html)

# Gravity & Probabilistic Movement Simulation

A cellular automaton that simulates gravitational fields and particle movement with velocity-based probabilistic motion.

## Simulation Rules

### Gravity Field Generation
- **Particle Sources**: Each particle generates a gravity field proportional to its mass
- **Field Propagation**: Gravity fields diffuse to neighboring cells each frame
- **Field Decay**: All gravity fields gradually decay over time to prevent infinite accumulation

### Particle Physics
- **Mass System**: Particles have variable mass (1-3 units) affecting their gravitational influence and inertia
- **Velocity Dynamics**: Particles maintain velocity vectors that are influenced by surrounding gravity fields
- **Gravity Acceleration**: Particles accelerate toward areas of higher gravitational field strength
- **Inertia**: Heavier particles accelerate slower than lighter ones when subjected to the same gravitational force

### Movement Mechanics
- **Probabilistic Motion**: Particles don't move deterministically - they have probabilities of moving in different directions
- **Velocity-Based Direction**: Movement probabilities are calculated based on the particle's current velocity vector
- **Alignment Factor**: Higher probability for moves that align with the particle's velocity direction
- **Velocity Threshold**: Particles need minimum velocity magnitude to attempt movement
- **Collision Avoidance**: Particles cannot move into occupied cells

### System Parameters
- **Velocity Damping**: Particle velocities gradually decrease over time (simulating friction/resistance)
- **Movement Scaling**: Velocity magnitude is scaled to determine movement probability strength
- **Field Strength**: Controls how much gravitational field particles generate
- **Diffusion Rate**: How quickly gravity fields spread to neighboring cells
