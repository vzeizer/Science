# **Introduction**

In this notebook it is shown the code created to simulate Ferromagnetic Shape Memory Alloys (FSMA).
Through minimization of the free energy density at different strenghts of magnetic field, we were able to simulate the magnetization reversal of thin films and rolled-up Nanomembranes of Ni<sub>2</sub>MnGa.

# **Theoretical Approach**

The current approach is to use energy minimization arguments to obtain the hysteresis loops.
The following energy terms were included:

1. Zeeman energy of the mirrored magnetic domains;
2. Magnetocrystalline energy of the responsive domain;
3. Elastic energy of the responsive domain, using a proper phenomenology to describe martensitic transformations;
4. Stress energy which is due to mechanical energy; again the proper phenomenology has been taken into account;
5. Curvature-induced anisotropy, when the nanomembrane is curved.

## Simulation of Flat Nanomembranes

The flat nanomembrane hysteresis was calculated by means of minimization of each element of the film in Python 3.
In order to accelerate the calculations, we used NumPy and @numba decorators.

## Simulation of Rolled-Up Nanomembranes

** The flat nanomembrane was tranformed into a rolled-up nanomembrane by means of convenient rotations of the strain tensor. **
Afterwards, in the same way as did in the flat nanomembrane, magnetic hysteresis loops were calculated.


