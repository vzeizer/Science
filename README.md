# **Stoner3D_FSMA**

## This notebook shows how to generate magnetic hysteresis loops of Ni2MnGa through a coherent-model (very) extended approach.

# Installation

$ git clone 

# Documentation

## **Introduction**

In this notebook it is shown the code created to simulate Ferromagnetic Shape Memory Alloys (FSMA).
Through minimization of the free energy density at different strenghts of magnetic field, we were able to simulate the magnetization reversal of thin films and rolled-up Nanomembranes of Ni<sub>2</sub>MnGa.

## **Theoretical Approach**

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

**The flat nanomembrane was tranformed into a rolled-up nanomembrane by means of convenient rotations of the strain tensor.**
Afterwards, in the same way as did in the flat nanomembrane, magnetic hysteresis loops were calculated.

# Suported Python Versions

The code can be run with Python 3.0 or above.

# What to install

1. python 3.4 or greater
2. numba
3. NumPy
4. scipy

# LICENSE

Stoner3D_FSMA is written and maintained by Vagner Zeizer Carvalho Paes.

## MIT License

Copyright (c) 2019 Vagner Zeizer C. Paes

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

