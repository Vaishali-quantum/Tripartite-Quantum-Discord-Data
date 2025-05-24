Title: Code and Data for the manuscript "Experimental Determination of Tripartite Quantum Discord"

Description:
This repository contains the experimental data and codes used in the preparation of the manuscript "Experimental Determination of Tripartite Quantum Discord." This repository contains the data and code necessary to reproduce the key result of the paper—the calculation of tripartite quantum discord for three-qubit states.

1. Quantum State Tomography (MATLAB)
Main file: three_qubit_sdp_optimised.m
Supporting files: Included in the same folder.

This script reconstructs the experimental density matrix from NMR data and computes fidelity with a theoretical state. The method is based on the approach described in this article:Gaikwad, A., Arvind & Dorai, K. True experimental reconstruction of quantum states and processes via convex optimization. Quantum Inf Process 20, 19 (2021).https://doi.org/10.1007/s11128-020-02930-z

To run:
Place the following data files in the same folder and execute the script. They are read in this order (as referenced in the code):

1h_real

1h_imag

19f_real

19f_imag

13c_real

13c_imag

The output is the experimental density matrix.

NMR data of GHZ states is in the GHZ_data folder; similar folders exist for other states.


2. Optimised Basis Calculation (Mathematica)
File: discord_optimalbases_calculation.nb
This notebook generates optimised measurement bases for the theoretical state. These are used in the experimental discord calculation step.

3. Discord Calculation (Mathematica)
File: Experimental_Discord.nb
Uses the experimental density matrix and the optimised bases from the previous steps to compute the tripartite quantum discord and its components.



