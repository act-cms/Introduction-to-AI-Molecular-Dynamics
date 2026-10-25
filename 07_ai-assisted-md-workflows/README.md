Lesson 07: AI-Assisted MD Workflows
===================================

The purpose of this lesson is to introduce responsible use of AI and large
language models (LLMs) in molecular dynamics (MD) workflows. Students use AI
tools to plan simulations, draft scripts, and summarize outputs, and they audit
every result for physical and technical correctness before trusting it.

## Lesson Information
### Lesson Learning Outcomes
At the end of this lesson, students will be able to...
1. Identify useful roles for AI assistants in MD workflows, and their limits.
2. Draft and revise MD scripts with AI assistance, using prompts that ask the
   assistant to state its assumptions and possible mistakes.
3. Audit AI generated code for physical and technical correctness with a
   checklist: units, atom style, potential, boundary conditions, time step,
   ensemble, outputs, and a small test run.
4. Summarize simulation outputs and error messages with AI help, and verify the
   summaries against documentation and results.
5. Plan a parameter sweep as a table that can drive a simulation campaign, and
   keep prompts, generated code, corrections, and logs together so that the
   work can be reproduced.

### Estimated Time

75 to 90 minutes.

### Cyberinfrastructure Prerequisites

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax, including simple pandas tables
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* LAMMPS input scripts and output
    - [Lesson 03](../03_lammps-fundamentals/) to
      [Lesson 06](../06_defects-and-materials-modeling/)
* Access to an AI assistant or LLM chat tool for the exercises

### Content Prerequisites

Before beginning this lesson, students are expected to be familiar with the
following content topics:

* The AI, machine learning, and LLM concepts in
  [Lesson 01](../01_AI-MD-101/)
* Units, boundary conditions, potentials, time steps, and ensembles in MD
  simulations

### Resources

* [LAMMPS Documentation](https://docs.lammps.org/)
* [LAMMPS Commands](https://docs.lammps.org/Commands_all.html)
* [pandas Documentation](https://pandas.pydata.org/docs/)

### References

Portions of this lesson were adapted from or informed by:
* [LAMMPS Documentation](https://docs.lammps.org/)
* The AI and LLM material in Lesson 01 of this module

## Lesson Versions & Intended Modalities

One notebook is provided. It can be used for independent work or in class.

| Modality     | Pedagogy                | Role of Instructor                                                         | Lesson Version                   |
|--------------|-------------------------|----------------------------------------------------------------------------|----------------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                                         | `ai-assisted-md-workflows.ipynb` |
| Synchronous  | Guided Inquiry Learning | Lead the audit of AI generated scripts and discuss what to accept or reject | `ai-assisted-md-workflows.ipynb` |

Running the notebook creates the folders `prompts/`, `lammps/`, `analysis/`, and
`figures/`, writes an example prompt for a LAMMPS script
(`prompts/lammps_lj_prompt.txt`), prints the audit checklist, and writes a
temperature sweep plan (`analysis/temperature_sweep_plan.csv`). The exercises
ask students to draft a LAMMPS script with an AI assistant and audit it, verify
an AI explanation of a LAMMPS error message against the documentation, test an
AI drafted log parser on a known log file, write a prompt that asks for
assumptions and failure modes, and compare two AI generated scripts for
physical soundness.

No separate instructor key or instructor notes notebook is currently provided
for this lesson.
