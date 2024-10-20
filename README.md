### SQQ - Superconducting Quantum Research Program – Chip Design Projects ###

#Project 1: Setting up a new device type for user queries:

Go find a device geometry that is not already implemented in SQuADDS, like two coupled differential transmons, a transmon with readout cavity and Purcell filter, two transmons coupled via a tunable coupler, etc., based on a published research article. This article must have enough information published so that you can fully reconstruct the device Hamiltonian--that is, all mode frequencies, anharmonicities, and couplings must be given explicitly or be easily obtainable from other data in the paper. Write code to generate the design (using Qiskit Metal), to vary relevant design geometry parameters (e.g., the dimensions of a coupling capacitor), to simulate it (using PALACE or ANSYS HFSS), and to extract the parameters of an effective lumped-element model that will give the correct effective Hamiltonian. Run quick-and-dirty simulations to see if your simulation results are vaguely close to the published data. Once you've accomplished this, contact the corresponding author of the paper and ask them if you have their permission to contribute the design to SQuADDS--if not, promise to keep it confidential.
The winning project will be given computing time on the Levenson-Falk Lab's workstations to run more accurate simulations, then will be asked to contribute the design if the author approves.

See SQuADDS wish list for detailed ideas: https://github.com/LFL-Lab/SQuADDS/blob/master/wish_list.md 

---------------------------------------------------------------------------------------------------------

#Project 2: Create machine learning model for generating a device geometry for a given target Hamiltonian, based on data already in SQuADDS: 

Currently, when a user inputs a target Hamiltonian, SQuADDS returns them the best-matching pre-simulated design and also uses a physics-based algorithm to give them an estimated best-fit design that has not yet been simulated. This algorithm is difficult to derive and does not generalize well. This is an ideal case for machine learning. Using the SQuADDS database on HuggingFace, create a ML model that is capable of generating a geometry that will give the correct behavior based on a user's target, without running an electromagnetic simulation. Ideally, your model should be able to train on some subset of the SQuADDS database and then generate the rest of the database with reasonable accuracy. Bonus points if your model is easily adapted to other types of design geometry.
The winning project will be asked to deploy on the SQuADDS HuggingFace account.

See SQuADDS wish list for detailed ideas: https://github.com/LFL-Lab/SQuADDS/blob/master/wish_list.md 

---------------------------------------------------------------------------------------------------------

#Project 3: Reliable integration with open-source EM solver: 

Currently, SQuADDS generates code to simulate designs using ANSYS, and the database was entirely simulated in ANSYS. However, ANSYS is expensive--it would be better to switch to some free / open-source solver. One such solver is AWS PALACE, but others may be available. Write wrapper code to export a design from SQuADDS into one of these solvers, run an accurate simulation, and import the results back into SQuADDS. Validate your simulation pipeline using the experimentally-measured WM1 chip from the SQuADDS database--show that you can match the device parameters using your simulations.
The winning project will be asked to deploy to the SQuADDS package.

See SQuADDS wish list for detailed ideas: https://github.com/LFL-Lab/SQuADDS/blob/master/wish_list.md 

---------------------------------------------------------------------------------------------------------

#Project 4: Design an optical mask for a simple multi-transmon device where the transmons have optimized Purcell-limited T1:

Some Reference: https://qiskit-community.github.io/qiskit-metal/circuit-examples/index.html#small-quantum-chips 

---------------------------------------------------------------------------------------------------------

#Project 5: Design transmons of varying Ej/Ec and look for strategies to further reduce the surface participation ratio and radiative losses from the best found in the literature:

Some References:
1. https://www.nature.com/articles/s41534-022-00530-6
2. https://sites.google.com/quantala.tech/website/scientific-papers?authuser=0
3. https://arxiv.org/abs/2204.07202

---------------------------------------------------------------------------------------------------------

#Project 6: Specify two superconducting transmons using Qubit simulator and simulate their energy spectrum:

Some Reference: https://github.com/Borealis126/QSM

---------------------------------------------------------------------------------------------------------

#Project 7: Design a transmon in a creative way to minimize “antenna modes” from the best values found in the literature:

Some References:
1. https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.132.017001
2. https://arxiv.org/abs/2203.06577

---------------------------------------------------------------------------------------------------------

#Project 8: Design a transmon in a creative way to minimize Purcell decay from the best values found in the literature:

Some References:
1. https://arxiv.org/abs/2405.10107
2. https://arxiv.org/abs/2409.04967
3. https://journals.aps.org/prx/pdf/10.1103/PhysRevX.14.041007

---------------------------------------------------------------------------------------------------------

#Project 9: 

Some References:


---------------------------------------------------------------------------------------------------------

#Project 10: 

Some References:


---------------------------------------------------------------------------------------------------------
