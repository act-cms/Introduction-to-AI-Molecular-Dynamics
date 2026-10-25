Introduction to AI-Molecular Dynamics
=====================================

This module teaches molecular dynamics (MD), the simulation of how atoms and
molecules move under physical force laws, from the basic MD loop to practical
materials modeling with LAMMPS, Atomsk, and OVITO. It also shows where AI tools
and large language models (LLMs) can help in planning, scripting, analysis, and
review of MD workflows, and how to audit what they produce for physical and
technical correctness. The module has seven lessons (eight notebooks), is
written for undergraduate and graduate students in materials science, physical
chemistry, and computational chemistry with beginner programming skills, and
takes about 8 to 12 hours in total.

The module was developed by Prof. Wenwu Xu (San Diego State University) as a
MolSSI ACT-CMS Faculty Fellow. It was piloted with undergraduate and graduate
students and used in ME 642 Materials Modeling at San Diego State University in
Spring 2026. Lesson pages, with links to open each notebook in Google Colab or
ChemCompute, are on the
[ACT-CMS Lesson Portal](https://act-cms.molssi.org/portal/lessons/Introduction-to-AI-Molecular-Dynamics/).

## Lesson/Module Contents

1. Introduction to Molecular Dynamics and AI-Assisted MD
    * Directory: `01_AI-MD-101`
    * Notebooks: `introduction-to-molecular-dynamics.ipynb` and
      `introduction-to-ai-llm-for-molecular-dynamics.ipynb`
    * Description: The basic MD loop (forces, potentials, Velocity Verlet
      integration, and trajectories) in Python, and what AI, machine learning,
      and LLMs can and cannot do in MD workflows.
    * Time: 2 to 2.5 hours (60 to 75 minutes per notebook)
2. Python MD From Scratch
    * Directory: `02_python-md-from-scratch`
    * Notebook: `python-md-from-scratch.ipynb`
    * Description: A small two dimensional MD code in NumPy with Lennard-Jones
      forces, periodic boundary conditions, Velocity Verlet integration, and an
      energy conservation check.
    * Time: 75 to 90 minutes
3. LAMMPS Fundamentals
    * Directory: `03_lammps-fundamentals`
    * Notebook: `lammps-fundamentals.ipynb`
    * Description: The sections of a LAMMPS input script, a minimal
      Lennard-Jones solid run, and the commands that set units, lattice,
      interactions, integration, and output.
    * Time: 75 to 90 minutes
4. Atomsk Structure Building
    * Directory: `04_atomsk-structure-building`
    * Notebook: `atomsk-structure-building.ipynb`
    * Description: Atomsk commands that build, duplicate, and orient crystals,
      remove an atom to make a vacancy, convert file formats, and prepare
      LAMMPS data files.
    * Time: 60 to 90 minutes
5. OVITO Visualization
    * Directory: `05_ovito-visualization`
    * Notebook: `ovito-visualization.ipynb`
    * Description: Loading LAMMPS output in OVITO, structure analysis modifiers
      (such as Common Neighbor Analysis, Coordination Analysis, and Atomic
      Strain), an optional OVITO Python script, and figure design.
    * Time: 60 to 90 minutes
6. Defects and Materials Modeling
    * Directory: `06_defects-and-materials-modeling`
    * Notebook: `defects-and-materials-modeling.ipynb`
    * Description: A step by step workflow that builds and relaxes a perfect
      FCC crystal, a vacancy, and a surface slab in LAMMPS, computes the vacancy
      formation energy and the surface energy, and checks the models in OVITO.
    * Time: 90 to 120 minutes
7. AI-Assisted MD Workflows
    * Directory: `07_ai-assisted-md-workflows`
    * Notebook: `ai-assisted-md-workflows.ipynb`
    * Description: Using LLMs to draft LAMMPS and analysis scripts and to plan
      parameter sweeps, and auditing AI output for physical and technical
      correctness with a checklist.
    * Time: 75 to 90 minutes

Each lesson directory has its own README with learning outcomes,
prerequisites, resources, and the files that the notebook creates.

## Running the Notebooks

* Each notebook can be opened in Google Colab, run on ChemCompute, or run in a
  local Python environment, which is recommended for the later lessons. Launch
  links for every notebook are on the lesson portal page.
* Lessons 1 and 2 need only Python with NumPy and Matplotlib. Lessons 3 to 7
  write LAMMPS, Atomsk, and OVITO input files into subfolders such as
  `lammps/`, `atomsk/`, and `ovito/`. Running those files needs local
  installations of LAMMPS, Atomsk, and OVITO, but students can also read and
  discuss the generated scripts without them. Lesson 7 also uses pandas.

## Prerequisites

* Basic Python (variables, loops, functions, and arrays) and running cells in
  Jupyter notebooks; see
  [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/).
* Introductory chemistry or materials science, including atomic structure,
  force, and energy. No prior experience with production MD software is
  required.

## For Instructors

Instructor notes are on the lesson portal page, and instructor access to the
course materials can be requested there. The lesson notebooks also serve as the
instructor versions; no separate instructor keys are provided. The `templates`,
`examples`, and `cookbooks` folders come from the ACT-CMS lesson template and
are not part of this module.

## How to Cite

Xu, W. *Introduction to AI-Molecular Dynamics*. ACT-CMS lesson module, The
Molecular Sciences Software Institute (MolSSI), 2026.
https://github.com/act-cms/Introduction-to-AI-Molecular-Dynamics

## License

This module is licensed under the Creative Commons
Attribution-NonCommercial-ShareAlike 4.0 International License (see
`LICENSE`).

## Acknowledgment

ACT-CMS (Accelerating Curricular Transformation in the Computational Molecular
Sciences) is a project of The Molecular Sciences Software Institute (MolSSI),
supported by the U.S. National Science Foundation (OAC 2321044 and 2321045).
