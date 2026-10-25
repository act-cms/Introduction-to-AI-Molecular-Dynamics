Lesson 06: Defects and Materials Modeling
=========================================

The purpose of this lesson is to apply LAMMPS, Atomsk, and OVITO to practical
materials modeling. Students build, relax, and analyze a perfect crystal, a
vacancy, and a surface slab, compute defect and surface energies, and decide
what must be validated before trusting a defect simulation. The examples use a
small Lennard-Jones FCC crystal, so the LAMMPS scripts need no separate
potential file; the same workflow carries over to real materials with a
validated potential, such as an EAM potential for a metal.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Explain the difference between a perfect crystal, a point defect, and a
   surface model.
2. Generate LAMMPS input scripts for a perfect FCC crystal, a vacancy, and a
   slab.
3. Compute the vacancy formation energy from relaxed total energies.
4. Estimate the surface energy from a slab calculation.
5. Create an OVITO visualization checklist for checking whether a model is
   physically reasonable.
6. Identify what must be validated before trusting a defect simulation,
   including LAMMPS or Atomsk commands drafted by an AI assistant.

### Estimated Time

90 to 120 minutes.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* LAMMPS input scripts, Atomsk commands, and OVITO
    - [Lesson 03](../03_lammps-fundamentals/),
      [Lesson 04](../04_atomsk-structure-building/), and
      [Lesson 05](../05_ovito-visualization/)
* Optional: a local LAMMPS installation (`lmp`, `lmp_serial`, `lammps`, or
  `lmp_mpi` on the PATH). Without it, the notebook uses example energies so
  that students can still practice the analysis.

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* Crystal structures and point defects at an introductory level
* Energy minimization (relaxation) and periodic boundary conditions
* Total energy and energy per atom

### Resources

* [LAMMPS `minimize` Command](https://docs.lammps.org/minimize.html)
* [LAMMPS `delete_atoms` Command](https://docs.lammps.org/delete_atoms.html)
* [Atomsk Documentation](https://atomsk.univ-lille.fr/doc/)
* [OVITO User Manual](https://www.ovito.org/manual/)

### References

Portions of this lesson were adapted from or informed by:
* Standard atomistic approaches to vacancy formation energy and surface energy
* [LAMMPS Documentation](https://docs.lammps.org/)

## Lesson Versions & Intended Modalities

One notebook is provided. It can be used for independent work or in class.

| Modality     | Pedagogy                | Role of Instructor                                                       | Lesson Version                         |
|--------------|-------------------------|--------------------------------------------------------------------------|----------------------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                                       | `defects-and-materials-modeling.ipynb` |
| Synchronous  | Guided Inquiry Learning | Pair students: one reads the input script, one tracks the physical meaning | `defects-and-materials-modeling.ipynb` |

Running the notebook creates the folders `lammps/`, `atomsk/`, `ovito/`,
`data/`, `figures/`, and `logs/`. It writes the LAMMPS inputs
`lammps/in.01_bulk_relax.lmp`, `lammps/in.02_vacancy_relax.lmp`, and
`lammps/in.03_slab_relax.lmp`, a workflow summary
(`data/defect_modeling_workflow.txt`), Atomsk command patterns
(`atomsk/atomsk_defect_command_patterns.txt`), and an OVITO checklist
(`ovito/visualization_checklist.md`). If LAMMPS is found, the notebook runs the
inputs, writes logs to `logs/` and relaxed structures to `data/`, and reads the
energies from the logs; otherwise it uses example values. The notebook ends
with student exercises and short instructor notes.

No separate instructor key or instructor notes notebook is currently provided
for this lesson.
