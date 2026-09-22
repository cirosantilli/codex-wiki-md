<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The four [laws of black-hole mechanics](../../../../../laws-of-black-hole-mechanics.md) closely parallel thermodynamics. The zeroth law says that the [surface gravity](../../../../../surface-gravity.md) $\kappa$ is constant over a stationary Killing horizon. The first law is

$$
\delta M=\frac{\kappa}{8\pi G}\delta A
+\Omega_H\delta J+\Phi_H\delta Q.
$$

The second law is [Hawking's area theorem](../../../../../hawking-s-area-theorem.md), $\delta A\geq0$ under the [null energy condition](../../../../../null-energy-condition.md), and the [third law of black-hole mechanics](../../../../../third-law-of-black-hole-mechanics.md) says that a regular extremal horizon with $\kappa=0$ cannot be reached by a finite physical process. These match constancy of temperature in equilibrium, $dE=T\,dS+$ work terms, entropy increase, and unattainability of zero temperature.

Quantum field theory makes the analogy literal. A stationary horizon emits at the [Hawking temperature](../../../../../hawking-temperature.md)

$$
T_H=\frac{\hbar\kappa}{2\pi k_Bc}.
$$

Comparing $T_HdS$ with the area term in the first law gives the [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md)

$$
\boxed{S_{\rm BH}=\frac{k_Bc^3A}{4G\hbar}}.
$$

For a Schwarzschild black hole, $\kappa=c^4/(4GM)$ and $T_H=\hbar c^3/(8\pi GMk_B)$.

To see why particles are produced, quantize a real scalar field using the conserved [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md). In the asymptotically Minkowski past choose positive-frequency modes $u_i^{\rm in}$ and write

$$
\widehat\Phi=\sum_i(a_i^{\rm in}u_i^{\rm in}
+a_i^{{\rm in}\dagger}u_i^{{\rm in}*}).
$$

The asymptotically Minkowski future supplies another positive-frequency basis $u_j^{\rm out}$ and operators $a_j^{\rm out}$. In a nonstationary middle region there is no preferred timelike Killing vector and therefore no invariant positive-frequency split: the notion of particle is observer- and basis-dependent. The two mode bases are related by a [Bogoliubov transformation](../../../../../bogoliubov-transformation.md),

$$
u_j^{\rm out}=\sum_i(\alpha_{ji}u_i^{\rm in}
+\beta_{ji}u_i^{{\rm in}*}),
$$

so the corresponding operators mix annihilation and creation operators. The in-vacuum then contains

$$
\langle0_{\rm in}|N_j^{\rm out}|0_{\rm in}\rangle
=\sum_i|\beta_{ji}|^2
$$

out-particles whenever $\beta\ne0$.

For a black hole formed by collapse, late outgoing modes traced backwards toward the event horizon undergo an exponentially large blueshift. This produces a universal Bogoliubov mixing with

$$
\langle N_\omega\rangle
=\frac1{e^{2\pi\omega/\kappa}-1},
$$

the Planck distribution at $T_H$. Greybody scattering outside the horizon modifies the flux reaching infinity but not its characteristic temperature.

Hawking radiation gives a black hole negative heat capacity: it heats up as it loses mass and can evaporate in finite time. The [generalized second law](../../../../../generalized-second-law.md) assigns entropy $S_{\rm BH}$ to the hole and states that this plus exterior entropy does not decrease. The enormous area entropy suggests microscopic horizon degrees of freedom. If semiclassical evaporation ends with only thermal radiation, an initially pure state appears to become mixed, producing the [black hole information paradox](../../../../../black-hole-information-paradox.md). Resolving the endpoint, information recovery, and the microscopic origin of the area law are central constraints on quantum gravity.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 311](../../paper-311-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
