Lesson 02: Python MD From Scratch
=================================

The purpose of this lesson is to build a minimal molecular dynamics (MD) engine
in Python so that students can see each moving part of an MD method: particle
positions and velocities, pair forces, periodic boundaries, time integration,
and energy checks. The goal is clarity, not speed.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Implement simple MD data structures (positions, velocities, and masses) with
   NumPy.
2. Apply periodic boundary conditions with the minimum image convention.
3. Compute pairwise forces and the potential energy from a simple potential
   (Lennard-Jones).
4. Use Velocity Verlet integration to propagate a trajectory.
5. Inspect energy conservation and explain how the time step affects stability.

### Estimated Time

75 to 90 minutes.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* Basic use of NumPy arrays, simple Matplotlib plots, and Jupyter notebooks
    - [Lesson 01: Introduction to Molecular Dynamics and AI-Assisted MD](../01_AI-MD-101/)

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* The basic MD loop and the Lennard-Jones potential (Lesson 01)
* Basic classical mechanics, including force, kinetic energy, and potential
  energy
* Reduced (dimensionless) units at an introductory level

### Resources

* [MolSSI Workshop: Python Scripting for Computational Molecular Sciences](https://education.molssi.org/python_scripting_cms/)
* [LAMMPS Documentation](https://docs.lammps.org/), for comparison with a
  production MD code

### References

Portions of this lesson were adapted from or informed by:
* Standard introductory molecular dynamics teaching examples based on the
  Lennard-Jones potential and Velocity Verlet integration

## Lesson Versions & Intended Modalities

One notebook is provided. It can be used for independent work or in class.

| Modality     | Pedagogy                | Role of Instructor                                               | Lesson Version                 |
|--------------|-------------------------|------------------------------------------------------------------|--------------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                               | `python-md-from-scratch.ipynb` |
| Synchronous  | Guided Inquiry Learning | Facilitate coding, discuss energy drift and the choice of time step | `python-md-from-scratch.ipynb` |

The notebook runs with Python, NumPy, and Matplotlib only and does not write any
files. It ends with exercises: change the time step and observe the drift in
total energy, increase the number of particles and note the runtime, add a
simple velocity rescaling thermostat, save the trajectory to an XYZ style file,
and outline a neighbor list strategy.

No separate instructor key or instructor notes notebook is currently provided
for this lesson.
