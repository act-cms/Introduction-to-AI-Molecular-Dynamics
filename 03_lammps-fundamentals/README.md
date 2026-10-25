Lesson 03: LAMMPS Fundamentals
==============================

The purpose of this lesson is to introduce practical molecular dynamics (MD)
simulation with LAMMPS. Students learn the structure of a LAMMPS input script,
write a minimal Lennard-Jones solid example from the notebook, and connect each
command to a physical modeling choice.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Identify the main sections of a LAMMPS input script: simulation settings,
   system construction, force field, output, and minimization or dynamics.
2. Create a simple atomistic system directly in LAMMPS (a Lennard-Jones FCC
   solid in reduced units).
3. Explain the role of key commands such as `units`, `lattice`, `create_atoms`,
   `pair_style`, `velocity`, `fix nve`, `thermo`, and `dump`.
4. Run the script with LAMMPS and interpret thermo output, dump files, and
   common run settings.

### Estimated Time

75 to 90 minutes.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* Basic use of a command line terminal to run a program
* Optional: a local LAMMPS installation to run the generated script (the
  executable may be named `lmp`, `lmp_serial`, `lmp_mpi`, or `lammps`)

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* The basic MD loop, pair potentials, and Velocity Verlet integration
  ([Lesson 01](../01_AI-MD-101/) and [Lesson 02](../02_python-md-from-scratch/))
* Crystal lattices, such as FCC, at an introductory level
* Constant energy (NVE) dynamics at an introductory level

### Resources

* [LAMMPS Documentation](https://docs.lammps.org/)
* [LAMMPS Commands](https://docs.lammps.org/Commands_all.html)
* [OVITO User Manual](https://www.ovito.org/manual/), to view the trajectory

### References

Portions of this lesson were adapted from or informed by:
* [LAMMPS Documentation](https://docs.lammps.org/) and the Lennard-Jones example
  inputs distributed with LAMMPS

## Lesson Versions & Intended Modalities

One notebook is provided. It can be used for independent work or in class.

| Modality     | Pedagogy                | Role of Instructor                                              | Lesson Version              |
|--------------|-------------------------|-----------------------------------------------------------------|-----------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                              | `lammps-fundamentals.ipynb` |
| Synchronous  | Guided Inquiry Learning | Walk through each section of the input script and run it live   | `lammps-fundamentals.ipynb` |

Running the notebook writes the input script `lammps/in.lj_solid`. Running that
script with LAMMPS (for example, `lmp -in lammps/in.lj_solid`) prints the thermo
output and writes the trajectory file `dump.lj` for OVITO. The exercises change
the run length, replace `fix nve` with `fix nvt` and a target temperature,
enlarge the lattice, open `dump.lj` in OVITO, and add a `write_data` command.

No separate instructor key or instructor notes notebook is currently provided
for this lesson.
