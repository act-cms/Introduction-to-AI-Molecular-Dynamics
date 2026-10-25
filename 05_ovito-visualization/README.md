Lesson 05: OVITO Visualization
==============================

The purpose of this lesson is to introduce visualization and analysis of
atomistic simulation data with OVITO: loading LAMMPS output, applying common
analysis modifiers, and preparing clear figures and movies.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Load LAMMPS dump and data files, and other common formats (XYZ, CFG, and
   POSCAR), into OVITO and confirm the simulation cell.
2. Apply common visualization and analysis modifiers, such as Coordination
   Analysis, Common Neighbor Analysis, and Atomic Strain.
3. Use coloring, slicing, and selection to make crowded structures readable.
4. Export snapshots, plots, or animations for scientific communication, by hand
   or with an optional OVITO Python script.

### Estimated Time

60 to 90 minutes.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* OVITO installed on a local computer (OVITO Basic is free); the OVITO Python
  module is optional
* A LAMMPS dump or data file, for example `dump.lj` from
  [Lesson 03](../03_lammps-fundamentals/)

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* Crystal structures and local atomic environments (FCC, BCC, and HCP) at an
  introductory level
* The LAMMPS output files introduced in Lesson 03

### Resources

* [OVITO User Manual](https://www.ovito.org/manual/)
* [OVITO Python Reference](https://docs.ovito.org/python/)

### References

Portions of this lesson were adapted from or informed by:
* [OVITO User Manual](https://www.ovito.org/manual/)

## Lesson Versions & Intended Modalities

One notebook is provided. It can be used for independent work or in class.

| Modality     | Pedagogy                | Role of Instructor                                                  | Lesson Version              |
|--------------|-------------------------|---------------------------------------------------------------------|-----------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                                  | `ovito-visualization.ipynb` |
| Synchronous  | Guided Inquiry Learning | Demonstrate the OVITO workflow live and discuss figure design       | `ovito-visualization.ipynb` |

Running the notebook writes an OVITO checklist to
`ovito/visualization_checklist.txt` and an optional OVITO Python example,
`ovito/ovito_python_example.py`, which applies Common Neighbor Analysis to a
LAMMPS trajectory and exports an image. The exercises open a dump file from
Lesson 03, color atoms by type and then by potential energy, apply Common
Neighbor Analysis, slice the simulation cell, and export a still image and a
short animation.

No separate instructor key or instructor notes notebook is currently provided
for this lesson.
