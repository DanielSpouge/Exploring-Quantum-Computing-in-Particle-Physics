
# Exploring Quantum Computing in Particle Physics

**MSci Research Project | Durham University | 2024**

This project was completed as part of my final-year MSci in Natural Sciences (Mathematics and Physics) at Durham University, under the supervision of Professor B. Pecjak.

## Overview

Quantum computers offer the potential to simulate quantum field theories (QFTs) that are computationally challenging to study using classical methods. However, representing continuous quantum fields on a finite number of qubits requires approximating their infinite-dimensional Hilbert spaces using finite-dimensional representations. This process, known as *digitisation*, inevitably introduces approximation errors.

The first part of this project reviews and reproduces existing research into two digitisation frameworks for scalar quantum fields: the **Jordan–Lee–Preskill (JLP) basis** and the **Harmonic Oscillator (HO) basis**. Their accuracy in calculating ground-state energy is investigated for free and self-interacting scalar field theories, focusing on how digitisation errors depend on the number of qubits and the choice of basis parameters.

The second part builds on this foundation, investigating whether **Hamiltonian Truncation Effective Theory (HTET)** can be used to improve the accuracy of eigenenergy calculations in the HO basis through second-order corrections, without substantially increasing quantum computing resource requirements. Whilst these corrections were found to require relatively modest additional quantum computing resources, numerical results showed no reliable improvement in calculated eigenenergy accuracy over the original HO basis approach.


## Python Notebooks

Numerical investigations were carried out in Python using NumPy and Matplotlib. The notebooks found in this repository contain the code used to generate six figures from the dissertation through the construction and diagonalisation of digitised Hamiltonian matrices.

| Notebook | Description |
|---|---|
| [01 – Field-Space Digitisation](notebooks/01_Field_Space_Digitisation.ipynb) | Figures 6-7: Investigates digitisation errors for free scalar-field theory and compares the JLP and HO bases for a strongly coupled self-interacting theory. |
| [02 – HO Basis Corrections](notebooks/02_HO_Basis_Corrections.ipynb) | Figures 8-10: Compares first- and second-order HO basis calculations for free, weakly coupled and strongly coupled scalar field theories |
| [03 – JLP vs HO Comparison](notebooks/03_JLP_vs_HO_Comparison.ipynb) | Figure 11: Compares the JLP basis against the second-order HO basis for the strongly coupled theory. |

The calculations use classical numerical methods to investigate the accuracy of Hamiltonians intended for representation on ideal quantum computers; no quantum hardware was used.

## Dissertation

The full dissertation, including the theoretical background, mathematical derivations and discussion of results, is available below.

**[Read the full dissertation](dissertation/Exploring_Quantum_Computing_in_Particle_Physics.pdf)**

## Tools

Python · NumPy · Matplotlib · Jupyter Notebook