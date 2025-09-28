# Phase-Filed-implmentaion-of-composite-fracture-
Set of Fortran, FEniCS scripts in the implentaion of elasto-plastic composite fracture using a non-local damage model
# Advanced Fracture Modeling in Composite Materials

*A Phase-Field Approach Incorporating Elasto-Plasticity and Non-Local Effects*

---

## Authors

* **Dr. Altaf Ahmad Lone** (Postdoctoral Researcher)
* **Dr. Mayank Agrawal** (Postdoctoral Researcher)
* **Prof. Durai Prabhakaran** (Professor, IIT Jammu)

**Affiliation:**
Department of Mechanical Engineering
Composite Materials and Mechanics Laboratory
Indian Institute of Technology Jammu

---

## Overview

This repository contains the implementation of the **phase-field method** for simulating crack initiation and propagation in fiber-reinforced composite lamina. The model is based on **finite element analysis** using the [FEniCS](https://fenicsproject.org/) framework, and incorporates:

* Orthotropic material behavior with fiber orientation
* Phase-field fracture evolution driven by energy release rates
* Iterative staggered scheme for displacement and phase-field coupling
* Visualization of crack patterns and load–displacement responses

The code is intended for academic research and reproducibility of results published under the title:
**“Advanced Fracture Modeling in Composite Materials: A Phase-Field Approach Incorporating Elasto-Plasticity and Non-Local Effects.”**

---

## Features

* Automated mesh generation for notched composite lamina
* Energy-based crack-driving force formulation
* Displacement-controlled loading with fracture evolution
* Output files for post-processing (`.csv`, `.xdmf`, `.png`)

---

## Requirements

* Python ≥ 3.8
* FEniCS ≥ 2019.1.0
* NumPy
* Matplotlib
* mshr

---

## Usage

1. Install [FEniCS](https://fenicsproject.org/download/).
2. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
3. Run the simulation:

   ```bash
   python composite_phasefield.py
   ```
4. Output files will be generated in:

   ```
   IITJammu_Composite_Analysis/
   ```

---

## Output

* **`simulation_results.csv`** → displacement vs. reaction force
* **`field_results.xdmf`** → crack pattern visualization (ParaView)
* **`phase_field_final.png`** → phase-field contour plot
* **`load_displacement_curve.png`** → load–displacement response

---

## Documentation

A full technical documentation (with details of the formulation and implementation) is available in the `docs/` folder.

---

## License

For academic and research use only. Please cite the authors and institution when using this code.

---

## Citation

If you use this repository in your research, please cite:

**Lone, A.A., Agrawal, M., Prabhakaran, D.**
*Advanced Fracture Modeling in Composite Materials: A Phase-Field Approach Incorporating Elasto-Plasticity and Non-Local Effects*.
Department of Mechanical Engineering, IIT Jammu.
