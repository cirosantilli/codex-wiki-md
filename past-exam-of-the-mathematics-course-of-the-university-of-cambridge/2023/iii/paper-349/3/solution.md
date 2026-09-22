<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Kennicutt–Schmidt law](../../../../../kennicutt-schmidt-law.md) is the empirical relation

$$
\Sigma_{\rm SFR}=A\Sigma_g^N,
\qquad N\simeq1.4
$$

for disk-averaged total gas, with a nearly linear molecular-gas relation in many resolved observations. Atomic gas is mapped through the H I 21-cm line, molecular gas mainly through carbon-monoxide line emission and a CO-to-$\mathrm H_2$ conversion factor, and star formation through combinations of ultraviolet continuum, H-alpha recombination emission, and infrared dust emission. Inclination, dust attenuation, the [initial mass function](../../../../../initial-mass-function.md), tracer lifetimes, and conversion factors must be treated consistently.

The gas-depletion time $M_g/\dot M_*$ is typically of order a gigayear, whereas a giant molecular cloud has a dynamical or free-fall time of order a few megayears. Star formation is therefore inefficient per collapse time, commonly at the percent level, rather than converting an entire cloud in one free fall.

For the first [closed-box model of galactic chemical evolution](../../../../../closed-box-model-of-galactic-chemical-evolution.md), neglect returned mass or absorb it into the definitions. Then

$$
\frac{dM_g}{dt}=-\dot M_*=-\frac{M_g}{\tau_*},
$$

and hence

$$
\boxed{M_g=M_{g0}e^{-t/\tau_*},
\qquad \dot M_*=\frac{M_{g0}}{\tau_*}e^{-t/\tau_*},
\qquad Z=y_Z\log\frac{M_{g0}}{M_g}=\frac{y_Zt}{\tau_*}.}
$$

Thus a region reaching $Z_\odot=0.014$ after an enrichment time $t_\odot$ with $y_Z=0.006$ has

$$
\boxed{\tau_*=\frac{y_Z}{Z_\odot}t_\odot\simeq0.43t_\odot,}
$$

about $4.3\,\mathrm{Gyr}$ for a fiducial $t_\odot\simeq10\,\mathrm{Gyr}$ enrichment age of the Galactic disk.

The second prescription implies $\dot M_*=M_g^2/(M_{g0}\widetilde\tau_*)$. Solving the gas-consumption equation gives

$$
\boxed{M_g=\frac{M_{g0}}{1+t/\widetilde\tau_*},
\qquad
\dot M_*=\frac{M_{g0}}{\widetilde\tau_*}
\left(1+\frac{t}{\widetilde\tau_*}\right)^{-2},
\qquad
Z=y_Z\log\left(1+\frac{t}{\widetilde\tau_*}\right).}
$$

Therefore

$$
\boxed{\widetilde\tau_*
=\frac{t_\odot}{e^{Z_\odot/y_Z}-1}
\simeq0.107t_\odot\simeq1.1\,\mathrm{Gyr}.}
$$

For long-lived stars, $dN$ is proportional to $dM_*=-dM_g$. In the exponential model,

$$
\frac{dN}{dZ}\propto
\dot M_*\frac{dt}{dZ}
=\frac{M_{g0}}{y_Z}e^{-Z/y_Z}.
$$

In the second model, $1+t/\widetilde\tau_*=e^{Z/y_Z}$; multiplying its star-formation rate by $dt/dZ$ gives exactly the same result:

$$
\boxed{\frac{dN}{dZ}\propto e^{-Z/y_Z}.}
$$

The metallicity distribution is fixed by the closed-box relation $M_g/M_{g0}=e^{-Z/y_Z}$ and is independent of the star-formation history. Merely changing the time law therefore does not cure the [G-dwarf problem](../../../../../g-dwarf-problem.md); gas inflow, outflow, variable yields, or selection effects must alter the closed-box assumptions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
