<div align="center">
    <img src="https://github.com/sanguinariojoe/imp_logo/blob/main/imp_logo_text.svg?raw=true" width="85%" alt="IMP logo">
</div>

# What is the IMP?

The IMP is a fascinating and playful entity, known for its delightful mischief.
It bestows unwavering stability upon any SPH practitioner clever enough to
unravel a conundrum --a fixed-point problem that eludes even the most
determined attempts of Newton's method.

# Why should I adopt an IMP?

There are several features that make IMP really well suited for SPH:

## Unconditional stability

Given its exact energy conservation, IMP is turning your SPH models
unconditionally stable.

**No need for any dissipation term! Not even viscosity!**

For the time being, the energy conservation is demonstrated for compressible
and weakly-compressible SPH incarnations.
Some on-going theoretical progress is done on Incompressible-SPH.

## Spectral convergence

Although adopting an IMP implies solving a fixed-point problem, the numerical
experiments show that the residues are spectrally converging.

**No better scenario can be figured out!**

Indeed, IMP is able to outperform typically used time integrators on SPH, like
Improved-Euler or 4th order Runge-Kutta, with just 4 or 5 iterations.

## Easy to implement

Adopting IMP is almost free!

| Code | Core code lines | Other code lines |
| --- | --- | --- |
| [AQUAgpusph](http://canal.etsin.upm.es/aquagpusph/) | 116 | 33 |
| [DualSPHysics](https://dual.sphysics.org/) | ~500 | ~10 |
| [PySPH](https://pysph.readthedocs.io/en/latest/) | ~750 | ~0 |
| [GPUSPH](https://www.gpusph.org/) | ~1000 | ~50 |

For the time being [AQUAgpusph](http://canal.etsin.upm.es/aquagpusph/) is the
only SPH code which already adopted the IMP.
Stimations are provided though for the most popular SPH implementations.
If you are a developer and you already adopted the IMP, please
[submit an issue](https://github.com/sanguinariojoe/adopt_the_imp/issues).
I will happily check it and update the table.

# Citing

Cercos-Pita, J. L., et al. "SPH energy conservation for fluid–solid interactions." <em>Computer Methods in Applied Mechanics and Engineering</em> 317 (2017): 771-791.

Cercos-Pita, J. L., et al. "The role of time integration in energy conservation in Smoothed Particle Hydrodynamics fluid dynamics simulations." <em>European Journal of Mechanics-B/Fluids</em> 97 (2023): 78-92.

Cercos-Pita, J. L., et al. "Boundary conditions for SPH through energy conservation." <em>Computers & Fluids</em> 285 (2024): 106454.

Merino-Alonso, P. & Violeau, D. "Energy conservation in ISPH" <em>17th ERCOFTAC SPHERIC workshop</em> (2023).
