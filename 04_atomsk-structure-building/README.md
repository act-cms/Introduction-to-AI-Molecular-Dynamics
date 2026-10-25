Lesson 04: Atomsk Structure Building
====================================

The purpose of this lesson is to introduce atomistic model construction with
Atomsk, a command line tool for creating, transforming, and converting
atomistic structures, and to connect the structures it builds to LAMMPS
simulations and OVITO visualization.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Build and transform common crystalline structures, such as FCC aluminum and
   BCC iron, with Atomsk.
2. Duplicate and orient simulation cells, and convert structures between file
   formats (XSF, LAMMPS data, and XYZ).
3. Introduce simple defects, starting with a vacancy, and describe how Atomsk
   also builds substitutions, surfaces, and interfaces.
4. Prepare structures for LAMMPS simulations and read them with `read_data`,
   supplying the interatomic potential separately.

### Estimated Time

60 to 90 minutes.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* Basic use of a command line terminal to run a program
* Optional: local installations of Atomsk and LAMMPS to run the commands, and
  an EAM potential file for aluminum (for example, `Al99.eam.alloy`) for the
  LAMMPS energy minimization

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* Crystal structures (FCC, BCC, and diamond) and lattice parameters at an
  introductory level
* The structure of a LAMMPS input script
  ([Lesson 03](../03_lammps-fundamentals/))
* Point defects, such as vacancies, at an introductory level

### Resources

* [Atomsk Documentation](https://atomsk.univ-lille.fr/doc/)
* [LAMMPS `read_data` Command](https://docs.lammps.org/read_data.html)
* [OVITO User Manual](https://www.ovito.org/manual/)

### References

Portions of this lesson were adapted from or informed by:
* [Atomsk Documentation](https://atomsk.univ-lille.fr/doc/)
* [LAMMPS Documentation](https://docs.lammps.org/)

## Lesson Versions & Intended Modalities

One notebook is provided. It can be used for independent work or in class.

| Modality     | Pedagogy                | Role of Instructor                                                  | Lesson Version                    |
|--------------|-------------------------|---------------------------------------------------------------------|-----------------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                                  | `atomsk-structure-building.ipynb` |
| Synchronous  | Guided Inquiry Learning | Demonstrate the Atomsk commands and check the structures in OVITO   | `atomsk-structure-building.ipynb` |

Running the notebook writes example Atomsk commands to
`atomsk/example_atomsk_commands.txt` and a LAMMPS input skeleton for an
Atomsk generated aluminum structure to `lammps/in.import_atomsk_al`. The
exercises build FCC Cu, BCC Fe, and diamond Si, compare small and large cells,
convert a structure to XYZ for OVITO, create a vacancy and compare atom counts,
and run an energy minimization in LAMMPS.

No separate instructor key or instructor notes notebook is currently provided
for this lesson.
