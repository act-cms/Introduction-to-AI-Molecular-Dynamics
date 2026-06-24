Lesson 01: Introduction to Molecular Dynamics and AI-Assisted MD
================================================================

The purpose of this lesson is to introduce students to the basic ideas behind
molecular dynamics (MD) and to show how artificial intelligence (AI) and large
language models (LLMs) can support MD workflows. Students work through simple
Python-based examples that connect forces, potentials, numerical integration,
trajectory analysis, and AI-assisted modeling concepts.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Describe the basic MD workflow of initializing particles, computing forces,
   integrating equations of motion, and analyzing trajectories.
2. Explain the role of a potential energy function using the Lennard-Jones
   potential as an introductory example.
3. Run and interpret a simple two-particle MD simulation using Python, NumPy,
   and Matplotlib.
4. Distinguish between physics-based models, machine learning models, and LLMs
   in the context of molecular simulation.
5. Identify appropriate and inappropriate uses of AI/LLM tools in MD workflows.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* Basic familiarity with Jupyter notebooks
    - Ability to run notebook cells, inspect code output, and rerun cells after
      changing parameters
* Basic use of Python scientific libraries
    - NumPy arrays and simple Matplotlib plots are introduced in the lesson, but
      prior exposure is helpful

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* Atomic and molecular structure at the introductory chemistry or materials
  science level
* Basic classical mechanics concepts, including position, velocity, force, and
  energy
* Basic mathematical functions and plots
* No prior experience with production MD software, machine learning potentials,
  or LLMs is required

### Resources

* [MolSSI Workshop: Python Scripting for Computational Molecular Sciences](https://education.molssi.org/python_scripting_cms/)
* [MolSSI CMS Python Workshop: Introduction](https://education.molssi.org/python_scripting_cms/01-introduction/index.html)
* [LAMMPS Documentation](https://docs.lammps.org/)
* [OVITO User Manual](https://www.ovito.org/manual/)
* [Atomsk Documentation](https://atomsk.univ-lille.fr/doc/)

### References

Portions of this lesson were adapted from or informed by:
* Standard introductory molecular dynamics teaching examples based on the
  Lennard-Jones potential and Velocity Verlet integration
* [LAMMPS Documentation](https://docs.lammps.org/)
* [OVITO User Manual](https://www.ovito.org/manual/)
* [Atomsk Documentation](https://atomsk.univ-lille.fr/doc/)

## Lesson Versions & Intended Modalities

Two introductory notebooks are provided. They can be used independently or as a
paired first lesson: the first notebook introduces MD fundamentals, and the
second introduces AI/LLM concepts for molecular simulation workflows.

| Modality     | Pedagogy                | Role of Instructor                                                       | Lesson Version                                            |
|--------------|-------------------------|---------------------------------------------------------------------------|----------------------------------------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                                       | `introduction-to-molecular-dynamics.ipynb`               |
| Synchronous  | Guided Inquiry Learning | Facilitate discussion, connect code behavior to MD concepts              | `introduction-to-molecular-dynamics.ipynb`               |
| Synchronous  | Guided Inquiry Learning | Guide discussion of AI use cases, limitations, and validation practices  | `introduction-to-ai-llm-for-molecular-dynamics.ipynb`    |

The `introduction-to-molecular-dynamics.ipynb` notebook introduces a minimal
MD workflow with a Lennard-Jones potential and Velocity Verlet integration. The
`introduction-to-ai-llm-for-molecular-dynamics.ipynb` notebook introduces AI,
machine learning, and LLM concepts through MD-relevant examples, including a
simple learned force-law demonstration.

No separate instructor key or instructor-notes notebook is currently provided
for this introductory lesson.
