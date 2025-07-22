<div align="center">
    <img src="https://github.com/sanguinariojoe/imp_logo/blob/main/imp_logo_text.svg?raw=true" width="85%" alt="IMP logo">
</div>

# What is the IMP?

The IMP is a fascinating and playful entity, known for its delightful mischief.
It bestows unwavering stability upon any SPH practitioner clever enough to
unravel a conundrum --a fixed-point problem that eludes even the most
determined attempts of Newton's method.

# Why should I adopt an IMP?

The IMP offers several advantages that make it an attractive choice for SPH
simulations.

## Unconditional stability

One of the key benefits of the IMP method is its ability to ensure
unconditional stability in SPH models.
This is achieved through exact energy conservation, **which eliminates the need
for dissipation terms.**

Currently, the energy conservation property of the IMP method has been
demonstrated for compressible and Weakly-Compressible SPH formulations.
Ongoing theoretical work is also being conducted on Incompressible SPH.

## Spectral convergence

Although the IMP method requires solving a fixed-point problem, numerical
experiments have shown that the residues converge spectrally.

**An ideal scenario for numerical simulations**

In fact, the IMP method has been shown to outperform commonly used time
integrators in SPH, such as Improved-Euler and 4th order Runge-Kutta, with just
4 or 5 iterations.

## Easy to implement

Adopting the IMP method is relatively straightforward and requires minimal
additional code.

| Code | Core code lines | Other code lines |
| --- | --- | --- |
| [AQUAgpusph](https://aquagpusph.org/) | 116 | 33 |
| [TNL-SPH](https://gitlab.com/tnl-project/tnl-sph) | 337 | 0 |
| [DualSPHysics](https://dual.sphysics.org/) | ~500 | ~10 |
| [PySPH](https://pysph.readthedocs.io/en/latest/) | ~750 | ~0 |
| [GPUSPH](https://www.gpusph.org/) | ~1000 | ~50 |

Currently, [AQUAgpusph](https://aquagpusph.org/) and
[TNL-SPH](https://gitlab.com/tnl-project/tnl-sph) are the only IMP
adopters.
However, estimates are provided for other popular SPH implementations.
If you are a developer who has adopetd an IMP, please
[submit an issue](https://github.com/sanguinariojoe/adopt_the_imp/issues) so
that we can update the table.

Some details on how it is implemented on AQUAgpusph can be found [here](https://github.com/sanguinariojoe/adopt_the_imp/wiki/AQUAgpusph)

# Citing

Cercos-Pita, J. L., et al. "SPH energy conservation for fluid–solid interactions." <em>Computer Methods in Applied Mechanics and Engineering</em> 317 (2017): 771-791.

Cercos-Pita, J. L., et al. "The role of time integration in energy conservation in Smoothed Particle Hydrodynamics fluid dynamics simulations." <em>European Journal of Mechanics-B/Fluids</em> 97 (2023): 78-92. (Available on [arXiv](https://arxiv.org/abs/2210.12372))

Cercos-Pita, J. L., et al. "Boundary conditions for SPH through energy conservation." <em>Computers & Fluids</em> 285 (2024): 106454. (Available on [arXiv](https://arxiv.org/abs/2410.08573))

Merino-Alonso, P. & Violeau, D. "Energy conservation in ISPH" <em>17th ERCOFTAC SPHERIC workshop</em> (2023).
